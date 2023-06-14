# Comparing `tmp/mpl_format-0.317.tar.gz` & `tmp/mpl_format-0.318.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_format-0.317.tar", last modified: Sat Jun 10 23:04:56 2023, max compression
+gzip compressed data, was "mpl_format-0.318.tar", last modified: Wed Jun 14 16:38:25 2023, max compression
```

## Comparing `mpl_format-0.317.tar` & `mpl_format-0.318.tar`

### file list

```diff
@@ -1,102 +1,101 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.393500 mpl_format-0.317/
--rw-rw-rw-   0        0        0     1080 2022-01-23 23:53:12.000000 mpl_format-0.317/LICENSE.txt
--rw-rw-rw-   0        0        0      473 2023-06-10 23:04:56.393500 mpl_format-0.317/PKG-INFO
--rw-rw-rw-   0        0        0      156 2022-01-23 23:53:12.000000 mpl_format-0.317/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:55.853360 mpl_format-0.317/mpl_format/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:55.900635 mpl_format-0.317/mpl_format/animation/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:55.918632 mpl_format-0.317/mpl_format/animation/animators/
--rw-rw-rw-   0        0        0       41 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/animators/__init__.py
--rw-rw-rw-   0        0        0     1125 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/animators/axes_animator.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:55.947787 mpl_format-0.317/mpl_format/animation/kwarg_animations/
--rw-rw-rw-   0        0        0       90 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/kwarg_animations/__init__.py
--rw-rw-rw-   0        0        0     4070 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/kwarg_animations/color_animation.py
--rw-rw-rw-   0        0        0     4970 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/kwarg_animations/float_animation.py
--rw-rw-rw-   0        0        0      864 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/rate.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.058596 mpl_format-0.317/mpl_format/animation/shapes/
--rw-rw-rw-   0        0        0      387 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/__init__.py
--rw-rw-rw-   0        0        0     3272 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/arc_animation.py
--rw-rw-rw-   0        0        0     2807 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/arrow_animation.py
--rw-rw-rw-   0        0        0     1558 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/base.py
--rw-rw-rw-   0        0        0     2639 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/circle_animation.py
--rw-rw-rw-   0        0        0     2871 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/ellipse_animation.py
--rw-rw-rw-   0        0        0     4032 2023-05-26 22:01:30.000000 mpl_format-0.317/mpl_format/animation/shapes/line_animation.py
--rw-rw-rw-   0        0        0     3676 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/rectangle_animation.py
--rw-rw-rw-   0        0        0     2856 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/regular_polygon_animation.py
--rw-rw-rw-   0        0        0     4190 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/text_animation.py
--rw-rw-rw-   0        0        0     3015 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/wedge_animation.py
--rw-rw-rw-   0        0        0      461 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/type_animations.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.090695 mpl_format-0.317/mpl_format/axes/
--rw-rw-rw-   0        0        0      314 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/axes/__init__.py
--rw-rw-rw-   0        0        0   112188 2023-05-26 22:01:06.000000 mpl_format-0.317/mpl_format/axes/axes_formatter.py
--rw-rw-rw-   0        0        0     1141 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/axes/axes_formatter_array.py
--rw-rw-rw-   0        0        0    15475 2022-10-29 21:01:39.000000 mpl_format-0.317/mpl_format/axes/axis_formatter.py
--rw-rw-rw-   0        0        0     9782 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/axes/axis_formatter_array.py
--rw-rw-rw-   0        0        0      413 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/axes/axis_utils.py
--rw-rw-rw-   0        0        0    14000 2023-06-10 22:56:32.000000 mpl_format-0.317/mpl_format/axes/ticks_formatter.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.106324 mpl_format-0.317/mpl_format/colors/
--rw-rw-rw-   0        0        0      163 2022-10-29 21:01:39.000000 mpl_format-0.317/mpl_format/colors/__init__.py
--rw-rw-rw-   0        0        0     1688 2023-05-26 21:46:47.000000 mpl_format-0.317/mpl_format/colors/color_maps.py
--rw-rw-rw-   0        0        0     5671 2022-10-29 21:01:39.000000 mpl_format-0.317/mpl_format/colors/office.py
--rw-rw-rw-   0        0        0     3209 2023-06-10 22:55:58.000000 mpl_format-0.317/mpl_format/compound_types.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.233989 mpl_format-0.317/mpl_format/enums/
--rw-rw-rw-   0        0        0      698 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/__init__.py
--rw-rw-rw-   0        0        0     1113 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/arrow_style.py
--rw-rw-rw-   0        0        0     1152 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/box_style.py
--rw-rw-rw-   0        0        0      389 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/cap_style.py
--rw-rw-rw-   0        0        0      686 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/connection_style.py
--rw-rw-rw-   0        0        0      751 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/draw_style.py
--rw-rw-rw-   0        0        0      775 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/font_size.py
--rw-rw-rw-   0        0        0     1053 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/font_stretch.py
--rw-rw-rw-   0        0        0      404 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/font_style.py
--rw-rw-rw-   0        0        0      553 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/font_variant.py
--rw-rw-rw-   0        0        0     1145 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/font_weight.py
--rw-rw-rw-   0        0        0      395 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/join_style.py
--rw-rw-rw-   0        0        0      618 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/line_style.py
--rw-rw-rw-   0        0        0      648 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/mappings.py
--rw-rw-rw-   0        0        0     2439 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/marker_style.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.265605 mpl_format-0.317/mpl_format/figures/
--rw-rw-rw-   0        0        0       65 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/figures/__init__.py
--rw-rw-rw-   0        0        0    30493 2023-05-26 21:58:33.000000 mpl_format-0.317/mpl_format/figures/figure_formatter.py
--rw-rw-rw-   0        0        0        6 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/figures/figure_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.275303 mpl_format-0.317/mpl_format/legend/
--rw-rw-rw-   0        0        0       64 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/legend/__init__.py
--rw-rw-rw-   0        0        0    17325 2023-05-26 21:58:25.000000 mpl_format-0.317/mpl_format/legend/legend_formatter.py
--rw-rw-rw-   0        0        0      706 2023-05-26 21:46:47.000000 mpl_format-0.317/mpl_format/literals.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.297647 mpl_format-0.317/mpl_format/patches/
--rw-rw-rw-   0        0        0       72 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/patches/__init__.py
--rw-rw-rw-   0        0        0      981 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/patches/arc_list_formatter.py
--rw-rw-rw-   0        0        0     2781 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/patches/patch_list_formatter.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.313714 mpl_format-0.317/mpl_format/plots/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/plots/__init__.py
--rw-rw-rw-   0        0        0    10229 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/plots/density.py
--rw-rw-rw-   0        0        0       43 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.345413 mpl_format-0.317/mpl_format/text/
--rw-rw-rw-   0        0        0      125 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/text/__init__.py
--rw-rw-rw-   0        0        0     8104 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/text/text_formatter.py
--rw-rw-rw-   0        0        0     5287 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/text/text_list_formatter.py
--rw-rw-rw-   0        0        0     2366 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/text/text_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.381492 mpl_format-0.317/mpl_format/utils/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/utils/__init__.py
--rw-rw-rw-   0        0        0      386 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/utils/arg_checks.py
--rw-rw-rw-   0        0        0     2825 2022-10-29 21:01:39.000000 mpl_format-0.317/mpl_format/utils/arg_transforms.py
--rw-rw-rw-   0        0        0     2157 2023-05-26 21:58:25.000000 mpl_format-0.317/mpl_format/utils/color_utils.py
--rw-rw-rw-   0        0        0     2054 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/utils/io_utils.py
--rw-rw-rw-   0        0        0     1210 2023-06-10 22:56:32.000000 mpl_format-0.317/mpl_format/utils/number_utils.py
--rw-rw-rw-   0        0        0      890 2023-05-26 22:01:06.000000 mpl_format-0.317/mpl_format/utils/type_checks.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:55.878458 mpl_format-0.317/mpl_format.egg-info/
--rw-rw-rw-   0        0        0      473 2023-06-10 23:04:55.000000 mpl_format-0.317/mpl_format.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2817 2023-06-10 23:04:55.000000 mpl_format-0.317/mpl_format.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 23:04:55.000000 mpl_format-0.317/mpl_format.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 23:04:55.000000 mpl_format-0.317/mpl_format.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-10 23:04:55.000000 mpl_format-0.317/mpl_format.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-10 23:04:56.409447 mpl_format-0.317/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-06-10 23:04:05.000000 mpl_format-0.317/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.393500 mpl_format-0.317/tests/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/tests/__init__.py
--rw-rw-rw-   0        0        0     4256 2022-01-23 23:53:12.000000 mpl_format-0.317/tests/test_axis_formatter.py
--rw-rw-rw-   0        0        0      385 2022-01-23 23:53:12.000000 mpl_format-0.317/tests/test_figure_formatter.py
-drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.393500 mpl_format-0.317/tests/test_text/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/tests/test_text/__init__.py
--rw-rw-rw-   0        0        0     1363 2022-01-23 23:53:12.000000 mpl_format-0.317/tests/test_text/test_text_utils.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.447967 mpl_format-0.318/
+-rw-r--r--   0 vahndi     (505) staff       (20)      495 2023-06-14 16:38:25.448330 mpl_format-0.318/PKG-INFO
+-rw-r--r--   0 vahndi     (505) staff       (20)      148 2021-10-12 11:13:45.000000 mpl_format-0.318/README.md
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.381991 mpl_format-0.318/mpl_format/
+-rw-r--r--   0 vahndi     (505) staff       (20)        0 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/__init__.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.387351 mpl_format-0.318/mpl_format/animation/
+-rw-r--r--   0 vahndi     (505) staff       (20)        0 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/__init__.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.388917 mpl_format-0.318/mpl_format/animation/animators/
+-rw-r--r--   0 vahndi     (505) staff       (20)       40 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/animators/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     1090 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/animators/axes_animator.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.391434 mpl_format-0.318/mpl_format/animation/kwarg_animations/
+-rw-r--r--   0 vahndi     (505) staff       (20)       88 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/kwarg_animations/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     3955 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/kwarg_animations/color_animation.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     4824 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/kwarg_animations/float_animation.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      833 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/rate.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.401369 mpl_format-0.318/mpl_format/animation/shapes/
+-rw-r--r--   0 vahndi     (505) staff       (20)      379 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/shapes/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     3202 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/shapes/arc_animation.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     2745 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/shapes/arrow_animation.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     1510 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/shapes/base.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     2581 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/shapes/circle_animation.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     2808 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/shapes/ellipse_animation.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     3945 2023-06-14 16:16:48.000000 mpl_format-0.318/mpl_format/animation/shapes/line_animation.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     3597 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/shapes/rectangle_animation.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     2796 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/shapes/regular_polygon_animation.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     4105 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/shapes/text_animation.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     2950 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/shapes/wedge_animation.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      451 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/animation/type_animations.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.409264 mpl_format-0.318/mpl_format/axes/
+-rw-r--r--   0 vahndi     (505) staff       (20)      309 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/axes/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)   109643 2023-06-14 16:37:25.000000 mpl_format-0.318/mpl_format/axes/axes_formatter.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     1098 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/axes/axes_formatter_array.py
+-rw-r--r--   0 vahndi     (505) staff       (20)    14990 2022-03-16 19:21:01.000000 mpl_format-0.318/mpl_format/axes/axis_formatter.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     9465 2021-11-27 15:42:23.000000 mpl_format-0.318/mpl_format/axes/axis_formatter_array.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      397 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/axes/axis_utils.py
+-rw-r--r--   0 vahndi     (505) staff       (20)    13584 2023-06-14 16:16:48.000000 mpl_format-0.318/mpl_format/axes/ticks_formatter.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.411755 mpl_format-0.318/mpl_format/colors/
+-rw-r--r--   0 vahndi     (505) staff       (20)      160 2022-02-01 02:19:12.000000 mpl_format-0.318/mpl_format/colors/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     1638 2023-05-22 13:05:37.000000 mpl_format-0.318/mpl_format/colors/color_maps.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     5469 2022-02-01 02:19:12.000000 mpl_format-0.318/mpl_format/colors/office.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     3109 2023-06-14 16:16:48.000000 mpl_format-0.318/mpl_format/compound_types.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.425647 mpl_format-0.318/mpl_format/enums/
+-rw-r--r--   0 vahndi     (505) staff       (20)      685 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     1066 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/arrow_style.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     1105 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/box_style.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      372 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/cap_style.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      657 2021-11-30 23:00:47.000000 mpl_format-0.318/mpl_format/enums/connection_style.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      720 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/draw_style.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      742 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/font_size.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     1016 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/font_stretch.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      387 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/font_style.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      530 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/font_variant.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     1098 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/font_weight.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      378 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/join_style.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      592 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/line_style.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      630 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/mappings.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     2352 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/enums/marker_style.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.427855 mpl_format-0.318/mpl_format/figures/
+-rw-r--r--   0 vahndi     (505) staff       (20)       64 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/figures/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)    29597 2023-06-14 16:16:48.000000 mpl_format-0.318/mpl_format/figures/figure_formatter.py
+-rw-r--r--   0 vahndi     (505) staff       (20)        3 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/figures/figure_utils.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.429201 mpl_format-0.318/mpl_format/legend/
+-rw-r--r--   0 vahndi     (505) staff       (20)       63 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/legend/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)    16911 2023-06-14 16:16:48.000000 mpl_format-0.318/mpl_format/legend/legend_formatter.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      692 2022-05-05 19:56:23.000000 mpl_format-0.318/mpl_format/literals.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.431287 mpl_format-0.318/mpl_format/patches/
+-rw-r--r--   0 vahndi     (505) staff       (20)       71 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/patches/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      939 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/patches/arc_list_formatter.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     2680 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/patches/patch_list_formatter.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.433143 mpl_format-0.318/mpl_format/plots/
+-rw-r--r--   0 vahndi     (505) staff       (20)        0 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/plots/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     9941 2021-11-30 23:01:06.000000 mpl_format-0.318/mpl_format/plots/density.py
+-rw-r--r--   0 vahndi     (505) staff       (20)       41 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/settings.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.437219 mpl_format-0.318/mpl_format/text/
+-rw-r--r--   0 vahndi     (505) staff       (20)      123 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/text/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     7821 2022-01-19 23:13:28.000000 mpl_format-0.318/mpl_format/text/text_formatter.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     5094 2021-11-30 21:48:57.000000 mpl_format-0.318/mpl_format/text/text_list_formatter.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     2289 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/text/text_utils.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.443859 mpl_format-0.318/mpl_format/utils/
+-rw-r--r--   0 vahndi     (505) staff       (20)        0 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/utils/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      373 2021-11-27 15:40:24.000000 mpl_format-0.318/mpl_format/utils/arg_checks.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     2739 2022-01-26 02:45:18.000000 mpl_format-0.318/mpl_format/utils/arg_transforms.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     2085 2023-06-14 16:16:48.000000 mpl_format-0.318/mpl_format/utils/color_utils.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     1977 2021-10-12 10:43:40.000000 mpl_format-0.318/mpl_format/utils/io_utils.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     1172 2023-06-14 16:16:48.000000 mpl_format-0.318/mpl_format/utils/number_utils.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      851 2023-06-14 16:16:48.000000 mpl_format-0.318/mpl_format/utils/type_checks.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.385481 mpl_format-0.318/mpl_format.egg-info/
+-rw-r--r--   0 vahndi     (505) staff       (20)      495 2023-06-14 16:38:25.000000 mpl_format-0.318/mpl_format.egg-info/PKG-INFO
+-rw-r--r--   0 vahndi     (505) staff       (20)     2805 2023-06-14 16:38:25.000000 mpl_format-0.318/mpl_format.egg-info/SOURCES.txt
+-rw-r--r--   0 vahndi     (505) staff       (20)        1 2023-06-14 16:38:25.000000 mpl_format-0.318/mpl_format.egg-info/dependency_links.txt
+-rw-r--r--   0 vahndi     (505) staff       (20)       42 2023-06-14 16:38:25.000000 mpl_format-0.318/mpl_format.egg-info/requires.txt
+-rw-r--r--   0 vahndi     (505) staff       (20)       17 2023-06-14 16:38:25.000000 mpl_format-0.318/mpl_format.egg-info/top_level.txt
+-rw-r--r--   0 vahndi     (505) staff       (20)       79 2023-06-14 16:38:25.449748 mpl_format-0.318/setup.cfg
+-rw-r--r--   0 vahndi     (505) staff       (20)      730 2023-06-14 16:37:32.000000 mpl_format-0.318/setup.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.445734 mpl_format-0.318/tests/
+-rw-r--r--   0 vahndi     (505) staff       (20)        0 2021-10-12 10:43:40.000000 mpl_format-0.318/tests/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     4134 2021-10-12 10:43:40.000000 mpl_format-0.318/tests/test_axis_formatter.py
+-rw-r--r--   0 vahndi     (505) staff       (20)      372 2021-10-12 10:43:40.000000 mpl_format-0.318/tests/test_figure_formatter.py
+drwxr-xr-x   0 vahndi     (505) staff       (20)        0 2023-06-14 16:38:25.447093 mpl_format-0.318/tests/test_text/
+-rw-r--r--   0 vahndi     (505) staff       (20)        0 2021-10-12 10:43:40.000000 mpl_format-0.318/tests/test_text/__init__.py
+-rw-r--r--   0 vahndi     (505) staff       (20)     1324 2021-10-12 10:43:40.000000 mpl_format-0.318/tests/test_text/test_text_utils.py
```

### Comparing `mpl_format-0.317/mpl_format/animation/animators/axes_animator.py` & `mpl_format-0.318/mpl_format/animation/animators/axes_animator.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from typing import Union, List
-
-from celluloid import Camera
-from numpy import linspace
-
-from mpl_format.animation.shapes.base import ShapeAnimation
-from mpl_format.axes import AxesFormatter
-from mpl_format.figures import FigureFormatter
-
-
-class AxesAnimator(object):
-
-    def __init__(self,
-                 formatter: Union[AxesFormatter, FigureFormatter],
-                 duration: float):
-
-        self.formatter: AxesFormatter = formatter or AxesFormatter()
-        self.duration: float = duration
-        self.shapes: List[ShapeAnimation] = []
-
-    def add_animation(self, animation: ShapeAnimation):
-
-        self.shapes.append(animation)
-
-    def animate(self, file_name: str, fps: float = 30):
-
-        camera = Camera(self.formatter.axes.figure)
-        for t in linspace(
-                0, self.duration, 1 + int(self.duration * fps)
-        ):
-            for shape in self.shapes:
-                shape.draw(t / self.duration, axes=self.formatter)
-            camera.snap()
-        animation = camera.animate()
-        animation.save(file_name, writer='imagemagick', fps=30)
+from typing import Union, List
+
+from celluloid import Camera
+from numpy import linspace
+
+from mpl_format.animation.shapes.base import ShapeAnimation
+from mpl_format.axes import AxesFormatter
+from mpl_format.figures import FigureFormatter
+
+
+class AxesAnimator(object):
+
+    def __init__(self,
+                 formatter: Union[AxesFormatter, FigureFormatter],
+                 duration: float):
+
+        self.formatter: AxesFormatter = formatter or AxesFormatter()
+        self.duration: float = duration
+        self.shapes: List[ShapeAnimation] = []
+
+    def add_animation(self, animation: ShapeAnimation):
+
+        self.shapes.append(animation)
+
+    def animate(self, file_name: str, fps: float = 30):
+
+        camera = Camera(self.formatter.axes.figure)
+        for t in linspace(
+                0, self.duration, 1 + int(self.duration * fps)
+        ):
+            for shape in self.shapes:
+                shape.draw(t / self.duration, axes=self.formatter)
+            camera.snap()
+        animation = camera.animate()
+        animation.save(file_name, writer='imagemagick', fps=30)
```

### Comparing `mpl_format-0.317/mpl_format/animation/kwarg_animations/color_animation.py` & `mpl_format-0.318/mpl_format/animation/kwarg_animations/color_animation.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-from typing import List, Union, Optional
-
-from numpy import linspace, sin, pi, sign, arcsin
-
-from mpl_format.compound_types import Color
-from mpl_format.animation.rate import Rate
-from mpl_format.utils.color_utils import set_alpha, cross_fade
-
-
-class ColorAnimation(object):
-
-    def __init__(self,
-                 colors: List[Color],
-                 t: Optional[List[float]] = None,
-                 rate: Optional[Union[Rate, str]] = None):
-
-        self.colors: List[Color] = colors
-        if t is not None:
-            self.t: List[float] = t
-        else:
-            self.t = list(linspace(0, 1, len(colors)))
-        self.rate: Rate = (
-            Rate.linear() if rate is None else
-            rate if isinstance(rate, Rate) else
-            Rate(rate)
-        )
-
-    @staticmethod
-    def fade_in(color: Color) -> 'ColorAnimation':
-
-        return ColorAnimation(
-            colors=[set_alpha(color, 0), color],
-            t=[0, 1]
-        )
-
-    @classmethod
-    def sine_wave(cls, color_1: Color, color_2: Color,
-                  cycles: float, phase: float = 0.0) -> 'ColorAnimation':
-        """
-        Return a sine wave oscillating between color_1 and color_2,
-        starting at phase * 2π with cycles complete waves.
-
-        :param color_1: Lowest color of the wave.
-        :param color_2: Highest color of the wave.
-        :param cycles: Number of complete oscillations.
-        :param phase: Value from 0 to 1 of where to start the wave.
-        """
-        middle_val = 0.5
-        amplitude = 0.5
-        rate = Rate(lambda t: (
-                middle_val +
-                amplitude * sin((2 * pi * t * cycles) - (2 * pi * phase))
-        ))
-        return ColorAnimation(colors=[color_1, color_2],
-                              rate=rate)
-
-    @classmethod
-    def square_wave(cls, color_1: Color, color_2: Color,
-                    cycles: float, phase: float = 0.0) -> 'ColorAnimation':
-        """
-        Return a square wave oscillating between min_val and max_val,
-        starting at phase * 2π with cycles complete waves.
-
-        :param color_1: Lowest color of the wave.
-        :param color_2: Highest color of the wave.
-        :param cycles: Number of complete oscillations.
-        :param phase: Value from 0 to 1 of where to start the wave.
-        """
-        middle_val = 0.5
-        amplitude = 0.5
-        rate = Rate(lambda t: (
-                middle_val +
-                amplitude * sign(
-                    sin((2 * pi * t * cycles) - (2 * pi * phase))
-                )
-        ))
-        return ColorAnimation(colors=[color_1, color_2],
-                              rate=rate)
-
-    @classmethod
-    def triangle_wave(cls, color_1: Color, color_2: Color,
-                      cycles: float, phase: float = 0.0) -> 'ColorAnimation':
-        """
-        Return a triangle wave oscillating between min_val and max_val,
-        starting at phase * 2π with cycles complete waves.
-
-        :param color_1: Lowest color of the wave.
-        :param color_2: Highest color of the wave.
-        :param cycles: Number of complete oscillations.
-        :param phase: Value from 0 to 1 of where to start the wave.
-        """
-        middle_val = 0.5
-        amplitude = 0.5
-        rate = Rate(lambda t: (
-                middle_val +
-                2 * amplitude * arcsin(
-                    sin((2 * pi * t * cycles) - (2 * pi * phase))
-                ) / pi
-        ))
-        return ColorAnimation(colors=[color_1, color_2],
-                              rate=rate)
-
-    def at(self, t: float) -> Color:
-
-        for i in range(len(self.t)):
-            if self.t[i + 1] >= t:
-                dt = self.rate(
-                    (t - self.t[i]) /
-                    (self.t[i + 1] - self.t[i])
-                )
-                return cross_fade(
-                    from_color=self.colors[i],
-                    to_color=self.colors[i + 1],
-                    amount=dt
-                )
+from typing import List, Union, Optional
+
+from numpy import linspace, sin, pi, sign, arcsin
+
+from mpl_format.compound_types import Color
+from mpl_format.animation.rate import Rate
+from mpl_format.utils.color_utils import set_alpha, cross_fade
+
+
+class ColorAnimation(object):
+
+    def __init__(self,
+                 colors: List[Color],
+                 t: Optional[List[float]] = None,
+                 rate: Optional[Union[Rate, str]] = None):
+
+        self.colors: List[Color] = colors
+        if t is not None:
+            self.t: List[float] = t
+        else:
+            self.t = list(linspace(0, 1, len(colors)))
+        self.rate: Rate = (
+            Rate.linear() if rate is None else
+            rate if isinstance(rate, Rate) else
+            Rate(rate)
+        )
+
+    @staticmethod
+    def fade_in(color: Color) -> 'ColorAnimation':
+
+        return ColorAnimation(
+            colors=[set_alpha(color, 0), color],
+            t=[0, 1]
+        )
+
+    @classmethod
+    def sine_wave(cls, color_1: Color, color_2: Color,
+                  cycles: float, phase: float = 0.0) -> 'ColorAnimation':
+        """
+        Return a sine wave oscillating between color_1 and color_2,
+        starting at phase * 2π with cycles complete waves.
+
+        :param color_1: Lowest color of the wave.
+        :param color_2: Highest color of the wave.
+        :param cycles: Number of complete oscillations.
+        :param phase: Value from 0 to 1 of where to start the wave.
+        """
+        middle_val = 0.5
+        amplitude = 0.5
+        rate = Rate(lambda t: (
+                middle_val +
+                amplitude * sin((2 * pi * t * cycles) - (2 * pi * phase))
+        ))
+        return ColorAnimation(colors=[color_1, color_2],
+                              rate=rate)
+
+    @classmethod
+    def square_wave(cls, color_1: Color, color_2: Color,
+                    cycles: float, phase: float = 0.0) -> 'ColorAnimation':
+        """
+        Return a square wave oscillating between min_val and max_val,
+        starting at phase * 2π with cycles complete waves.
+
+        :param color_1: Lowest color of the wave.
+        :param color_2: Highest color of the wave.
+        :param cycles: Number of complete oscillations.
+        :param phase: Value from 0 to 1 of where to start the wave.
+        """
+        middle_val = 0.5
+        amplitude = 0.5
+        rate = Rate(lambda t: (
+                middle_val +
+                amplitude * sign(
+                    sin((2 * pi * t * cycles) - (2 * pi * phase))
+                )
+        ))
+        return ColorAnimation(colors=[color_1, color_2],
+                              rate=rate)
+
+    @classmethod
+    def triangle_wave(cls, color_1: Color, color_2: Color,
+                      cycles: float, phase: float = 0.0) -> 'ColorAnimation':
+        """
+        Return a triangle wave oscillating between min_val and max_val,
+        starting at phase * 2π with cycles complete waves.
+
+        :param color_1: Lowest color of the wave.
+        :param color_2: Highest color of the wave.
+        :param cycles: Number of complete oscillations.
+        :param phase: Value from 0 to 1 of where to start the wave.
+        """
+        middle_val = 0.5
+        amplitude = 0.5
+        rate = Rate(lambda t: (
+                middle_val +
+                2 * amplitude * arcsin(
+                    sin((2 * pi * t * cycles) - (2 * pi * phase))
+                ) / pi
+        ))
+        return ColorAnimation(colors=[color_1, color_2],
+                              rate=rate)
+
+    def at(self, t: float) -> Color:
+
+        for i in range(len(self.t)):
+            if self.t[i + 1] >= t:
+                dt = self.rate(
+                    (t - self.t[i]) /
+                    (self.t[i + 1] - self.t[i])
+                )
+                return cross_fade(
+                    from_color=self.colors[i],
+                    to_color=self.colors[i + 1],
+                    amount=dt
+                )
```

### Comparing `mpl_format-0.317/mpl_format/animation/kwarg_animations/float_animation.py` & `mpl_format-0.318/mpl_format/animation/kwarg_animations/float_animation.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-from numpy import pi, sin, sign, arcsin
-from typing import List, Union, Optional
-
-from mpl_format.animation.rate import Rate
-
-
-class FloatAnimation(object):
-
-    def __init__(self,
-                 values: Optional[List[float]] = None,
-                 t: Optional[List[float]] = None,
-                 rate: Optional[Union[Rate, str]] = None):
-
-        if values is not None:
-            self.values: List[float] = values
-        else:
-            self.values = [0, 1]
-        if t is not None:
-            self.t: List[float] = t
-        else:
-            self.t = [0, 1]
-        self.rate: Rate = (
-            Rate.linear() if rate is None else
-            rate if isinstance(rate, Rate) else
-            Rate(rate)
-        )
-
-    def set_values(self, values: List[float]) -> 'FloatAnimation':
-
-        self.values = values
-        return self
-
-    def reverse_values(self) -> 'FloatAnimation':
-
-        return FloatAnimation(
-            values=self.values[:: -1],
-            t=self.t, rate=self.rate
-        )
-
-    @classmethod
-    def linear(cls) -> 'FloatAnimation':
-        return FloatAnimation(rate='linear')
-
-    @classmethod
-    def quadratic(cls) -> 'FloatAnimation':
-        return FloatAnimation(rate='quadratic')
-
-    @classmethod
-    def cubic(cls) -> 'FloatAnimation':
-        return FloatAnimation(rate='cubic')
-
-    @classmethod
-    def sine_wave(cls, min_val: float, max_val: float,
-                  cycles: float, phase: float = 0.0) -> 'FloatAnimation':
-        """
-        Return a sine wave oscillating between min_val and max_val,
-        starting at phase * 2π with cycles complete waves.
-
-        :param min_val: Lowest value of the wave.
-        :param max_val: Highest value of the wave.
-        :param cycles: Number of complete oscillations.
-        :param phase: Value from 0 to 1 of where to start the wave.
-        """
-        middle_val = (min_val + max_val) / 2
-        amplitude = (max_val - min_val) / 2
-        rate = Rate(lambda t: (
-                middle_val +
-                amplitude * sin((2 * pi * t * cycles) - (2 * pi * phase))
-        ))
-        return FloatAnimation(rate=rate)
-
-    @classmethod
-    def square_wave(cls, min_val: float, max_val: float,
-                    cycles: float, phase: float = 0.0) -> 'FloatAnimation':
-        """
-        Return a square wave oscillating between min_val and max_val,
-        starting at phase * 2π with cycles complete waves.
-
-        :param min_val: Lowest value of the wave.
-        :param max_val: Highest value of the wave.
-        :param cycles: Number of complete oscillations.
-        :param phase: Value from 0 to 1 of where to start the wave.
-        """
-        middle_val = (min_val + max_val) / 2
-        amplitude = (max_val - min_val) / 2
-        rate = Rate(lambda t: (
-                middle_val +
-                amplitude * sign(
-                    sin((2 * pi * t * cycles) - (2 * pi * phase))
-                )
-        ))
-        return FloatAnimation(rate=rate)
-
-    @classmethod
-    def triangle_wave(cls, min_val: float, max_val: float,
-                      cycles: float, phase: float = 0.0) -> 'FloatAnimation':
-        """
-        Return a triangle wave oscillating between min_val and max_val,
-        starting at phase * 2π with cycles complete waves.
-
-        :param min_val: Lowest value of the wave.
-        :param max_val: Highest value of the wave.
-        :param cycles: Number of complete oscillations.
-        :param phase: Value from 0 to 1 of where to start the wave.
-        """
-        middle_val = (min_val + max_val) / 2
-        amplitude = (max_val - min_val) / 2
-        rate = Rate(lambda t: (
-                middle_val +
-                2 * amplitude * arcsin(
-                    sin((2 * pi * t * cycles) - (2 * pi * phase))
-                ) / pi
-        ))
-        return FloatAnimation(rate=rate)
-
-    @classmethod
-    def rotation(cls, cycles: float,
-                 clockwise: bool = True,
-                 phase: Optional[float] = 0.0):
-        """
-        Return a rotation in degrees.
-
-        :param cycles: Number of complete rotations.
-        :param clockwise: Rotate clockwise if True.
-        :param phase: Starting phase between 0.0 and 1.0.
-        """
-        if clockwise:
-            multiplier = -1
-        else:
-            multiplier = 1
-        return FloatAnimation(rate=Rate(
-            lambda t: (phase * 360) + multiplier * t * cycles * 360
-        ))
-
-    def at(self, t: float) -> float:
-
-        for i in range(len(self.t)):
-            if self.t[i + 1] >= t:
-                dt = self.rate(
-                    (t - self.t[i]) /
-                    (self.t[i + 1] - self.t[i])
-                )
-                return (
-                    self.values[i] +
-                    (self.values[i + 1] - self.values[i]) * dt
-                )
+from numpy import pi, sin, sign, arcsin
+from typing import List, Union, Optional
+
+from mpl_format.animation.rate import Rate
+
+
+class FloatAnimation(object):
+
+    def __init__(self,
+                 values: Optional[List[float]] = None,
+                 t: Optional[List[float]] = None,
+                 rate: Optional[Union[Rate, str]] = None):
+
+        if values is not None:
+            self.values: List[float] = values
+        else:
+            self.values = [0, 1]
+        if t is not None:
+            self.t: List[float] = t
+        else:
+            self.t = [0, 1]
+        self.rate: Rate = (
+            Rate.linear() if rate is None else
+            rate if isinstance(rate, Rate) else
+            Rate(rate)
+        )
+
+    def set_values(self, values: List[float]) -> 'FloatAnimation':
+
+        self.values = values
+        return self
+
+    def reverse_values(self) -> 'FloatAnimation':
+
+        return FloatAnimation(
+            values=self.values[:: -1],
+            t=self.t, rate=self.rate
+        )
+
+    @classmethod
+    def linear(cls) -> 'FloatAnimation':
+        return FloatAnimation(rate='linear')
+
+    @classmethod
+    def quadratic(cls) -> 'FloatAnimation':
+        return FloatAnimation(rate='quadratic')
+
+    @classmethod
+    def cubic(cls) -> 'FloatAnimation':
+        return FloatAnimation(rate='cubic')
+
+    @classmethod
+    def sine_wave(cls, min_val: float, max_val: float,
+                  cycles: float, phase: float = 0.0) -> 'FloatAnimation':
+        """
+        Return a sine wave oscillating between min_val and max_val,
+        starting at phase * 2π with cycles complete waves.
+
+        :param min_val: Lowest value of the wave.
+        :param max_val: Highest value of the wave.
+        :param cycles: Number of complete oscillations.
+        :param phase: Value from 0 to 1 of where to start the wave.
+        """
+        middle_val = (min_val + max_val) / 2
+        amplitude = (max_val - min_val) / 2
+        rate = Rate(lambda t: (
+                middle_val +
+                amplitude * sin((2 * pi * t * cycles) - (2 * pi * phase))
+        ))
+        return FloatAnimation(rate=rate)
+
+    @classmethod
+    def square_wave(cls, min_val: float, max_val: float,
+                    cycles: float, phase: float = 0.0) -> 'FloatAnimation':
+        """
+        Return a square wave oscillating between min_val and max_val,
+        starting at phase * 2π with cycles complete waves.
+
+        :param min_val: Lowest value of the wave.
+        :param max_val: Highest value of the wave.
+        :param cycles: Number of complete oscillations.
+        :param phase: Value from 0 to 1 of where to start the wave.
+        """
+        middle_val = (min_val + max_val) / 2
+        amplitude = (max_val - min_val) / 2
+        rate = Rate(lambda t: (
+                middle_val +
+                amplitude * sign(
+                    sin((2 * pi * t * cycles) - (2 * pi * phase))
+                )
+        ))
+        return FloatAnimation(rate=rate)
+
+    @classmethod
+    def triangle_wave(cls, min_val: float, max_val: float,
+                      cycles: float, phase: float = 0.0) -> 'FloatAnimation':
+        """
+        Return a triangle wave oscillating between min_val and max_val,
+        starting at phase * 2π with cycles complete waves.
+
+        :param min_val: Lowest value of the wave.
+        :param max_val: Highest value of the wave.
+        :param cycles: Number of complete oscillations.
+        :param phase: Value from 0 to 1 of where to start the wave.
+        """
+        middle_val = (min_val + max_val) / 2
+        amplitude = (max_val - min_val) / 2
+        rate = Rate(lambda t: (
+                middle_val +
+                2 * amplitude * arcsin(
+                    sin((2 * pi * t * cycles) - (2 * pi * phase))
+                ) / pi
+        ))
+        return FloatAnimation(rate=rate)
+
+    @classmethod
+    def rotation(cls, cycles: float,
+                 clockwise: bool = True,
+                 phase: Optional[float] = 0.0):
+        """
+        Return a rotation in degrees.
+
+        :param cycles: Number of complete rotations.
+        :param clockwise: Rotate clockwise if True.
+        :param phase: Starting phase between 0.0 and 1.0.
+        """
+        if clockwise:
+            multiplier = -1
+        else:
+            multiplier = 1
+        return FloatAnimation(rate=Rate(
+            lambda t: (phase * 360) + multiplier * t * cycles * 360
+        ))
+
+    def at(self, t: float) -> float:
+
+        for i in range(len(self.t)):
+            if self.t[i + 1] >= t:
+                dt = self.rate(
+                    (t - self.t[i]) /
+                    (self.t[i + 1] - self.t[i])
+                )
+                return (
+                    self.values[i] +
+                    (self.values[i + 1] - self.values[i]) * dt
+                )
```

### Comparing `mpl_format-0.317/mpl_format/animation/rate.py` & `mpl_format-0.318/mpl_format/animation/rate.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Callable, Union
-
-
-class Rate(object):
-
-    def __init__(self, lambda_t: Union[str, Callable[[float], float]]):
-
-        if isinstance(lambda_t, str):
-            if hasattr(self, lambda_t):
-                self._lambda_t: Union[str, Callable[[float], float]] = \
-                    getattr(self, lambda_t)()
-            else:
-                raise ValueError(f'Rate class has no method {lambda_t}')
-        else:
-            self._lambda_t: Callable[[float], float] = lambda_t
-
-    def __call__(self, t: float) -> float:
-
-        return self._lambda_t(t)
-
-    @classmethod
-    def linear(cls) -> 'Rate':
-        return Rate(lambda t: t)
-
-    @classmethod
-    def quadratic(cls) -> 'Rate':
-        return Rate(lambda t: t ** 2)
-
-    @classmethod
-    def cubic(cls) -> 'Rate':
-        return Rate(lambda t: t ** 3)
+from typing import Callable, Union
+
+
+class Rate(object):
+
+    def __init__(self, lambda_t: Union[str, Callable[[float], float]]):
+
+        if isinstance(lambda_t, str):
+            if hasattr(self, lambda_t):
+                self._lambda_t: Union[str, Callable[[float], float]] = \
+                    getattr(self, lambda_t)()
+            else:
+                raise ValueError(f'Rate class has no method {lambda_t}')
+        else:
+            self._lambda_t: Callable[[float], float] = lambda_t
+
+    def __call__(self, t: float) -> float:
+
+        return self._lambda_t(t)
+
+    @classmethod
+    def linear(cls) -> 'Rate':
+        return Rate(lambda t: t)
+
+    @classmethod
+    def quadratic(cls) -> 'Rate':
+        return Rate(lambda t: t ** 2)
+
+    @classmethod
+    def cubic(cls) -> 'Rate':
+        return Rate(lambda t: t ** 3)
```

### Comparing `mpl_format-0.317/mpl_format/animation/shapes/arc_animation.py` & `mpl_format-0.318/mpl_format/animation/shapes/arc_animation.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from typing import Optional, Union
-
-from mpl_format.animation.shapes.base import ShapeAnimation
-from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
-    StrOrFloatAnimation, StrOrFloatOrFloatAnimation, ColorOrColorAnimation
-from mpl_format.axes import AxesFormatter
-from mpl_format.enums.join_style import JOIN_STYLE
-from mpl_format.enums.cap_style import CAP_STYLE
-from mpl_format.enums.line_style import LINE_STYLE
-
-
-class ArcAnimation(ShapeAnimation, object):
-
-    def __init__(
-            self,
-            x_center: FloatOrFloatAnimation,
-            y_center: FloatOrFloatAnimation,
-            width: FloatOrFloatAnimation,
-            height: FloatOrFloatAnimation,
-            length: Optional[StrOrFloatAnimation] = None,
-            angle: FloatOrFloatAnimation = 0.0,
-            theta_start: FloatOrFloatAnimation = 0.0,
-            theta_end: FloatOrFloatAnimation = 360.0,
-            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
-            cap_style: Optional[Union[str, CAP_STYLE]] = None,
-            color: Optional[ColorOrColorAnimation] = None,
-            edge_color: Optional[ColorOrColorAnimation] = None,
-            join_style: Optional[Union[str, JOIN_STYLE]] = None,
-            label: Optional[str] = None,
-            line_style: Optional[Union[str, LINE_STYLE]] = None,
-            line_width: Optional[FloatOrFloatAnimation] = None
-    ):
-        self.x_center: FloatOrFloatAnimation = x_center
-        self.y_center: FloatOrFloatAnimation = y_center
-        self.width: FloatOrFloatAnimation = width
-        self.height: FloatOrFloatAnimation = height
-        self.length: Optional[StrOrFloatAnimation] = self._float_anim(length)
-        self.angle: FloatOrFloatAnimation = angle
-        self.theta_start: FloatOrFloatAnimation = theta_start
-        self.theta_end: FloatOrFloatAnimation = theta_end
-        self.alpha: FloatOrFloatAnimation = self._float_anim(alpha)
-        self.cap_style: Optional[Union[str, CAP_STYLE]] = cap_style
-        self.color: Optional[ColorOrColorAnimation] = color
-        self.edge_color: Optional[ColorOrColorAnimation] = edge_color
-        self.join_style: Optional[Union[str, JOIN_STYLE]] = join_style
-        self.label: Optional[str] = label
-        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
-        self.line_width: Optional[FloatOrFloatAnimation] = line_width
-
-    def draw(self, t: float, axes: AxesFormatter):
-
-        kwargs = {}
-        if self.length is not None:
-            kwargs['theta_end'] = (
-                self.theta_start +
-                self.length.at(t) * (self.theta_end - self.theta_start)
-            )
-        else:
-            kwargs['theta_end'] = self.theta_end
-        for float_kwarg in (
-                'x_center', 'y_center', 'width', 'height',
-                'angle', 'theta_start', 'alpha', 'line_width'
-        ):
-            self._add_float_kwarg(float_kwarg, kwargs, t)
-        for color_kwarg in ('color', 'edge_color'):
-            self._add_color_kwarg(color_kwarg, kwargs, t)
-        for kwarg in ('cap_style', 'join_style', 'label', 'line_style'):
-            self._add_non_animated_kwarg(kwarg, kwargs)
-
-        axes.add_arc(**kwargs)
+from typing import Optional, Union
+
+from mpl_format.animation.shapes.base import ShapeAnimation
+from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
+    StrOrFloatAnimation, StrOrFloatOrFloatAnimation, ColorOrColorAnimation
+from mpl_format.axes import AxesFormatter
+from mpl_format.enums.join_style import JOIN_STYLE
+from mpl_format.enums.cap_style import CAP_STYLE
+from mpl_format.enums.line_style import LINE_STYLE
+
+
+class ArcAnimation(ShapeAnimation, object):
+
+    def __init__(
+            self,
+            x_center: FloatOrFloatAnimation,
+            y_center: FloatOrFloatAnimation,
+            width: FloatOrFloatAnimation,
+            height: FloatOrFloatAnimation,
+            length: Optional[StrOrFloatAnimation] = None,
+            angle: FloatOrFloatAnimation = 0.0,
+            theta_start: FloatOrFloatAnimation = 0.0,
+            theta_end: FloatOrFloatAnimation = 360.0,
+            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
+            cap_style: Optional[Union[str, CAP_STYLE]] = None,
+            color: Optional[ColorOrColorAnimation] = None,
+            edge_color: Optional[ColorOrColorAnimation] = None,
+            join_style: Optional[Union[str, JOIN_STYLE]] = None,
+            label: Optional[str] = None,
+            line_style: Optional[Union[str, LINE_STYLE]] = None,
+            line_width: Optional[FloatOrFloatAnimation] = None
+    ):
+        self.x_center: FloatOrFloatAnimation = x_center
+        self.y_center: FloatOrFloatAnimation = y_center
+        self.width: FloatOrFloatAnimation = width
+        self.height: FloatOrFloatAnimation = height
+        self.length: Optional[StrOrFloatAnimation] = self._float_anim(length)
+        self.angle: FloatOrFloatAnimation = angle
+        self.theta_start: FloatOrFloatAnimation = theta_start
+        self.theta_end: FloatOrFloatAnimation = theta_end
+        self.alpha: FloatOrFloatAnimation = self._float_anim(alpha)
+        self.cap_style: Optional[Union[str, CAP_STYLE]] = cap_style
+        self.color: Optional[ColorOrColorAnimation] = color
+        self.edge_color: Optional[ColorOrColorAnimation] = edge_color
+        self.join_style: Optional[Union[str, JOIN_STYLE]] = join_style
+        self.label: Optional[str] = label
+        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
+        self.line_width: Optional[FloatOrFloatAnimation] = line_width
+
+    def draw(self, t: float, axes: AxesFormatter):
+
+        kwargs = {}
+        if self.length is not None:
+            kwargs['theta_end'] = (
+                self.theta_start +
+                self.length.at(t) * (self.theta_end - self.theta_start)
+            )
+        else:
+            kwargs['theta_end'] = self.theta_end
+        for float_kwarg in (
+                'x_center', 'y_center', 'width', 'height',
+                'angle', 'theta_start', 'alpha', 'line_width'
+        ):
+            self._add_float_kwarg(float_kwarg, kwargs, t)
+        for color_kwarg in ('color', 'edge_color'):
+            self._add_color_kwarg(color_kwarg, kwargs, t)
+        for kwarg in ('cap_style', 'join_style', 'label', 'line_style'):
+            self._add_non_animated_kwarg(kwarg, kwargs)
+
+        axes.add_arc(**kwargs)
```

### Comparing `mpl_format-0.317/mpl_format/animation/shapes/arrow_animation.py` & `mpl_format-0.318/mpl_format/animation/shapes/regular_polygon_animation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,60 @@
-from typing import Optional, Union
-
-from mpl_format.animation.shapes.base import ShapeAnimation
-from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
-    StrOrFloatOrFloatAnimation, ColorOrColorAnimation
-from mpl_format.axes import AxesFormatter
-from mpl_format.enums.join_style import JOIN_STYLE
-from mpl_format.enums.cap_style import CAP_STYLE
-from mpl_format.enums.line_style import LINE_STYLE
-
-
-class ArrowAnimation(ShapeAnimation, object):
-
-    def __init__(
-            self,
-            x_tail: FloatOrFloatAnimation,
-            y_tail: FloatOrFloatAnimation,
-            dx: FloatOrFloatAnimation,
-            dy: FloatOrFloatAnimation,
-            width: FloatOrFloatAnimation = 1.0,
-            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
-            cap_style: Optional[Union[str, CAP_STYLE]] = None,
-            color: Optional[ColorOrColorAnimation] = None,
-            edge_color: Optional[ColorOrColorAnimation] = None,
-            face_color: Optional[ColorOrColorAnimation] = None,
-            fill: bool = True,
-            join_style: Optional[Union[str, JOIN_STYLE]] = None,
-            label: Optional[str] = None,
-            line_style: Optional[Union[str, LINE_STYLE]] = None,
-            line_width: Optional[FloatOrFloatAnimation] = None,
-    ):
-        self.x_tail: FloatOrFloatAnimation = x_tail
-        self.y_tail: FloatOrFloatAnimation = y_tail
-        self.dx: FloatOrFloatAnimation = dx
-        self.dy: FloatOrFloatAnimation = dy
-        self.width: FloatOrFloatAnimation = width
-        self.alpha: Optional[StrOrFloatOrFloatAnimation] = alpha
-        self.cap_style: Optional[Union[str, CAP_STYLE]] = cap_style
-        self.color: Optional[ColorOrColorAnimation] = color
-        self.edge_color: Optional[ColorOrColorAnimation] = edge_color
-        self.face_color: Optional[ColorOrColorAnimation] = face_color
-        self.fill: bool = fill
-        self.join_style: Optional[Union[str, JOIN_STYLE]] = join_style
-        self.label: Optional[str] = label
-        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
-        self.line_width: Optional[FloatOrFloatAnimation] = line_width
-
-    def draw(self, t: float, axes: AxesFormatter):
-
-        kwargs = {}
-        for float_kwarg in (
-                'x_tail', 'y_tail', 'dx', 'dy',
-                'width', 'alpha', 'line_width',
-        ):
-            self._add_float_kwarg(float_kwarg, kwargs, t)
-        for color_kwarg in ('color', 'edge_color', 'face_color'):
-            self._add_color_kwarg(color_kwarg, kwargs, t)
-        for kwarg in ('cap_style', 'fill', 'join_style',
-                      'label', 'line_style'):
-            self._add_non_animated_kwarg(kwarg, kwargs)
-
-        axes.add_arrow(**kwargs)
+from typing import Optional, Union
+
+from mpl_format.animation.shapes.base import ShapeAnimation
+from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
+    StrOrFloatOrFloatAnimation, ColorOrColorAnimation
+from mpl_format.axes import AxesFormatter
+from mpl_format.enums.join_style import JOIN_STYLE
+from mpl_format.enums.cap_style import CAP_STYLE
+from mpl_format.enums.line_style import LINE_STYLE
+
+
+class RegularPolygonAnimation(ShapeAnimation, object):
+
+    def __init__(
+            self,
+            x_center: FloatOrFloatAnimation,
+            y_center: FloatOrFloatAnimation,
+            num_vertices: int,
+            radius: FloatOrFloatAnimation,
+            angle: FloatOrFloatAnimation = 0,
+            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
+            color: Optional[ColorOrColorAnimation] = None,
+            edge_color: Optional[ColorOrColorAnimation] = None,
+            face_color: Optional[ColorOrColorAnimation] = None,
+            fill: bool = True,
+            label: Optional[str] = None,
+            line_style: Optional[Union[str, LINE_STYLE]] = None,
+            line_width: Optional[FloatOrFloatAnimation] = None,
+            cap_style: Optional[Union[str, CAP_STYLE]] = None,
+            join_style: Optional[Union[str, JOIN_STYLE]] = None,
+    ):
+        self.x_center: FloatOrFloatAnimation = x_center
+        self.y_center: FloatOrFloatAnimation = y_center
+        self.num_vertices: int = num_vertices
+        self.radius: FloatOrFloatAnimation = radius
+        self.angle: FloatOrFloatAnimation = angle
+        self.alpha: Optional[FloatOrFloatAnimation] = self._float_anim(alpha)
+        self.color: Optional[ColorOrColorAnimation] = color
+        self.edge_color: Optional[ColorOrColorAnimation] = edge_color
+        self.face_color: Optional[ColorOrColorAnimation] = face_color
+        self.fill: bool = fill
+        self.label: Optional[str] = label
+        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
+        self.line_width: Optional[FloatOrFloatAnimation] = line_width
+        self.cap_style: Optional[Union[str, CAP_STYLE]] = cap_style
+        self.join_style: Optional[Union[str, JOIN_STYLE]] = join_style
+
+    def draw(self, t: float, axes: AxesFormatter):
+
+        kwargs = {}
+        for float_kwarg in ('x_center', 'y_center', 'radius',
+                            'angle', 'alpha', 'line_width'):
+            self._add_float_kwarg(float_kwarg, kwargs, t)
+        for color_kwarg in ('color', 'edge_color', 'face_color'):
+            self._add_color_kwarg(color_kwarg, kwargs, t)
+        for kwarg in ('num_vertices', 'fill', 'label',
+                      'line_style', 'cap_style', 'join_style'):
+            self._add_non_animated_kwarg(kwarg, kwargs)
+
+        axes.add_regular_polygon(**kwargs)
```

### Comparing `mpl_format-0.317/mpl_format/animation/shapes/base.py` & `mpl_format-0.318/mpl_format/animation/shapes/base.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import Optional
-
-from mpl_format.animation.kwarg_animations.color_animation import ColorAnimation
-from mpl_format.animation.kwarg_animations.float_animation import FloatAnimation
-from mpl_format.animation.type_animations import StrOrFloatAnimation
-from mpl_format.animation.rate import Rate
-from mpl_format.axes import AxesFormatter
-
-
-class ShapeAnimation(object):
-
-    @staticmethod
-    def _float_anim(
-            variable: Optional[StrOrFloatAnimation]
-    ) -> Optional[FloatAnimation]:
-
-        if isinstance(variable, str):
-            variable = FloatAnimation(rate=variable)
-        return variable
-
-    def draw(self, t: float, axes: AxesFormatter):
-
-        raise NotImplementedError
-
-    def _add_non_animated_kwarg(self, arg_name: str, kwargs: dict):
-
-        value = getattr(self, arg_name)
-        if value is not None:
-            kwargs[arg_name] = value
-
-    def _add_color_kwarg(self, arg_name: str, kwargs: dict, t: float):
-
-        value = getattr(self, arg_name)
-        if value is not None:
-            kwargs[arg_name] = (
-                value.at(t) if isinstance(value, ColorAnimation)
-                else value
-            )
-
-    def _add_float_kwarg(self, arg_name: str, kwargs: dict, t: float):
-
-        value = getattr(self, arg_name)
-        if value is not None:
-            kwargs[arg_name] = (
-                value.at(t) if isinstance(value, FloatAnimation)
-                else Rate(value)(t) if isinstance(value, str)
-                else value
-            )
+from typing import Optional
+
+from mpl_format.animation.kwarg_animations.color_animation import ColorAnimation
+from mpl_format.animation.kwarg_animations.float_animation import FloatAnimation
+from mpl_format.animation.type_animations import StrOrFloatAnimation
+from mpl_format.animation.rate import Rate
+from mpl_format.axes import AxesFormatter
+
+
+class ShapeAnimation(object):
+
+    @staticmethod
+    def _float_anim(
+            variable: Optional[StrOrFloatAnimation]
+    ) -> Optional[FloatAnimation]:
+
+        if isinstance(variable, str):
+            variable = FloatAnimation(rate=variable)
+        return variable
+
+    def draw(self, t: float, axes: AxesFormatter):
+
+        raise NotImplementedError
+
+    def _add_non_animated_kwarg(self, arg_name: str, kwargs: dict):
+
+        value = getattr(self, arg_name)
+        if value is not None:
+            kwargs[arg_name] = value
+
+    def _add_color_kwarg(self, arg_name: str, kwargs: dict, t: float):
+
+        value = getattr(self, arg_name)
+        if value is not None:
+            kwargs[arg_name] = (
+                value.at(t) if isinstance(value, ColorAnimation)
+                else value
+            )
+
+    def _add_float_kwarg(self, arg_name: str, kwargs: dict, t: float):
+
+        value = getattr(self, arg_name)
+        if value is not None:
+            kwargs[arg_name] = (
+                value.at(t) if isinstance(value, FloatAnimation)
+                else Rate(value)(t) if isinstance(value, str)
+                else value
+            )
```

### Comparing `mpl_format-0.317/mpl_format/animation/shapes/circle_animation.py` & `mpl_format-0.318/mpl_format/animation/shapes/arrow_animation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-from typing import Optional, Union
-
-from mpl_format.animation.shapes.base import ShapeAnimation
-from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
-    StrOrFloatOrFloatAnimation, ColorOrColorAnimation
-from mpl_format.axes import AxesFormatter
-from mpl_format.enums.join_style import JOIN_STYLE
-from mpl_format.enums.cap_style import CAP_STYLE
-from mpl_format.enums.line_style import LINE_STYLE
-
-
-class CircleAnimation(ShapeAnimation, object):
-
-    def __init__(
-            self,
-            x_center: FloatOrFloatAnimation,
-            y_center: FloatOrFloatAnimation,
-            radius: FloatOrFloatAnimation,
-            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
-            cap_style: Optional[Union[str, CAP_STYLE]] = None,
-            color: Optional[ColorOrColorAnimation] = None,
-            edge_color: Optional[ColorOrColorAnimation] = None,
-            face_color: Optional[ColorOrColorAnimation] = None,
-            fill: bool = True,
-            label: Optional[str] = None,
-            line_style: Optional[Union[str, LINE_STYLE]] = None,
-            line_width: Optional[FloatOrFloatAnimation] = None,
-            join_style: Optional[Union[str, JOIN_STYLE]] = None
-    ):
-        self.x_center: FloatOrFloatAnimation = x_center
-        self.y_center: FloatOrFloatAnimation = y_center
-        self.radius: FloatOrFloatAnimation = radius
-        self.alpha: Optional[StrOrFloatOrFloatAnimation] = alpha
-        self.cap_style: Optional[Union[str, CAP_STYLE]] = cap_style
-        self.color: Optional[ColorOrColorAnimation] = color
-        self.edge_color: Optional[ColorOrColorAnimation] = edge_color
-        self.face_color: Optional[ColorOrColorAnimation] = face_color
-        self.fill: bool = fill
-        self.label: Optional[str] = label
-        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
-        self.line_width: Optional[FloatOrFloatAnimation] = line_width
-        self.join_style: Optional[Union[str, JOIN_STYLE]] = join_style
-
-    def draw(self, t: float, axes: AxesFormatter):
-
-        kwargs = {}
-        for float_kwarg in (
-                'x_center', 'y_center', 'radius',
-                'alpha', 'line_width'
-        ):
-            self._add_float_kwarg(float_kwarg, kwargs, t)
-        for color_kwarg in ('color', 'edge_color', 'face_color'):
-            self._add_color_kwarg(color_kwarg, kwargs, t)
-        for kwarg in ('cap_style', 'fill', 'label',
-                      'line_style', 'join_style'):
-            self._add_non_animated_kwarg(kwarg, kwargs)
-
-        axes.add_circle(**kwargs)
+from typing import Optional, Union
+
+from mpl_format.animation.shapes.base import ShapeAnimation
+from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
+    StrOrFloatOrFloatAnimation, ColorOrColorAnimation
+from mpl_format.axes import AxesFormatter
+from mpl_format.enums.join_style import JOIN_STYLE
+from mpl_format.enums.cap_style import CAP_STYLE
+from mpl_format.enums.line_style import LINE_STYLE
+
+
+class ArrowAnimation(ShapeAnimation, object):
+
+    def __init__(
+            self,
+            x_tail: FloatOrFloatAnimation,
+            y_tail: FloatOrFloatAnimation,
+            dx: FloatOrFloatAnimation,
+            dy: FloatOrFloatAnimation,
+            width: FloatOrFloatAnimation = 1.0,
+            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
+            cap_style: Optional[Union[str, CAP_STYLE]] = None,
+            color: Optional[ColorOrColorAnimation] = None,
+            edge_color: Optional[ColorOrColorAnimation] = None,
+            face_color: Optional[ColorOrColorAnimation] = None,
+            fill: bool = True,
+            join_style: Optional[Union[str, JOIN_STYLE]] = None,
+            label: Optional[str] = None,
+            line_style: Optional[Union[str, LINE_STYLE]] = None,
+            line_width: Optional[FloatOrFloatAnimation] = None,
+    ):
+        self.x_tail: FloatOrFloatAnimation = x_tail
+        self.y_tail: FloatOrFloatAnimation = y_tail
+        self.dx: FloatOrFloatAnimation = dx
+        self.dy: FloatOrFloatAnimation = dy
+        self.width: FloatOrFloatAnimation = width
+        self.alpha: Optional[StrOrFloatOrFloatAnimation] = alpha
+        self.cap_style: Optional[Union[str, CAP_STYLE]] = cap_style
+        self.color: Optional[ColorOrColorAnimation] = color
+        self.edge_color: Optional[ColorOrColorAnimation] = edge_color
+        self.face_color: Optional[ColorOrColorAnimation] = face_color
+        self.fill: bool = fill
+        self.join_style: Optional[Union[str, JOIN_STYLE]] = join_style
+        self.label: Optional[str] = label
+        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
+        self.line_width: Optional[FloatOrFloatAnimation] = line_width
+
+    def draw(self, t: float, axes: AxesFormatter):
+
+        kwargs = {}
+        for float_kwarg in (
+                'x_tail', 'y_tail', 'dx', 'dy',
+                'width', 'alpha', 'line_width',
+        ):
+            self._add_float_kwarg(float_kwarg, kwargs, t)
+        for color_kwarg in ('color', 'edge_color', 'face_color'):
+            self._add_color_kwarg(color_kwarg, kwargs, t)
+        for kwarg in ('cap_style', 'fill', 'join_style',
+                      'label', 'line_style'):
+            self._add_non_animated_kwarg(kwarg, kwargs)
+
+        axes.add_arrow(**kwargs)
```

### Comparing `mpl_format-0.317/mpl_format/animation/shapes/ellipse_animation.py` & `mpl_format-0.318/mpl_format/animation/shapes/circle_animation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,58 @@
-from typing import Optional, Union
-
-from mpl_format.animation.shapes.base import ShapeAnimation
-from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
-    StrOrFloatOrFloatAnimation, ColorOrColorAnimation
-from mpl_format.axes import AxesFormatter
-from mpl_format.enums.join_style import JOIN_STYLE
-from mpl_format.enums.cap_style import CAP_STYLE
-from mpl_format.enums.line_style import LINE_STYLE
-
-
-class EllipseAnimation(ShapeAnimation, object):
-
-    def __init__(
-            self,
-            x_center: FloatOrFloatAnimation,
-            y_center: FloatOrFloatAnimation,
-            width: FloatOrFloatAnimation,
-            height: FloatOrFloatAnimation,
-            angle: FloatOrFloatAnimation = 0.0,
-            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
-            cap_style: Optional[Union[str, CAP_STYLE]] = None,
-            color: Optional[ColorOrColorAnimation] = None,
-            edge_color: Optional[ColorOrColorAnimation] = None,
-            face_color: Optional[ColorOrColorAnimation] = None,
-            fill: bool = True,
-            join_style: Optional[Union[str, JOIN_STYLE]] = None,
-            label: Optional[str] = None,
-            line_style: Optional[Union[str, LINE_STYLE]] = None,
-            line_width: Optional[FloatOrFloatAnimation] = None,
-    ):
-        self.x_center: FloatOrFloatAnimation = x_center
-        self.y_center: FloatOrFloatAnimation = y_center
-        self.width: FloatOrFloatAnimation = width
-        self.height: FloatOrFloatAnimation = height
-        self.angle: FloatOrFloatAnimation = angle
-        self.alpha: Optional[StrOrFloatOrFloatAnimation] = alpha
-        self.cap_style: Optional[Union[str, CAP_STYLE]] = cap_style
-        self.color: Optional[ColorOrColorAnimation] = color
-        self.edge_color: Optional[ColorOrColorAnimation] = edge_color
-        self.face_color: Optional[ColorOrColorAnimation] = face_color
-        self.fill: bool = fill
-        self.join_style: Optional[Union[str, JOIN_STYLE]] = join_style
-        self.label: Optional[str] = label
-        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
-        self.line_width: Optional[FloatOrFloatAnimation] = line_width
-
-    def draw(self, t: float, axes: AxesFormatter):
-
-        kwargs = {}
-        for float_kwarg in (
-                'x_center', 'y_center',
-                'width', 'height', 'angle',
-                'alpha', 'line_width'
-        ):
-            self._add_float_kwarg(float_kwarg, kwargs, t)
-        for color_kwarg in ('color', 'edge_color', 'face_color'):
-            self._add_color_kwarg(color_kwarg, kwargs, t)
-        for kwarg in ('cap_style', 'fill', 'join_style',
-                      'label', 'line_style'):
-            self._add_non_animated_kwarg(kwarg, kwargs)
-
-        axes.add_ellipse(**kwargs)
+from typing import Optional, Union
+
+from mpl_format.animation.shapes.base import ShapeAnimation
+from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
+    StrOrFloatOrFloatAnimation, ColorOrColorAnimation
+from mpl_format.axes import AxesFormatter
+from mpl_format.enums.join_style import JOIN_STYLE
+from mpl_format.enums.cap_style import CAP_STYLE
+from mpl_format.enums.line_style import LINE_STYLE
+
+
+class CircleAnimation(ShapeAnimation, object):
+
+    def __init__(
+            self,
+            x_center: FloatOrFloatAnimation,
+            y_center: FloatOrFloatAnimation,
+            radius: FloatOrFloatAnimation,
+            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
+            cap_style: Optional[Union[str, CAP_STYLE]] = None,
+            color: Optional[ColorOrColorAnimation] = None,
+            edge_color: Optional[ColorOrColorAnimation] = None,
+            face_color: Optional[ColorOrColorAnimation] = None,
+            fill: bool = True,
+            label: Optional[str] = None,
+            line_style: Optional[Union[str, LINE_STYLE]] = None,
+            line_width: Optional[FloatOrFloatAnimation] = None,
+            join_style: Optional[Union[str, JOIN_STYLE]] = None
+    ):
+        self.x_center: FloatOrFloatAnimation = x_center
+        self.y_center: FloatOrFloatAnimation = y_center
+        self.radius: FloatOrFloatAnimation = radius
+        self.alpha: Optional[StrOrFloatOrFloatAnimation] = alpha
+        self.cap_style: Optional[Union[str, CAP_STYLE]] = cap_style
+        self.color: Optional[ColorOrColorAnimation] = color
+        self.edge_color: Optional[ColorOrColorAnimation] = edge_color
+        self.face_color: Optional[ColorOrColorAnimation] = face_color
+        self.fill: bool = fill
+        self.label: Optional[str] = label
+        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
+        self.line_width: Optional[FloatOrFloatAnimation] = line_width
+        self.join_style: Optional[Union[str, JOIN_STYLE]] = join_style
+
+    def draw(self, t: float, axes: AxesFormatter):
+
+        kwargs = {}
+        for float_kwarg in (
+                'x_center', 'y_center', 'radius',
+                'alpha', 'line_width'
+        ):
+            self._add_float_kwarg(float_kwarg, kwargs, t)
+        for color_kwarg in ('color', 'edge_color', 'face_color'):
+            self._add_color_kwarg(color_kwarg, kwargs, t)
+        for kwarg in ('cap_style', 'fill', 'label',
+                      'line_style', 'join_style'):
+            self._add_non_animated_kwarg(kwarg, kwargs)
+
+        axes.add_circle(**kwargs)
```

### Comparing `mpl_format-0.317/mpl_format/animation/shapes/line_animation.py` & `mpl_format-0.318/mpl_format/animation/shapes/line_animation.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from typing import Union, Optional
-
-from numpy import linspace
-from scipy.interpolate import interp1d
-
-from mpl_format.compound_types import FloatIterable
-from mpl_format.animation.kwarg_animations.float_animation import FloatAnimation
-from mpl_format.animation.shapes.base import ShapeAnimation
-from mpl_format.animation.type_animations import \
-    FloatOrFloatAnimation, ColorOrColorAnimation, StrOrFloatAnimation, \
-    StrOrFloatOrFloatAnimation
-from mpl_format.axes import AxesFormatter
-from mpl_format.enums.marker_style import MARKER_STYLE
-from mpl_format.enums.draw_style import DRAW_STYLE
-from mpl_format.enums.line_style import LINE_STYLE
-
-
-class LineAnimation(ShapeAnimation, object):
-
-    def __init__(
-            self,
-            x: FloatIterable,
-            y: FloatIterable,
-            smooth: Union[bool, int] = False,
-            smooth_order: int = 2,
-            length: Optional[StrOrFloatAnimation] = None,
-            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
-            color: Optional[ColorOrColorAnimation] = None,
-            draw_style: Optional[Union[str, DRAW_STYLE]] = None,
-            label: Optional[str] = None,
-            line_style: Optional[Union[str, LINE_STYLE]] = None,
-            line_width: Optional[FloatOrFloatAnimation] = None,
-            marker: Optional[Union[str, MARKER_STYLE]] = None,
-            marker_edge_color: Optional[ColorOrColorAnimation] = None,
-            marker_edge_width: Optional[FloatOrFloatAnimation] = None,
-            marker_face_color: Optional[ColorOrColorAnimation] = None,
-            marker_face_color_alt: Optional[ColorOrColorAnimation] = None,
-            marker_size: Optional[FloatOrFloatAnimation] = None
-    ):
-        if smooth is not False:
-            if smooth is True:
-                smooth = 1000
-            f_smooth = interp1d(x, y, kind=smooth_order)
-            x_smooth = linspace(min(x), max(x), smooth)
-            y_smooth = f_smooth(x_smooth)
-            x = x_smooth
-            y = y_smooth
-        self.x: FloatIterable = x
-        self.y: FloatIterable = y
-        self.length: Optional[FloatAnimation] = self._float_anim(length)
-        self.alpha: FloatOrFloatAnimation = self._float_anim(alpha)
-        self.color: Optional[ColorOrColorAnimation] = color
-        self.draw_style: Optional[Union[str, DRAW_STYLE]] = draw_style
-        self.label: Optional[str] = label
-        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
-        self.line_width: Optional[FloatOrFloatAnimation] = line_width
-        self.marker: Optional[Union[str, MARKER_STYLE]] = marker
-        self.marker_edge_color: Optional[ColorOrColorAnimation] = \
-            marker_edge_color
-        self.marker_edge_width: Optional[FloatOrFloatAnimation] = \
-            marker_edge_width
-        self.marker_face_color: Optional[ColorOrColorAnimation] = \
-            marker_face_color
-        self.marker_face_color_alt: Optional[ColorOrColorAnimation] = \
-            marker_face_color_alt
-        self.marker_size: Optional[FloatOrFloatAnimation] = marker_size
-
-    def draw(self, t: float, axes: AxesFormatter):
-
-        kwargs = {}
-
-        if self.length is not None:
-            kwargs['x'] = self.x[: int(round(self.length.at(t) * len(self.x)))]
-            kwargs['y'] = self.y[: int(round(self.length.at(t) * len(self.y)))]
-        else:
-            kwargs['x'] = self.x
-            kwargs['y'] = self.y
-        for float_kwarg in ('alpha', 'line_width',
-                            'marker_edge_width', 'marker_size'):
-            self._add_float_kwarg(float_kwarg, kwargs, t)
-        for color_kwarg in ('color', 'marker_edge_color',
-                            'marker_face_color', 'marker_face_color_alt'):
-            self._add_color_kwarg(color_kwarg, kwargs, t)
-        for kwarg in ('draw_style', 'label', 'line_style', 'marker'):
-            self._add_non_animated_kwarg(kwarg, kwargs)
-
-        axes.add_line(**kwargs)
+from typing import Union, Optional
+
+from numpy import linspace
+from scipy.interpolate import interp1d
+
+from mpl_format.compound_types import FloatIterable
+from mpl_format.animation.kwarg_animations.float_animation import FloatAnimation
+from mpl_format.animation.shapes.base import ShapeAnimation
+from mpl_format.animation.type_animations import \
+    FloatOrFloatAnimation, ColorOrColorAnimation, StrOrFloatAnimation, \
+    StrOrFloatOrFloatAnimation
+from mpl_format.axes import AxesFormatter
+from mpl_format.enums.marker_style import MARKER_STYLE
+from mpl_format.enums.draw_style import DRAW_STYLE
+from mpl_format.enums.line_style import LINE_STYLE
+
+
+class LineAnimation(ShapeAnimation, object):
+
+    def __init__(
+            self,
+            x: FloatIterable,
+            y: FloatIterable,
+            smooth: Union[bool, int] = False,
+            smooth_order: int = 2,
+            length: Optional[StrOrFloatAnimation] = None,
+            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
+            color: Optional[ColorOrColorAnimation] = None,
+            draw_style: Optional[Union[str, DRAW_STYLE]] = None,
+            label: Optional[str] = None,
+            line_style: Optional[Union[str, LINE_STYLE]] = None,
+            line_width: Optional[FloatOrFloatAnimation] = None,
+            marker: Optional[Union[str, MARKER_STYLE]] = None,
+            marker_edge_color: Optional[ColorOrColorAnimation] = None,
+            marker_edge_width: Optional[FloatOrFloatAnimation] = None,
+            marker_face_color: Optional[ColorOrColorAnimation] = None,
+            marker_face_color_alt: Optional[ColorOrColorAnimation] = None,
+            marker_size: Optional[FloatOrFloatAnimation] = None
+    ):
+        if smooth is not False:
+            if smooth is True:
+                smooth = 1000
+            f_smooth = interp1d(x, y, kind=smooth_order)
+            x_smooth = linspace(min(x), max(x), smooth)
+            y_smooth = f_smooth(x_smooth)
+            x = x_smooth
+            y = y_smooth
+        self.x: FloatIterable = x
+        self.y: FloatIterable = y
+        self.length: Optional[FloatAnimation] = self._float_anim(length)
+        self.alpha: FloatOrFloatAnimation = self._float_anim(alpha)
+        self.color: Optional[ColorOrColorAnimation] = color
+        self.draw_style: Optional[Union[str, DRAW_STYLE]] = draw_style
+        self.label: Optional[str] = label
+        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
+        self.line_width: Optional[FloatOrFloatAnimation] = line_width
+        self.marker: Optional[Union[str, MARKER_STYLE]] = marker
+        self.marker_edge_color: Optional[ColorOrColorAnimation] = \
+            marker_edge_color
+        self.marker_edge_width: Optional[FloatOrFloatAnimation] = \
+            marker_edge_width
+        self.marker_face_color: Optional[ColorOrColorAnimation] = \
+            marker_face_color
+        self.marker_face_color_alt: Optional[ColorOrColorAnimation] = \
+            marker_face_color_alt
+        self.marker_size: Optional[FloatOrFloatAnimation] = marker_size
+
+    def draw(self, t: float, axes: AxesFormatter):
+
+        kwargs = {}
+
+        if self.length is not None:
+            kwargs['x'] = self.x[: int(round(self.length.at(t) * len(self.x)))]
+            kwargs['y'] = self.y[: int(round(self.length.at(t) * len(self.y)))]
+        else:
+            kwargs['x'] = self.x
+            kwargs['y'] = self.y
+        for float_kwarg in ('alpha', 'line_width',
+                            'marker_edge_width', 'marker_size'):
+            self._add_float_kwarg(float_kwarg, kwargs, t)
+        for color_kwarg in ('color', 'marker_edge_color',
+                            'marker_face_color', 'marker_face_color_alt'):
+            self._add_color_kwarg(color_kwarg, kwargs, t)
+        for kwarg in ('draw_style', 'label', 'line_style', 'marker'):
+            self._add_non_animated_kwarg(kwarg, kwargs)
+
+        axes.add_line(**kwargs)
```

### Comparing `mpl_format-0.317/mpl_format/animation/shapes/regular_polygon_animation.py` & `mpl_format-0.318/mpl_format/animation/shapes/ellipse_animation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-from typing import Optional, Union
-
-from mpl_format.animation.shapes.base import ShapeAnimation
-from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
-    StrOrFloatOrFloatAnimation, ColorOrColorAnimation
-from mpl_format.axes import AxesFormatter
-from mpl_format.enums.join_style import JOIN_STYLE
-from mpl_format.enums.cap_style import CAP_STYLE
-from mpl_format.enums.line_style import LINE_STYLE
-
-
-class RegularPolygonAnimation(ShapeAnimation, object):
-
-    def __init__(
-            self,
-            x_center: FloatOrFloatAnimation,
-            y_center: FloatOrFloatAnimation,
-            num_vertices: int,
-            radius: FloatOrFloatAnimation,
-            angle: FloatOrFloatAnimation = 0,
-            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
-            color: Optional[ColorOrColorAnimation] = None,
-            edge_color: Optional[ColorOrColorAnimation] = None,
-            face_color: Optional[ColorOrColorAnimation] = None,
-            fill: bool = True,
-            label: Optional[str] = None,
-            line_style: Optional[Union[str, LINE_STYLE]] = None,
-            line_width: Optional[FloatOrFloatAnimation] = None,
-            cap_style: Optional[Union[str, CAP_STYLE]] = None,
-            join_style: Optional[Union[str, JOIN_STYLE]] = None,
-    ):
-        self.x_center: FloatOrFloatAnimation = x_center
-        self.y_center: FloatOrFloatAnimation = y_center
-        self.num_vertices: int = num_vertices
-        self.radius: FloatOrFloatAnimation = radius
-        self.angle: FloatOrFloatAnimation = angle
-        self.alpha: Optional[FloatOrFloatAnimation] = self._float_anim(alpha)
-        self.color: Optional[ColorOrColorAnimation] = color
-        self.edge_color: Optional[ColorOrColorAnimation] = edge_color
-        self.face_color: Optional[ColorOrColorAnimation] = face_color
-        self.fill: bool = fill
-        self.label: Optional[str] = label
-        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
-        self.line_width: Optional[FloatOrFloatAnimation] = line_width
-        self.cap_style: Optional[Union[str, CAP_STYLE]] = cap_style
-        self.join_style: Optional[Union[str, JOIN_STYLE]] = join_style
-
-    def draw(self, t: float, axes: AxesFormatter):
-
-        kwargs = {}
-        for float_kwarg in ('x_center', 'y_center', 'radius',
-                            'angle', 'alpha', 'line_width'):
-            self._add_float_kwarg(float_kwarg, kwargs, t)
-        for color_kwarg in ('color', 'edge_color', 'face_color'):
-            self._add_color_kwarg(color_kwarg, kwargs, t)
-        for kwarg in ('num_vertices', 'fill', 'label',
-                      'line_style', 'cap_style', 'join_style'):
-            self._add_non_animated_kwarg(kwarg, kwargs)
-
-        axes.add_regular_polygon(**kwargs)
+from typing import Optional, Union
+
+from mpl_format.animation.shapes.base import ShapeAnimation
+from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
+    StrOrFloatOrFloatAnimation, ColorOrColorAnimation
+from mpl_format.axes import AxesFormatter
+from mpl_format.enums.join_style import JOIN_STYLE
+from mpl_format.enums.cap_style import CAP_STYLE
+from mpl_format.enums.line_style import LINE_STYLE
+
+
+class EllipseAnimation(ShapeAnimation, object):
+
+    def __init__(
+            self,
+            x_center: FloatOrFloatAnimation,
+            y_center: FloatOrFloatAnimation,
+            width: FloatOrFloatAnimation,
+            height: FloatOrFloatAnimation,
+            angle: FloatOrFloatAnimation = 0.0,
+            alpha: Optional[StrOrFloatOrFloatAnimation] = None,
+            cap_style: Optional[Union[str, CAP_STYLE]] = None,
+            color: Optional[ColorOrColorAnimation] = None,
+            edge_color: Optional[ColorOrColorAnimation] = None,
+            face_color: Optional[ColorOrColorAnimation] = None,
+            fill: bool = True,
+            join_style: Optional[Union[str, JOIN_STYLE]] = None,
+            label: Optional[str] = None,
+            line_style: Optional[Union[str, LINE_STYLE]] = None,
+            line_width: Optional[FloatOrFloatAnimation] = None,
+    ):
+        self.x_center: FloatOrFloatAnimation = x_center
+        self.y_center: FloatOrFloatAnimation = y_center
+        self.width: FloatOrFloatAnimation = width
+        self.height: FloatOrFloatAnimation = height
+        self.angle: FloatOrFloatAnimation = angle
+        self.alpha: Optional[StrOrFloatOrFloatAnimation] = alpha
+        self.cap_style: Optional[Union[str, CAP_STYLE]] = cap_style
+        self.color: Optional[ColorOrColorAnimation] = color
+        self.edge_color: Optional[ColorOrColorAnimation] = edge_color
+        self.face_color: Optional[ColorOrColorAnimation] = face_color
+        self.fill: bool = fill
+        self.join_style: Optional[Union[str, JOIN_STYLE]] = join_style
+        self.label: Optional[str] = label
+        self.line_style: Optional[Union[str, LINE_STYLE]] = line_style
+        self.line_width: Optional[FloatOrFloatAnimation] = line_width
+
+    def draw(self, t: float, axes: AxesFormatter):
+
+        kwargs = {}
+        for float_kwarg in (
+                'x_center', 'y_center',
+                'width', 'height', 'angle',
+                'alpha', 'line_width'
+        ):
+            self._add_float_kwarg(float_kwarg, kwargs, t)
+        for color_kwarg in ('color', 'edge_color', 'face_color'):
+            self._add_color_kwarg(color_kwarg, kwargs, t)
+        for kwarg in ('cap_style', 'fill', 'join_style',
+                      'label', 'line_style'):
+            self._add_non_animated_kwarg(kwarg, kwargs)
+
+        axes.add_ellipse(**kwargs)
```

### Comparing `mpl_format-0.317/mpl_format/animation/shapes/text_animation.py` & `mpl_format-0.318/mpl_format/animation/shapes/text_animation.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-from typing import Optional, Union
-
-from mpl_format.animation.kwarg_animations import FloatAnimation
-from mpl_format.animation.shapes.base import ShapeAnimation
-from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
-    StrOrFloatAnimation, ColorOrColorAnimation
-from mpl_format.compound_types import Color
-from mpl_format.enums import FONT_SIZE, FONT_STRETCH, FONT_STYLE, \
-    FONT_VARIANT, FONT_WEIGHT, CAP_STYLE, JOIN_STYLE, LINE_STYLE
-
-
-class TextAnimation(ShapeAnimation, object):
-
-    def __init__(
-            self, x: FloatOrFloatAnimation,
-            y: FloatOrFloatAnimation,
-            text: str,
-            length: Optional[StrOrFloatAnimation] = None,
-            font_dict: Optional[dict] = None,
-            alpha: Optional[float] = None,
-            color: Optional[ColorOrColorAnimation] = None,
-            h_align: Optional[str] = None,
-            v_align: Optional[str] = None,
-            m_align: Optional[str] = None,
-            line_spacing: Optional[float] = None,
-            font_family: Optional[str] = None,
-            font_size: Optional[Union[int, float, str, FONT_SIZE]] = None,
-            font_stretch: Optional[Union[int, float, FONT_STRETCH]] = None,
-            font_style: Optional[Union[str, FONT_STYLE]] = None,
-            font_variant: Optional[Union[str, FONT_VARIANT]] = None,
-            font_weight: Optional[Union[int, float, str, FONT_WEIGHT]] = None,
-            wrap: Optional[bool] = None,
-            bbox_style: Optional[str] = None,
-            bbox_alpha: Optional[float] = None,
-            bbox_cap_style: Optional[Union[str, CAP_STYLE]] = None,
-            bbox_color: Optional[Color] = None,
-            bbox_edge_color: Optional[Color] = None,
-            bbox_face_color: Optional[Color] = None,
-            bbox_fill: Optional[bool] = None,
-            bbox_join_style: Optional[Union[str, JOIN_STYLE]] = None,
-            bbox_line_style: Optional[Union[str, LINE_STYLE]] = None,
-            bbox_line_width: Optional[float] = None
-    ):
-        self.x: FloatOrFloatAnimation = x
-        self.y: FloatOrFloatAnimation = y
-        self.text: str = text
-        self.length: Optional[FloatAnimation] = self._float_anim(length)
-        self.font_dict: Optional[dict] = font_dict
-        self.alpha: FloatOrFloatAnimation = self._float_anim(alpha)
-        self.color: Optional[ColorOrColorAnimation] = color
-        self.h_align: Optional[str] = h_align
-        self.v_align: Optional[str] = v_align
-        self.m_align: Optional[str] = m_align
-        self.line_spacing: Optional[float] = line_spacing
-        self.font_family: Optional[str] = font_family
-        self.font_size: Optional[Union[int, float, str, FONT_SIZE]] = font_size
-        self.font_stretch: Optional[
-            Union[int, float, FONT_STRETCH]] = font_stretch
-        self.font_style: Optional[Union[str, FONT_STYLE]] = font_style
-        self.font_variant: Optional[Union[str, FONT_VARIANT]] = font_variant
-        self.font_weight: Optional[
-            Union[int, float, str, FONT_WEIGHT]] = font_weight
-        self.wrap: Optional[bool] = wrap
-        self.bbox_style: Optional[str] = bbox_style
-        self.bbox_alpha: Optional[float] = bbox_alpha
-        self.bbox_cap_style: Optional[Union[str, CAP_STYLE]] = bbox_cap_style
-        self.bbox_color: Optional[Color] = bbox_color
-        self.bbox_edge_color: Optional[Color] = bbox_edge_color
-        self.bbox_face_color: Optional[Color] = bbox_face_color
-        self.bbox_fill: Optional[bool] = bbox_fill
-        self.bbox_join_style: Optional[Union[str, JOIN_STYLE]] = bbox_join_style
-        self.bbox_line_style: Optional[Union[str, LINE_STYLE]] = bbox_line_style
-        self.bbox_line_width: Optional[float] = bbox_line_width
-
-    # def draw(self, t: float, axes: AxesFormatter):
-    #
-    #     kwargs = {}
-    #
-    #     if self.length is not None:
-    #         num_chars = int(len(self.text) * self.length.at(t))
-    #         kwargs['text'] = self.text[: num_chars]
-    #     else:
-    #         kwargs['text'] = self.text
-    #
-    #     for float_kwarg in ('x', 'y', '')
+from typing import Optional, Union
+
+from mpl_format.animation.kwarg_animations import FloatAnimation
+from mpl_format.animation.shapes.base import ShapeAnimation
+from mpl_format.animation.type_animations import FloatOrFloatAnimation, \
+    StrOrFloatAnimation, ColorOrColorAnimation
+from mpl_format.compound_types import Color
+from mpl_format.enums import FONT_SIZE, FONT_STRETCH, FONT_STYLE, \
+    FONT_VARIANT, FONT_WEIGHT, CAP_STYLE, JOIN_STYLE, LINE_STYLE
+
+
+class TextAnimation(ShapeAnimation, object):
+
+    def __init__(
+            self, x: FloatOrFloatAnimation,
+            y: FloatOrFloatAnimation,
+            text: str,
+            length: Optional[StrOrFloatAnimation] = None,
+            font_dict: Optional[dict] = None,
+            alpha: Optional[float] = None,
+            color: Optional[ColorOrColorAnimation] = None,
+            h_align: Optional[str] = None,
+            v_align: Optional[str] = None,
+            m_align: Optional[str] = None,
+            line_spacing: Optional[float] = None,
+            font_family: Optional[str] = None,
+            font_size: Optional[Union[int, float, str, FONT_SIZE]] = None,
+            font_stretch: Optional[Union[int, float, FONT_STRETCH]] = None,
+            font_style: Optional[Union[str, FONT_STYLE]] = None,
+            font_variant: Optional[Union[str, FONT_VARIANT]] = None,
+            font_weight: Optional[Union[int, float, str, FONT_WEIGHT]] = None,
+            wrap: Optional[bool] = None,
+            bbox_style: Optional[str] = None,
+            bbox_alpha: Optional[float] = None,
+            bbox_cap_style: Optional[Union[str, CAP_STYLE]] = None,
+            bbox_color: Optional[Color] = None,
+            bbox_edge_color: Optional[Color] = None,
+            bbox_face_color: Optional[Color] = None,
+            bbox_fill: Optional[bool] = None,
+            bbox_join_style: Optional[Union[str, JOIN_STYLE]] = None,
+            bbox_line_style: Optional[Union[str, LINE_STYLE]] = None,
+            bbox_line_width: Optional[float] = None
+    ):
+        self.x: FloatOrFloatAnimation = x
+        self.y: FloatOrFloatAnimation = y
+        self.text: str = text
+        self.length: Optional[FloatAnimation] = self._float_anim(length)
+        self.font_dict: Optional[dict] = font_dict
+        self.alpha: FloatOrFloatAnimation = self._float_anim(alpha)
+        self.color: Optional[ColorOrColorAnimation] = color
+        self.h_align: Optional[str] = h_align
+        self.v_align: Optional[str] = v_align
+        self.m_align: Optional[str] = m_align
+        self.line_spacing: Optional[float] = line_spacing
+        self.font_family: Optional[str] = font_family
+        self.font_size: Optional[Union[int, float, str, FONT_SIZE]] = font_size
+        self.font_stretch: Optional[
+            Union[int, float, FONT_STRETCH]] = font_stretch
+        self.font_style: Optional[Union[str, FONT_STYLE]] = font_style
+        self.font_variant: Optional[Union[str, FONT_VARIANT]] = font_variant
+        self.font_weight: Optional[
+            Union[int, float, str, FONT_WEIGHT]] = font_weight
+        self.wrap: Optional[bool] = wrap
+        self.bbox_style: Optional[str] = bbox_style
+        self.bbox_alpha: Optional[float] = bbox_alpha
+        self.bbox_cap_style: Optional[Union[str, CAP_STYLE]] = bbox_cap_style
+        self.bbox_color: Optional[Color] = bbox_color
+        self.bbox_edge_color: Optional[Color] = bbox_edge_color
+        self.bbox_face_color: Optional[Color] = bbox_face_color
+        self.bbox_fill: Optional[bool] = bbox_fill
+        self.bbox_join_style: Optional[Union[str, JOIN_STYLE]] = bbox_join_style
+        self.bbox_line_style: Optional[Union[str, LINE_STYLE]] = bbox_line_style
+        self.bbox_line_width: Optional[float] = bbox_line_width
+
+    # def draw(self, t: float, axes: AxesFormatter):
+    #
+    #     kwargs = {}
+    #
+    #     if self.length is not None:
+    #         num_chars = int(len(self.text) * self.length.at(t))
+    #         kwargs['text'] = self.text[: num_chars]
+    #     else:
+    #         kwargs['text'] = self.text
+    #
+    #     for float_kwarg in ('x', 'y', '')
```

### Comparing `mpl_format-0.317/mpl_format/axes/axes_formatter.py` & `mpl_format-0.318/mpl_format/axes/axes_formatter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,2766 +1,2771 @@
-from datetime import date
-from math import pi, atan2
-from typing import Optional, Union, List, Tuple, Iterable, TYPE_CHECKING, \
-    Callable
-
-import matplotlib.pyplot as plt
-from mpl_format.compound_types import ArrayLike
-from mpl_format.compound_types import FloatOrFloatIterable, StrOrStrIterable, \
-    DictOrDictIterable, BoolOrBoolIterable, FloatIterable, Scalar, \
-    IntOrIntIterable, NdArrayIterable
-from mpl_format.utils.type_checks import all_are_none, one_is_not_none
-from matplotlib.axes import Axes
-from matplotlib.collections import PathCollection
-from matplotlib.figure import Figure
-from matplotlib.font_manager import FontProperties
-from matplotlib.patches import \
-    Arc, Arrow, BoxStyle, Circle, Ellipse, \
-    FancyArrow, FancyArrowPatch, FancyBboxPatch, \
-    Patch, Polygon, Rectangle, RegularPolygon, Wedge
-from matplotlib.path import Path
-
-from mpl_format.enums.font_size import FONT_SIZE
-from numpy import ndarray, linspace
-from numpy.ma import cos, sin
-from pandas import DataFrame, Series
-from scipy.interpolate import interp1d
-
-from mpl_format.axes.axis_formatter import AxisFormatter
-from mpl_format.axes.axis_utils import new_axes
-from mpl_format.axes.ticks_formatter import TicksFormatter
-from mpl_format.compound_types import FontSize, Color, LegendLocation, \
-    StringMapper, ColorOrColorIterable, FontStretch, FontWeight, \
-    FontSizeIterable, FontStretchIterable, FontStyle, FontStyleIterable, \
-    FontVariant, FontVariantIterable, CapStyle, CapStyleIterable, \
-    JoinStyleIterable, JoinStyle, LineStyleIterable, LineStyle, \
-    ArrowStyleIterable, ArrowStyle, ConnectionStyleIterable, ConnectionStyle, \
-    PathIterable, PatchIterable, BoxStyleTypeIterable
-from mpl_format.enums.box_style import BOX_STYLE, BoxStyleType
-from mpl_format.enums.cap_style import CAP_STYLE
-from mpl_format.enums.connection_style import CONNECTION_STYLE
-from mpl_format.enums.draw_style import DRAW_STYLE
-from mpl_format.enums.font_weight import FONT_WEIGHT
-from mpl_format.enums.line_style import LINE_STYLE
-from mpl_format.enums.mappings import kwarg_mappings
-from mpl_format.enums.marker_style import MARKER_STYLE
-from mpl_format.legend.legend_formatter import LegendFormatter
-from mpl_format.literals import H_ALIGN, V_ALIGN, ROTATION_MODE, WHICH_TICKS, \
-    FIGURE_UNITS, WHICH_AXIS, LINE_STYLE_STR, ASPECT, ANCHOR
-from mpl_format.patches.patch_list_formatter import PatchListFormatter
-from mpl_format.text.text_formatter import TextFormatter
-from mpl_format.text.text_utils import wrap_text
-from mpl_format.utils.arg_checks import check_h_align, check_v_align
-from mpl_format.utils.arg_transforms import smart_zip_kwargs, \
-    drop_none_values, apply_mappings
-from mpl_format.utils.color_utils import cross_fade
-from mpl_format.utils.io_utils import save_plot
-
-if TYPE_CHECKING:
-    from mpl_format.figures.figure_formatter import FigureFormatter
-
-
-class AxesFormatter(object):
-
-    def __init__(self, axes: Optional[Axes] = None,
-                 width: Optional[Scalar] = None,
-                 height: Optional[Scalar] = None,
-                 constrained_layout: bool = False):
-        """
-        Create a new AxesFormatter
-
-        :param axes: The matplotlib Axes instance to wrap.
-        :param width: Width of new Axes, if none are given.
-        :param height: Height of new Axes, if none are given.
-        :param constrained_layout: Option for constrained_layout of new Axes.
-        """
-        if axes is None:
-            self._axes: Axes = new_axes(
-                width=width, height=height,
-                constrained_layout=constrained_layout
-            )
-        else:
-            self._axes: Axes = axes
-        self._x_axis: AxisFormatter = AxisFormatter(
-            axis=self._axes.xaxis, direction='x', axes=self._axes
-        )
-        self._y_axis: AxisFormatter = AxisFormatter(
-            axis=self._axes.yaxis, direction='y', axes=self._axes
-        )
-        self._title: TextFormatter = TextFormatter(self._axes.title)
-        legend = self._axes.get_legend()
-        if legend is None:
-            self._legend = None
-        else:
-            self._legend = LegendFormatter(legend)
-        self._ticks: TicksFormatter = TicksFormatter(
-            axis='both', which='both', axes=self._axes)
-        self._major_ticks: TicksFormatter = TicksFormatter(
-            axis='both', which='major', axes=self._axes)
-        self._minor_ticks: TicksFormatter = TicksFormatter(
-            axis='both', which='minor', axes=self._axes)
-        self._x_ticks: TicksFormatter = TicksFormatter(
-            axis='x', which='both', axes=self._axes)
-        self._x_major_ticks: TicksFormatter = TicksFormatter(
-            axis='x', which='major', axes=self._axes)
-        self._x_minor_ticks: TicksFormatter = TicksFormatter(
-            axis='x', which='minor', axes=self._axes)
-        self._y_ticks: TicksFormatter = TicksFormatter(
-            axis='y', which='both', axes=self._axes)
-        self._y_major_ticks: TicksFormatter = TicksFormatter(
-            axis='y', which='major', axes=self._axes)
-        self._y_minor_ticks = TicksFormatter(
-            axis='y', which='minor', axes=self._axes)
-
-    @staticmethod
-    def gca() -> 'AxesFormatter':
-
-        return AxesFormatter(axes=plt.gca())
-
-    @staticmethod
-    def find_in_figure(
-            figure: Figure,
-            match: Callable[['AxesFormatter'], bool]
-    ):
-        """
-        Return and AxesFormatter matching the first Axes in the instance where
-        an AxesFormatter wrapping the Axes matches the lambda function.
-
-        :param figure: Figure e.g. plt.gcf()
-        :param match: Method that return True for the matching Axes.
-        """
-        for axes in figure.axes:
-            axf = AxesFormatter(axes)
-            if match(axf):
-                return axf
-        raise ValueError('No matching Axes')
-
-    # region properties
-
-    @property
-    def axes(self) -> Axes:
-        """
-        Return the wrapped Axes instance.
-        """
-        return self._axes
-
-    @property
-    def x_axis(self) -> AxisFormatter:
-        """
-        Return an AxisFormatter for the x-axis of the wrapped Axes.
-        """
-        return self._x_axis
-
-    @property
-    def y_axis(self) -> AxisFormatter:
-        """
-        Return an AxisFormatter for the y-axis of the wrapped Axes.
-        """
-        return self._y_axis
-
-    @property
-    def legend(self) -> LegendFormatter:
-        """
-        Return a LegendFormatter for the legend of the wrapped Axes,
-        if there is one.
-        """
-        return self._legend
-
-    @property
-    def title(self) -> TextFormatter:
-        return self._title
-
-    @property
-    def figure(self) -> 'FigureFormatter':
-
-        from mpl_format.figures.figure_formatter import FigureFormatter
-        return FigureFormatter(self._axes)
-
-    @property
-    def ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the ticks on both axes.
-        """
-        return self._ticks
-    
-    @property
-    def x_ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the ticks on the x-axis.
-        """
-        return self._x_ticks
-
-    @property
-    def y_ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the ticks on the y-axis.
-        """
-        return self._y_ticks
-
-    @property
-    def major_ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the major ticks on both axes.
-        """
-        return self._major_ticks
-
-    @property
-    def x_major_ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the major ticks on the x-axis.
-        """
-        return self._x_major_ticks
-
-    @property
-    def y_major_ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the major ticks on the y-axis.
-        """
-        return self._y_major_ticks
-
-    @property
-    def minor_ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the minor ticks on both axes.
-        """
-        return self._minor_ticks
-
-    @property
-    def x_minor_ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the minor ticks on the x-axis.
-        """
-        return self._x_minor_ticks
-
-    @property
-    def y_minor_ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the minor ticks on the y-axis.
-        """
-        return self._y_minor_ticks
-    
-    # endregion
-
-    # region set text
-
-    def set_title_text(self, text: str) -> 'AxesFormatter':
-        """
-        Set the text of the Axes title.
-
-        :param text: The text to use for the Axes title.
-        """
-        self.title.set_text(text)
-        return self
-
-    def map_title_text(
-            self, mapping: StringMapper
-    ) -> 'AxesFormatter':
-        """
-        Map the label text for the title using a dictionary or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        self.title.map(mapping=mapping)
-        return self
-
-    def get_x_label_text(self) -> str:
-
-        return self.x_axis.get_label_text()
-
-    def set_x_label_text(self, text: str) -> 'AxesFormatter':
-        """
-        Set the text for the x-axis label.
-
-        :param text: The text to use for the Axis label.
-        """
-        self.x_axis.set_label_text(text)
-        return self
-
-    def get_y_label_text(self) -> str:
-
-        return self.y_axis.get_label_text()
-
-    def set_y_label_text(self, text: str) -> 'AxesFormatter':
-        """
-        Set the text for the y-axis label.
-
-        :param text: The text to use for the Axis label.
-        """
-        self.y_axis.set_label_text(text)
-        return self
-
-    def set_text(self, title: Optional[str] = None,
-                 x_label: Optional[str] = None,
-                 y_label: Optional[str] = None) -> 'AxesFormatter':
-        """
-        Set text properties for elements of the Axes.
-
-        :param title: Text for the title.
-        :param x_label: Text for the x-axis label.
-        :param y_label: Text for the y-axis label.
-        """
-        if title is not None:
-            self.set_title_text(title)
-        if x_label is not None:
-            self.x_axis.set_label_text(x_label)
-        if y_label is not None:
-            self.y_axis.set_label_text(y_label)
-        return self
-
-    # endregion
-
-    # region wrap text
-
-    def wrap_title(self, max_width: int) -> 'AxesFormatter':
-        """
-        Wrap the text for the title if it exceeds a given width of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        self.set_title_text(wrap_text(self.title.text, max_width=max_width))
-        return self
-
-    def wrap_x_label(self, max_width: int) -> 'AxesFormatter':
-        """
-        Wrap the text for the x-axis label if it exceeds a given width of
-        characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        self.x_axis.wrap_label(max_width=max_width)
-        return self
-
-    def wrap_y_label(self, max_width: int) -> 'AxesFormatter':
-        """
-        Wrap the text for the y-axis label if it exceeds a given width of
-        characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        self.y_axis.wrap_label(max_width=max_width)
-        return self
-
-    def wrap_axis_labels(self, max_width: int) -> 'AxesFormatter':
-        """
-        Wrap the texts for the x and y-axis labels if they exceeds a given width
-        of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        self.wrap_x_label(max_width=max_width)
-        self.wrap_y_label(max_width=max_width)
-        return self
-
-    # endregion
-
-    # region set font sizes
-
-    def _get_font_size(self, font_size: FontSize):
-
-        if isinstance(font_size, FONT_SIZE):
-            return font_size.get_name()
-        else:
-            return font_size
-
-    def set_title_size(self, font_size: FontSize) -> 'AxesFormatter':
-        """
-        Set the font size for the title of the wrapped Axes.
-
-        :param font_size: Size of the font in points, or size name.
-        """
-        self.title.set_size(self._get_font_size(font_size))
-        return self
-
-    def set_x_label_size(self, font_size: FontSize) -> 'AxesFormatter':
-        """
-        Set the font size for the x-axis label.
-
-        :param font_size: Size of the font in points, or size name.
-        """
-        self.x_axis.set_label_size(self._get_font_size(font_size))
-        return self
-
-    def set_y_label_size(self, font_size: FontSize) -> 'AxesFormatter':
-        """
-        Set the font size for the x-axis label.
-
-        :param font_size: Size of the font in points, or size name.
-        """
-        self.y_axis.set_label_size(self._get_font_size(font_size))
-        return self
-
-    def set_axis_label_sizes(self, font_size: FontSize) -> 'AxesFormatter':
-        """
-        Set the font size for the axis labels.
-
-        :param font_size: Size of the font in points, or size name.
-        """
-        self.set_x_label_size(font_size)
-        self.set_y_label_size(font_size)
-        return self
-
-    def set_font_sizes(
-            self,
-            title: Optional[FontSize] = None,
-            axis_labels: Optional[FontSize] = None,
-            tick_labels: Optional[FontSize] = None,
-            legend: Optional[FontSize] = None,
-            figure_title: Optional[FontSize] = None,
-            x_axis_label: Optional[FontSize] = None,
-            y_axis_label: Optional[FontSize] = None,
-            major_tick_labels: Optional[FontSize] = None,
-            minor_tick_labels: Optional[FontSize] = None,
-            x_tick_labels: Optional[FontSize] = None,
-            x_major_tick_labels: Optional[FontSize] = None,
-            x_minor_tick_labels: Optional[FontSize] = None,
-            y_tick_labels: Optional[FontSize] = None,
-            y_major_tick_labels: Optional[FontSize] = None,
-            y_minor_tick_labels: Optional[FontSize] = None,
-    ) -> 'AxesFormatter':
-        """
-        Set font sizes for different axes elements.
-        """
-        ax = self._axes
-        # title
-        if title is not None:
-            self.set_title_size(title)
-        # axis labels
-        if axis_labels is not None:
-            self.set_axis_label_sizes(axis_labels)
-        if x_axis_label is not None:
-            self.set_x_label_size(x_axis_label)
-        if y_axis_label is not None:
-            self.set_y_label_size(y_axis_label)
-        # tick labels
-        if tick_labels is not None:
-            self.ticks.set_label_size(tick_labels)
-        if major_tick_labels is not None:
-            self.major_ticks.set_label_size(major_tick_labels)
-        if minor_tick_labels is not None:
-            self.minor_ticks.set_label_size(minor_tick_labels)
-        if x_tick_labels is not None:
-            self.x_ticks.set_label_size(tick_labels)
-        if x_major_tick_labels is not None:
-            self.x_major_ticks.set_label_size(x_major_tick_labels)
-        if x_minor_tick_labels is not None:
-            self.x_minor_ticks.set_label_size(x_minor_tick_labels)
-        if y_tick_labels is not None:
-            self.y_ticks.set_label_size(tick_labels)
-        if y_major_tick_labels is not None:
-            self.y_major_ticks.set_label_size(y_major_tick_labels)
-        if y_minor_tick_labels is not None:
-            self.y_minor_ticks.set_label_size(y_major_tick_labels)
-        if legend is not None:
-            if isinstance(legend, FONT_SIZE):
-                legend = legend.get_name()
-            ax.legend(fontsize=legend)
-        if figure_title is not None:
-            if isinstance(figure_title, FONT_SIZE):
-                figure_title = figure_title.get_name()
-            ax.figure.suptitle(ax.get_title(), fontsize=figure_title)
-
-        return self
-
-    # endregion
-
-    # region map labels
-
-    def map_x_axis_label(
-            self, mapping: StringMapper
-    ) -> 'AxesFormatter':
-        """
-        Map the label text for the x-axis using a dictionary or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        self.x_axis.map_label_text(mapping)
-        return self
-
-    def map_y_axis_label(
-            self, mapping: StringMapper
-    ) -> 'AxesFormatter':
-        """
-        Map the label text for the y-axis using a dictionary or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        self.y_axis.map_label_text(mapping)
-        return self
-
-    def map_axis_labels(
-            self, mapping: StringMapper
-    ) -> 'AxesFormatter':
-        """
-        Map the label text for the x and y axes using a dictionary or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        self.map_x_axis_label(mapping)
-        self.map_y_axis_label(mapping)
-        return self
-
-    # endregion
-
-    # region remove
-
-    def remove_title(self) -> 'AxesFormatter':
-        """
-        Remove the title from the Axes.
-        """
-        self.set_title_text('')
-        return self
-
-    def remove_legend(self) -> 'AxesFormatter':
-        """
-        Remove the legend from the Axes.
-        """
-        legend = self._axes.get_legend()
-        if legend is not None:
-            legend.remove()
-            self._legend = None
-        return self
-
-    def remove_x_ticks(self) -> 'AxesFormatter':
-        """
-        Remove x-ticks from the Axes.
-        """
-        self._axes.set_xticks([])
-        return self
-
-    def remove_y_ticks(self) -> 'AxesFormatter':
-        """
-        Remove y-ticks from the Axes.
-        """
-        self._axes.set_yticks([])
-        return self
-
-    def remove_axes_ticks(self) -> 'AxesFormatter':
-        """
-        Remove x- and y- ticks from the Axes.
-        """
-        self.remove_x_ticks()
-        self.remove_y_ticks()
-        return self
-
-    def remove_x_label(self) -> 'AxesFormatter':
-        """
-        Remove the label from the x-axis.
-        """
-        self.x_axis.remove_label()
-        return self
-
-    def remove_y_label(self) -> 'AxesFormatter':
-        """
-        Remove the label from the y-axis.
-        """
-        self.y_axis.remove_label()
-        return self
-
-    def remove_axes_labels(self) -> 'AxesFormatter':
-        """
-        Remove the labels from the x- and y- axes.
-        """
-        self.remove_x_label()
-        self.remove_y_label()
-        return self
-
-    # endregion
-
-    # region rotation
-
-    def rotate_x_label(self,
-                       rotation: int,
-                       how: ROTATION_MODE = 'absolute') -> 'AxesFormatter':
-        """
-        Set the rotation of the x-axis label.
-
-        :param rotation: The rotation value to set in degrees.
-        :param how: 'absolute' or 'relative'
-        """
-        self.x_axis.rotate_label(rotation, how)
-        return self
-
-    def rotate_y_label(self,
-                       rotation: int,
-                       how: ROTATION_MODE = 'absolute') -> 'AxesFormatter':
-        """
-        Set the rotation of the x-axis label.
-
-        :param rotation: The rotation value to set in degrees.
-        :param how: 'absolute' or 'relative'
-        """
-        self.y_axis.rotate_label(rotation, how)
-        return self
-
-    # endregion
-
-    # region spans
-
-    def add_h_line(self, y: Union[float, str, date] = 0,
-                   x_min: Union[float, str] = 0,
-                   x_max: Union[float, str] = 1,
-                   color: Optional[Color] = None,
-                   alpha: Optional[float] = None,
-                   line_style: Optional[LineStyle] = None,
-                   line_width: Optional[float] = None,
-                   label: Optional[str] = None,
-                   marker_edge_color: Optional[Color] = None,
-                   marker_edge_width: Optional[Color] = None,
-                   marker_face_color: Optional[Color] = None,
-                   marker_size: Optional[float] = None) -> 'AxesFormatter':
-        """
-        Add a horizontal line to the plot.
-
-        :param y: y position in data coordinates of the horizontal line
-        :param x_min: Between 0 and 1, 0 being the far left of the plot,
-                      1 the far right of the plot
-        :param x_max: Between 0 and 1, 0 being the far left of the plot,
-                      1 the far right of the plot
-        :param color: Color of the line
-        :param alpha: Opacity of the line
-        :param line_style: One of {'-', '--', '-.', ':', ''}
-        :param line_width: Width of the line
-        :param label: Text for the label
-        :param marker_edge_color: Color for the edges of the line markers
-        :param marker_edge_width: Width for the edges of the line markers
-        :param marker_face_color: Color for the markers
-        :param marker_size: Size of the markers.
-        """
-        line_style = LINE_STYLE.get_line_style(line_style)
-        kwargs = {}
-        for arg, mpl_arg in zip(
-            [color, line_style, line_width,
-             marker_edge_color, marker_edge_width,
-             marker_face_color, marker_size,
-             alpha, label],
-            ['c', 'ls', 'lw', 'mec', 'mew', 'mfc', 'ms', 'alpha', 'label']
-        ):
-            if arg is not None:
-                kwargs[mpl_arg] = arg
-
-        self._axes.axhline(
-            y=y, xmin=x_min, xmax=x_max,
-            **kwargs
-        )
-        return self
-
-    def add_v_line(self, x: Union[float, str, date] = 0,
-                   y_min: Union[float, str] = 0,
-                   y_max: Union[float, str] = 1,
-                   color: Optional[Color] = None, alpha: Optional[float] = None,
-                   line_style: Optional[Union[
-                       LineStyle, LineStyleIterable]] = None,
-                   line_width: Optional[float] = None,
-                   label: Optional[str] = None,
-                   marker_edge_color: Optional[Color] = None,
-                   marker_edge_width: Optional[Color] = None,
-                   marker_face_color: Optional[Color] = None,
-                   marker_size: Optional[float] = None) -> 'AxesFormatter':
-        """
-        Add a vertical line to the plot.
-
-        :param x: x position in data coordinates of the vertical line
-        :param y_min: Should be between 0 and 1, with 0 being the bottom of the
-                      plot, and 1 the top of the plot
-        :param y_max: Should be between 0 and 1, with 0 being the bottom of the
-                      plot, and 1 the top of the plot
-        :param color: Color of the line
-        :param alpha: Opacity of the line
-        :param line_style: One of {'-', '--', '-.', ':', ''}
-        :param line_width: Width of the line
-        :param label: Text for the label
-        :param marker_edge_color: Color for the edges of the line markers
-        :param marker_edge_width: Width for the edges of the line markers
-        :param marker_face_color: Color for the markers
-        :param marker_size: Size of the markers.
-        """
-        line_style = LINE_STYLE.get_line_style(line_style)
-        kwargs = {}
-        for arg, mpl_arg in zip(
-            [color, line_style, line_width, marker_edge_color,
-             marker_edge_width, marker_face_color, marker_size,
-             alpha, label],
-            ['c', 'ls', 'lw', 'mec',
-             'mew', 'mfc', 'ms',
-             'alpha', 'label']
-        ):
-            if arg is not None:
-                kwargs[mpl_arg] = arg
-
-        self._axes.axvline(
-            x=x, ymin=y_min, ymax=y_max,
-            **kwargs
-        )
-        return self
-
-    def add_h_lines(self, y: FloatOrFloatIterable,
-                    x_min: FloatOrFloatIterable,
-                    x_max: FloatOrFloatIterable,
-                    colors='k',
-                    line_styles: LINE_STYLE_STR = 'solid',
-                    label: Optional[str] = '') -> 'AxesFormatter':
-        """
-        Plot horizontal lines at each y from x_min to x_max.
-
-        :param y: x-indexes where to plot the lines.
-        :param x_min: Beginning of each or all lines.
-        :param x_max: End of each or all lines.
-        :param colors: Line colors.
-        :param line_styles: One of {'solid', 'dashed', 'dashdot', 'dotted'}
-        :param label: Label.
-        """
-        self._axes.hlines(y=y, xmin=x_min, xmax=x_max,
-                          colors=colors, linestyles=line_styles,
-                          label=label)
-        return self
-
-    def add_v_lines(self, x: FloatOrFloatIterable,
-                    y_min: FloatOrFloatIterable,
-                    y_max: FloatOrFloatIterable,
-                    colors='k',
-                    line_styles: LINE_STYLE_STR = 'solid',
-                    label: Optional[str] = '') -> 'AxesFormatter':
-        """
-        Plot vertical lines at each x from y_min to y_max.
-
-        :param x: x-indexes where to plot the lines.
-        :param y_min: Beginning of each or all lines.
-        :param y_max: End of each or all lines.
-        :param colors: Line colors.
-        :param line_styles: One of {'solid', 'dashed', 'dashdot', 'dotted'}
-        :param label: Label.
-        """
-        self._axes.vlines(x=x, ymin=y_min, ymax=y_max,
-                          colors=colors, linestyles=line_styles,
-                          label=label)
-        return self
-
-    def fill_between(self, x: Union[ArrayLike, str],
-                     y1: Union[float, ArrayLike, str],
-                     y2: Union[float, ArrayLike, str],
-                     data: Optional[DataFrame] = None,
-                     where: Optional[ArrayLike] = None,
-                     interpolate: bool = False,
-                     step: Optional[str] = None,
-                     color: Optional[Color] = None,
-                     alpha: Optional[float] = None,
-                     line_style: Optional[LineStyle] = None,
-                     line_width: Optional[float] = None,
-                     edge_color: Optional[Color] = None,
-                     face_color: Optional[Color] = None) -> 'AxesFormatter':
-        """
-        Make filled polygons between two curves.
-
-        :param x: N-length array of, or name of column with the x data.
-        :param y1: N-length array, scalar, or name of column with the y1 data.
-        :param y2: N-length array, scalar, or name of column with the y2 data.
-        :param data: Optional DataFrame with x, y1 and y2 columns.
-        :param where: If None, default to fill between everywhere. If not None,
-                      it is an N-length numpy boolean array and the fill will
-                      only happen over the regions where where==True.
-        :param interpolate: If True, interpolate between the two lines to find
-                            the precise point of intersection. Otherwise, the
-                            start and end points of the filled region will only
-                            occur on explicit values in the x array.
-        :param step: One of {‘pre’, ‘post’, ‘mid’}. If not None, fill with step
-                     logic.
-        :param color: matplotlib color arg or sequence of rgba tuples
-        :param alpha: Opacity.
-        :param line_style: One of {'-', '--', '-.', ':', ''}
-        :param line_width: float or sequence of floats
-        :param edge_color: matplotlib color spec or sequence of specs
-        :param face_color: matplotlib color spec or sequence of specs
-        """
-        line_style = LINE_STYLE.get_line_style(line_style)
-        # get arrays from DataFrame
-        if data is not None:
-            if isinstance(x, str):
-                x = data[x]
-            if isinstance(y1, str):
-                y1 = data[y1]
-            if isinstance(y2, str):
-                y2 = data[y2]
-        # convert args to matplotlib names
-        kwargs = {}
-        for arg, mpl_arg in zip(
-            [color, alpha, line_style, line_width, edge_color, face_color],
-            ['color', 'alpha', 'line_style',
-             'line_width', 'edge_color', 'face_color']
-        ):
-            if arg is not None:
-                kwargs[mpl_arg] = arg
-        # call matplotlib method
-        self._axes.fill_between(
-            x=x, y1=y1, y2=y2,
-            where=where, interpolate=interpolate,
-            step=step,
-            **kwargs
-        )
-        return self
-
-    # endregion
-
-    # region colors
-
-    def set_face_color(self, color: Color) -> 'AxesFormatter':
-
-        self._axes.set_facecolor(color)
-        return self
-
-    def get_frame_color(self) -> Union[Color, List[Color]]:
-        """
-        Return the color of the frame if all edges are the same color,
-        otherwise a list of the top, bottom, left and right colors.
-        """
-        colors = self.get_frame_colors()
-        if len(set(colors)) == 1:
-            return colors[0]
-        else:
-            return self.get_frame_colors()
-
-    def set_frame_color(self, color: Color) -> 'AxesFormatter':
-
-        for pos in ['top', 'bottom', 'left', 'right']:
-            self._axes.spines[pos].set_edgecolor(color)
-        return self
-
-    def get_frame_colors(self) -> List[Color]:
-        """
-        Return the colors of the top, bottom, left and right edges of the Axes.
-        """
-        return [
-            self._axes.spines[pos].get_edgecolor()
-            for pos in ['top', 'bottom', 'left', 'right']
-        ]
-
-    # endregion
-
-    # region shapes
-
-    # region patches
-
-    def add_text(
-            self,
-            x: Union[FloatOrFloatIterable, date, Iterable[date]],
-            y: Union[FloatOrFloatIterable, date, Iterable[date]],
-            text: StrOrStrIterable,
-            max_width: Optional[IntOrIntIterable] = None,
-            font_dict: Optional[DictOrDictIterable] = None,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            h_align: Optional[StrOrStrIterable] = None,
-            v_align: Optional[StrOrStrIterable] = None,
-            m_align: Optional[StrOrStrIterable] = None,
-            rotation: Optional[
-                Union[IntOrIntIterable, StrOrStrIterable]] = None,
-            rotation_mode: Optional[StrOrStrIterable] = None,
-            line_spacing: Optional[FloatOrFloatIterable] = None,
-            font_family: Optional[StrOrStrIterable] = None,
-            font_size: Optional[Union[FontSize, FontSizeIterable]] = None,
-            font_stretch: Optional[
-                Union[FontStretch, FontStretchIterable]] = None,
-            font_style: Optional[Union[FontStyle, FontStyleIterable]] = None,
-            font_variant: Optional[
-                Union[FontVariant, FontVariantIterable]] = None,
-            font_weight: Optional[Union[FontWeight, FONT_WEIGHT]] = None,
-            wrap: Optional[BoolOrBoolIterable] = None,
-            bbox_style: Optional[StrOrStrIterable] = None,
-            bbox_alpha: Optional[FloatOrFloatIterable] = None,
-            bbox_cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            bbox_color: Optional[ColorOrColorIterable] = None,
-            bbox_edge_color: Optional[ColorOrColorIterable] = None,
-            bbox_face_color: Optional[ColorOrColorIterable] = None,
-            bbox_fill: Optional[BoolOrBoolIterable] = None,
-            bbox_join_style: Optional[
-                Union[JoinStyle, JoinStyleIterable]] = None,
-            bbox_line_style: Optional[
-                Union[LineStyle, LineStyleIterable]] = None,
-            bbox_line_width: Optional[FloatOrFloatIterable] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a single or multiple text blocks to the plot.
-
-        :param x: x-coordinate(s) of the text.
-        :param y: y-coordinate(s) of the text.
-        :param text: String or iterable of text strings to add.
-        :param max_width: Max number of characters to wrap lines at.
-        :param font_dict: A dictionary to override the default text properties.
-                          If font_dict is None, the defaults are determined by
-                          your rc parameters.
-        :param alpha: Text opacity.
-        :param color: Text color.
-        :param h_align: Horizontal alignment.
-        :param v_align: Vertical alignment.
-        :param m_align: Multi-line alignment.
-        :param rotation: float or {'vertical', 'horizontal'}
-        :param rotation_mode: {None, 'default', 'anchor'}
-        :param line_spacing:
-        :param font_family:
-        :param font_size: float or {'xx-small', 'x-small', 'small', 'medium',
-                                    'large', 'x-large', 'xx-large'}
-        :param font_stretch: {a numeric value in range 0-1000,
-                             'ultra-condensed', 'extra-condensed', 'condensed',
-                             'semi-condensed', 'normal', 'semi-expanded',
-                             'expanded', 'extra-expanded', 'ultra-expanded'}
-        :param font_style: {'normal', 'italic', 'oblique'}
-        :param font_variant: {'normal', 'small-caps'}
-        :param font_weight: {a numeric value in range 0-1000, 'ultralight',
-                             'light', 'normal', 'regular', 'book', 'medium',
-                             'roman', 'semibold', 'demibold', 'demi', 'bold',
-                             'heavy', 'extra bold', 'black'}
-        :param wrap: Set whether the text can be wrapped.
-        :param bbox_alpha: Opacity.
-        :param bbox_style: Box style.
-        :param bbox_cap_style: Cap style.
-        :param bbox_color: Use to set both the edge-color and the face-color.
-        :param bbox_edge_color: Edge color.
-        :param bbox_face_color: Face color.
-        :param bbox_fill: Whether to fill the rectangle.
-        :param bbox_join_style: Join style.
-        :param bbox_line_style: Line style for edge.
-        :param bbox_line_width: Line width for edge.
-        :param z_order: z-order for the text.
-        """
-        for kwargs in smart_zip_kwargs(
-                x=x, y=y, s=text,
-                fontdict=font_dict, max_width=max_width,
-                alpha=alpha, color=color,
-                ha=h_align, va=v_align, ma=m_align,
-                rotation=rotation, rotation_mode=rotation_mode,
-                linespacing=line_spacing,
-                fontfamily=font_family, fontsize=font_size,
-                fontstretch=font_stretch, fontstyle=font_style,
-                fontvariant=font_variant, fontweight=font_weight,
-                wrap=wrap, zorder=z_order,
-                bbox__boxstyle=bbox_style, bbox__alpha=bbox_alpha,
-                bbox__capstyle=bbox_cap_style, bbox__color=bbox_color,
-                bbox__edgecolor=bbox_edge_color,
-                bbox__facecolor=bbox_face_color,
-                bbox__fill=bbox_fill, bbox__joinstyle=bbox_join_style,
-                bbox__linestyle=bbox_line_style, bbox__linewidth=bbox_line_width
-        ):
-            # main kwargs
-            kwargs = drop_none_values(kwargs)
-            kwargs = apply_mappings(kwargs, kwarg_mappings)
-            # bbox kwargs
-            bbox_kwargs = {}
-            for kw, arg in kwargs.items():
-                if kw.startswith('bbox__'):
-                    bbox_kwargs[kw[6:]] = arg
-            kwargs = {kw: arg for kw, arg in kwargs.items()
-                      if not kw.startswith('bbox__')}
-            if bbox_kwargs:
-                bbox_kwargs = apply_mappings(bbox_kwargs, kwarg_mappings)
-                kwargs['bbox'] = bbox_kwargs
-            # max width
-            mw = kwargs.pop('max_width', None)
-            if mw is not None:
-                kwargs['s'] = wrap_text(text=kwargs['s'], max_width=mw)
-            # add text
-            self._axes.text(**drop_none_values(kwargs))
-
-        return self
-
-    def add_arc(
-            self,
-            x_center: FloatOrFloatIterable,
-            y_center: FloatOrFloatIterable,
-            width: FloatOrFloatIterable,
-            height: FloatOrFloatIterable,
-            angle: FloatOrFloatIterable = 0.0,
-            theta_start: FloatOrFloatIterable = 0.0,
-            theta_end: FloatOrFloatIterable = 360.0,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
-            label: Optional[StrOrStrIterable] = None,
-            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ):
-        """
-        Add an elliptical arc, i.e. a segment of an ellipse.
-
-        :param x_center: The x-coordinate of the center of the ellipse.
-        :param y_center: The y-coordinate of the center of the ellipse.
-        :param width: The length of the horizontal axis.
-        :param height: The length of the vertical axis.
-        :param angle: Rotation of the ellipse in degrees (counterclockwise).
-        :param theta_start: Starting angle of the arc in degrees.
-                            Relative to angle, e.g. if angle = 45 and
-                            theta_start = 90 the absolute starting angle is 135.
-        :param theta_end: Ending angle of the arc in degrees.
-        :param alpha: Opacity.
-        :param cap_style: Cap style.
-        :param color: Use to set both the edge-color and the face-color.
-        :param edge_color: Edge color.
-        :param join_style: Join style.
-        :param label: Label for the object in the legend.
-        :param line_style: Line style for edge.
-        :param line_width: Line width for edge.
-        :param z_order: z-order for the arc.
-        """
-        for kwargs in smart_zip_kwargs(
-            x_center=x_center, y_center=y_center,
-            width=width, height=height, angle=angle,
-            theta1=theta_start, theta2=theta_end,
-            alpha=alpha, capstyle=cap_style, color=color, edgecolor=edge_color,
-            joinstyle=join_style, label=label,
-            linestyle=line_style, linewidth=line_width, zorder=z_order
-        ):
-            kwargs = drop_none_values(kwargs)
-            kwargs['xy'] = kwargs.pop('x_center'), kwargs.pop('y_center')
-            arc = Arc(**kwargs)
-            self._axes.add_artist(arc)
-
-        return self
-
-    def add_arrow(
-            self,
-            x_tail: FloatOrFloatIterable,
-            y_tail: FloatOrFloatIterable,
-            x_head: Optional[FloatOrFloatIterable] = None,
-            y_head: Optional[FloatOrFloatIterable] = None,
-            dx: Optional[FloatOrFloatIterable] = None,
-            dy: Optional[FloatOrFloatIterable] = None,
-            width: Optional[FloatOrFloatIterable] = None,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
-            label: StrOrStrIterable = None,
-            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ):
-        """
-        Add an an arrow patch.
-
-        :param x_tail: The x-coordinate of the arrow tail.
-        :param y_tail: The y-coordinate of the arrow tail.
-        :param x_head: The x-coordinate of the arrow head.
-        :param y_head: The y-coordinate of the arrow head.
-        :param dx: Arrow length in the x direction. Only used if x_head is None.
-        :param dy: Arrow length in the y direction. Only used if y_head is None.
-        :param width: Width of full arrow tail. default: 0.001
-        :param alpha: Opacity.
-        :param cap_style: Cap style.
-        :param color: Use to set both the edge-color and the face-color.
-        :param edge_color: Edge color.
-        :param face_color: Face color.
-        :param fill: Whether to fill the rectangle.
-        :param join_style: Join style.
-        :param label: Label for the object in the legend.
-        :param line_style: Line style for edge.
-        :param line_width: Line width for edge.
-        :param z_order: z-order for the arrow.
-        """
-        if not one_is_not_none(dx, x_head):
-            raise ValueError('Must give dx or x_head')
-        if not one_is_not_none(dy, y_head):
-            raise ValueError('Must give dy or y_head')
-        for kwargs in smart_zip_kwargs(
-                x=x_tail, y=y_tail, x_head=x_head, y_head=y_head,
-                dx=dx, dy=dy, width=width,
-                alpha=alpha, capstyle=cap_style,
-                color=color, edgecolor=edge_color, facecolor=face_color,
-                fill=fill, joinstyle=join_style, label=label,
-                linestyle=line_style, linewidth=line_width,
-                zorder=z_order
-        ):
-            kwargs = drop_none_values(kwargs)
-            kwargs = apply_mappings(kwargs, kwarg_mappings)
-            if kwargs['x_head'] is not None:
-                kwargs['dx'] = kwargs['x_head'] - kwargs['x']
-                kwargs.pop('x_head')
-            if kwargs['y_head'] is not None:
-                kwargs['dy'] = kwargs['y_head'] - kwargs['y']
-                kwargs.pop('y_head')
-            arrow = Arrow(**kwargs)
-            self._axes.add_artist(arrow)
-
-        return self
-
-    def add_circle(
-            self,
-            x_center: FloatOrFloatIterable,
-            y_center: FloatOrFloatIterable,
-            radius: FloatOrFloatIterable,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            label: Optional[StrOrStrIterable] = None,
-            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None,
-            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a rectangle to the Axes.
-
-        :param x_center: The left rectangle coordinate.
-        :param y_center: The bottom rectangle coordinate.
-        :param radius: The radius of the circle.
-        :param alpha: Opacity.
-        :param color: Use to set both the edge-color and the face-color.
-        :param edge_color: Edge color.
-        :param face_color: Face color.
-        :param fill: Whether to fill the rectangle.
-        :param join_style: Join style.
-        :param label: Label for the object in the legend.
-        :param line_style: Line style for edge.
-        :param line_width: Line width for edge.
-        :param cap_style: Cap style.
-        :param z_order: z-order for the circle.
-        """
-        for kwargs in smart_zip_kwargs(
-                x_center=x_center, y_center=y_center, radius=radius,
-                alpha=alpha, capstyle=cap_style,
-                color=color, edgecolor=edge_color, facecolor=face_color,
-                fill=fill, joinstyle=join_style, label=label,
-                linestyle=line_style, linewidth=line_width,
-                zorder=z_order
-        ):
-            kwargs = drop_none_values(kwargs)
-            kwargs = apply_mappings(kwargs, kwarg_mappings)
-            kwargs['xy'] = kwargs.pop('x_center'), kwargs.pop('y_center')
-            circle = Circle(**kwargs)
-            self._axes.add_artist(circle)
-
-        return self
-
-    def add_ellipse(
-            self,
-            x_center: FloatOrFloatIterable,
-            y_center: FloatOrFloatIterable,
-            width: FloatOrFloatIterable,
-            height: FloatOrFloatIterable,
-            angle: FloatOrFloatIterable = 0.0,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
-            label: Optional[StrOrStrIterable] = None,
-            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ):
-        """
-        Add an elliptical arc, i.e. a segment of an ellipse.
-
-        :param x_center: The x-coordinate of the center of the ellipse.
-        :param y_center: The y-coordinate of the center of the ellipse.
-        :param width: The length (diameter) of the horizontal axis.
-        :param height: The length (diameter) of the vertical axis.
-        :param angle: Rotation of the ellipse in degrees (counter-clockwise).
-        :param alpha: Opacity.
-        :param cap_style: Cap style.
-        :param color: Use to set both the edge-color and the face-color.
-        :param edge_color: Edge color.
-        :param face_color: Face color.
-        :param fill: Whether to fill the rectangle.
-        :param join_style: Join style.
-        :param label: Label for the object in the legend.
-        :param line_style: Line style for edge.
-        :param line_width: Line width for edge.
-        :param z_order: z-order for the ellipse.
-        """
-        for kwargs in smart_zip_kwargs(
-            x_center=x_center, y_center=y_center,
-            width=width, height=height, angle=angle,
-            alpha=alpha, capstyle=cap_style,
-            color=color, edgecolor=edge_color, facecolor=face_color,
-            fill=fill, joinstyle=join_style, label=label,
-            linestyle=line_style, linewidth=line_width, zorder=z_order
-        ):
-            kwargs = drop_none_values(kwargs)
-            kwargs = apply_mappings(kwargs, kwarg_mappings)
-            kwargs['xy'] = kwargs.pop('x_center'), kwargs.pop('y_center')
-            ellipse = Ellipse(**kwargs)
-            self._axes.add_artist(ellipse)
-
-        return self
-
-    def add_fancy_arrow(
-            self,
-            x_tail: FloatOrFloatIterable,
-            y_tail: FloatOrFloatIterable,
-            x_head: Optional[FloatOrFloatIterable] = None,
-            y_head: Optional[FloatOrFloatIterable] = None,
-            dx: Optional[FloatOrFloatIterable] = None,
-            dy: Optional[FloatOrFloatIterable] = None,
-            tail_width: FloatOrFloatIterable = 0.001,
-            length_includes_head: BoolOrBoolIterable = False,
-            head_width: Optional[FloatOrFloatIterable] = None,
-            head_length: Optional[FloatOrFloatIterable] = None,
-            shape: StrOrStrIterable = 'full',
-            overhang: FloatOrFloatIterable = 0.0,
-            head_starts_at_zero: BoolOrBoolIterable = False,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
-            label: Optional[StrOrStrIterable] = None,
-            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ):
-        """
-        Like Arrow, but lets you set head width and head height independently.
-
-        :param x_tail: The x-coordinate of the arrow tail.
-        :param y_tail: The y-coordinate of the arrow tail.
-        :param x_head: The x-coordinate of the arrow head.
-        :param y_head: The y-coordinate of the arrow head.
-        :param dx: Arrow length in the x direction. Only used if x_head is None.
-        :param dy: Arrow length in the y direction. Only used if y_head is None.
-        :param tail_width: Width of full arrow tail.
-        :param length_includes_head: True if head is to be counted in
-                                     calculating the length.
-        :param head_width: Total width of the full arrow head
-        :param head_length: Length of arrow head
-        :param shape: Draw the left-half, right-half, or full arrow.
-                      One of ['full', 'left', 'right'].
-        :param overhang: Fraction that the arrow is swept back
-                         (0 overhang means triangular shape).
-                         Can be negative or greater than one.
-        :param head_starts_at_zero: If True, the head starts being drawn at
-                                    coordinate 0 instead of ending at
-                                    coordinate 0.
-        :param alpha: Opacity.
-        :param cap_style: Cap style.
-        :param color: Use to set both the edge-color and the face-color.
-        :param edge_color: Edge color.
-        :param face_color: Face color.
-        :param fill: Whether to fill the rectangle.
-        :param join_style: Join style.
-        :param label: Label for the object in the legend.
-        :param line_style: Line style for edge.
-        :param line_width: Line width for edge.
-        :param z_order: z-order for the arrow.
-        """
-        if not one_is_not_none(dx, x_head):
-            raise ValueError('Must give dx or x_head')
-        if not one_is_not_none(dy, y_head):
-            raise ValueError('Must give dy or y_head')
-        for kwargs in smart_zip_kwargs(
-                x=x_tail, y=y_tail, x_head=x_head, y_head=y_head,
-                dx=dx, dy=dy, width=tail_width,
-                length_includes_head=length_includes_head,
-                head_width=head_width, head_length=head_length,
-                shape=shape, overhang=overhang,
-                head_starts_at_zero=head_starts_at_zero,
-                alpha=alpha, capstyle=cap_style,
-                color=color, edgecolor=edge_color, facecolor=face_color,
-                fill=fill, joinstyle=join_style, label=label,
-                linestyle=line_style, linewidth=line_width,
-                zorder=z_order
-        ):
-            kwargs = drop_none_values(kwargs)
-            kwargs = apply_mappings(kwargs, kwarg_mappings)
-            if kwargs['x_head'] is not None:
-                kwargs['dx'] = kwargs['x_head'] - kwargs['x']
-                kwargs.pop('x_head')
-            if kwargs['y_head'] is not None:
-                kwargs['dy'] = kwargs['y_head'] - kwargs['y']
-                kwargs.pop('y_head')
-            arrow = FancyArrow(**kwargs)
-            self._axes.add_artist(arrow)
-
-        return self
-
-    def add_fancy_arrow_patch(
-            self,
-            x: FloatOrFloatIterable,
-            y: FloatOrFloatIterable,
-            dx: FloatOrFloatIterable,
-            dy: FloatOrFloatIterable,
-            path: Optional[Union[Path, PathIterable]] = None,
-            arrow_style: Union[ArrowStyle, ArrowStyleIterable] = 'simple',
-            connection_style: Union[
-                ConnectionStyle, ConnectionStyleIterable
-            ] = CONNECTION_STYLE.arc_3,
-            tail_patch: Optional[Union[Patch, PatchIterable]] = None,
-            head_patch: Optional[Union[Patch, PatchIterable]] = None,
-            tail_shrink_factor: Optional[FloatOrFloatIterable] = 2,
-            head_shrink_factor: Optional[FloatOrFloatIterable] = 2,
-            mutation_scale: Optional[FloatOrFloatIterable] = 1,
-            mutation_aspect: Optional[FloatOrFloatIterable] = None,
-            dpi_cor: Optional[FloatOrFloatIterable] = 1,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
-            label: Optional[StrOrStrIterable] = None,
-            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ):
-        """
-        Like Arrow, but lets you set head width and head height independently.
-
-        :param x: The x-coordinate of the arrow tail.
-        :param y: The y-coordinate of the arrow tail.
-        :param dx: Arrow length in the x direction.
-        :param dy: Arrow length in the y direction.
-        :param path: If provided, an arrow is drawn along this path and
-                     tail_patch, head_patch, tail_shrink_factor, and
-                     head_shrink_factor are ignored.
-        :param arrow_style: Describes how the fancy arrow will be drawn.
-                            It can be string of the available arrowstyle names,
-                            with optional comma-separated attributes,
-                            or an ArrowStyle instance.
-                            The optional attributes are meant to be scaled with
-                            the mutation_scale.
-        :param connection_style: Describes how the arrow ends are connected.
-        :param tail_patch: Optional tail patch.
-        :param head_patch: Optional head patch.
-        :param tail_shrink_factor: Shrinking factor of the tail.
-        :param head_shrink_factor: Shrinking factor of the head.
-        :param mutation_scale: Value with which attributes of arrowstyle
-                               (e.g., head_length) will be scaled.
-        :param mutation_aspect: The height of the rectangle will be squeezed by
-                                this value before the mutation and the mutated
-                                box will be stretched by the inverse of it.
-        :param dpi_cor: dpi_cor is currently used for linewidth-related things
-                        and shrink factor. Mutation scale is affected by this.
-        :param alpha: Opacity.
-        :param cap_style: Cap style.
-        :param color: Use to set both the edge-color and the face-color.
-        :param edge_color: Edge color.
-        :param face_color: Face color.
-        :param fill: Whether to fill the rectangle.
-        :param join_style: Join style.
-        :param label: Label for the object in the legend.
-        :param line_style: Line style for edge.
-        :param line_width: Line width for edge.
-        :param z_order: z-order for the arrow.
-        """
-        for kwargs in smart_zip_kwargs(
-                x=x, y=y, dx=dx, dy=dy, path=path,
-                arrowstyle=arrow_style, connectionstyle=connection_style,
-                patchA=tail_patch, patchB=head_patch,
-                shrinkA=tail_shrink_factor, shrinkB=head_shrink_factor,
-                mutation_scale=mutation_scale, mutation_aspect=mutation_aspect,
-                dpi_cor=dpi_cor,
-                alpha=alpha, capstyle=cap_style,
-                color=color, edgecolor=edge_color, facecolor=face_color,
-                fill=fill, joinstyle=join_style, label=label,
-                linestyle=line_style, linewidth=line_width,
-                zorder=z_order
-        ):
-            x = kwargs.pop('x')
-            y = kwargs.pop('y')
-            dx = kwargs.pop('dx')
-            dy = kwargs.pop('dy')
-            kwargs['posA'] = x, y
-            kwargs['posB'] = x + dx, y + dy
-            kwargs = drop_none_values(kwargs)
-            kwargs = apply_mappings(kwargs, kwarg_mappings)
-            arrow = FancyArrowPatch(**kwargs)
-            self._axes.add_artist(arrow)
-
-        return self
-
-    def add_fancy_box_patch(
-            self,
-            x: FloatOrFloatIterable,
-            y: FloatOrFloatIterable,
-            width: FloatOrFloatIterable,
-            height: FloatOrFloatIterable,
-            box_style: Union[
-                BoxStyleType, BoxStyleTypeIterable] = BOX_STYLE.round,
-            mutation_scale: Optional[FloatOrFloatIterable] = 1,
-            mutation_aspect: Optional[FloatOrFloatIterable] = None,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
-            label: Optional[StrOrStrIterable] = None,
-            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ):
-        """
-        A fancy box around a rectangle with lower left at xy = (x, y)
-        with specified width and height.
-
-        :param x: The left coord of the rectangle.
-        :param y: The bottom coord of the rectangle.
-        :param width: The rectangle width.
-        :param height: The rectangle height.
-        :param box_style: The box style.
-        :param mutation_scale: Value with which attributes of arrowstyle
-                               (e.g. head_length) will be scaled.
-        :param mutation_aspect: The height of the rectangle will be squeezed by
-                                this value before the mutation and the mutated
-                                box will be stretched by the inverse of it.
-        :param alpha: Opacity.
-        :param cap_style: Cap style.
-        :param color: Use to set both the edge-color and the face-color.
-        :param edge_color: Edge color.
-        :param face_color: Face color.
-        :param fill: Whether to fill the rectangle.
-        :param join_style: Join style.
-        :param label: Label for the object in the legend.
-        :param line_style: Line style for edge.
-        :param line_width: Line width for edge.
-        :param z_order: z-order for the box.
-        """
-        for kwargs in smart_zip_kwargs(
-                x=x, y=y, width=width, height=height,
-                boxstyle=box_style,
-                mutation_scale=mutation_scale, mutation_aspect=mutation_aspect,
-                alpha=alpha, fill=fill,
-                color=color, edgecolor=edge_color, facecolor=face_color,
-                capstyle=cap_style, joinstyle=join_style,
-                label=label,
-                linestyle=line_style, linewidth=line_width,
-                zorder=z_order,
-        ):
-            kwargs = drop_none_values(kwargs)
-            kwargs = apply_mappings(kwargs, kwarg_mappings)
-            kwargs['xy'] = kwargs.pop('x'), kwargs.pop('y')
-            fancy_box = FancyBboxPatch(**kwargs)
-            self._axes.add_artist(fancy_box)
-
-        return self
-
-    def add_polygon(
-            self,
-            xy: Union[ndarray, NdArrayIterable],
-            closed: BoolOrBoolIterable = True,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            label: Optional[StrOrStrIterable] = None,
-            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None,
-            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a general polygon patch.
-
-        :param xy: A numpy array with shape Nx2.
-        :param closed: If True, the polygon will be closed so the starting and
-                       ending points are the same.
-        :param alpha: Opacity.
-        :param cap_style: Cap style.
-        :param color: Use to set both the edge-color and the face-color.
-        :param edge_color: Edge color.
-        :param face_color: Face color.
-        :param fill: Whether to fill the rectangle.
-        :param join_style: Join style.
-        :param label: Label for the object in the legend.
-        :param line_style: Line style for edge.
-        :param line_width: Line width for edge.
-        :param z_order: z-order for the polygon.
-        """
-        for kwargs in smart_zip_kwargs(
-                xy=xy, closed=closed,
-                alpha=alpha, color=color, edgecolor=edge_color,
-                facecolor=face_color, fill=fill,
-                label=label,
-                linestyle=line_style, linewidth=line_width,
-                capstyle=cap_style, joinstyle=join_style,
-                zorder=z_order,
-        ):
-            kwargs = drop_none_values(kwargs)
-            kwargs = apply_mappings(kwargs, kwarg_mappings)
-            polygon = Polygon(**kwargs)
-            self._axes.add_artist(polygon)
-
-        return self
-
-    def add_rectangle(
-            self,
-            width: FloatOrFloatIterable, 
-            height: FloatOrFloatIterable,
-            angle: FloatOrFloatIterable = 0.0,
-            x_left: Optional[FloatOrFloatIterable] = None, 
-            y_bottom: Optional[FloatOrFloatIterable] = None,
-            x_center: Optional[FloatOrFloatIterable] = None, 
-            y_center: Optional[FloatOrFloatIterable] = None,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
-            label: Optional[StrOrStrIterable] = None,
-            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a rectangle to the Axes.
-
-        :param x_left: The left rectangle coordinate.
-        :param y_bottom: The bottom rectangle coordinate.
-        :param width: Rectangle width.
-        :param height: Rectangle height.
-        :param x_left: The left rectangle coordinate.
-        :param y_bottom: The bottom rectangle coordinate.
-        :param x_center: The center rectangle x-coordinate.
-        :param y_center: The center rectangle y-coordinate.
-        :param angle: Rotation in degrees anti-clockwise about xy (default=0.0)
-        :param alpha: Opacity.
-        :param cap_style: Cap style.
-        :param color: Use to set both the edge-color and the face-color.
-        :param edge_color: Edge color.
-        :param face_color: Face color.
-        :param fill: Whether to fill the rectangle.
-        :param join_style: Join style.
-        :param label: Label for the object in the legend.
-        :param line_style: Line style for edge.
-        :param line_width: Line width for edge.
-        :param z_order: z-order for the rectangle.
-        """
-        for kwargs in smart_zip_kwargs(
-                width=width, height=height, angle=angle,
-                x_left=x_left, y_bottom=y_bottom,
-                x_center=x_center, y_center=y_center,
-                alpha=alpha, fill=fill, label=label,
-                color=color, edgecolor=edge_color, facecolor=face_color,
-                capstyle=cap_style, joinstyle=join_style,
-                linestyle=line_style, linewidth=line_width,
-                zorder=z_order
-        ):
-
-            if not one_is_not_none(x_left, x_center):
-                raise ValueError('Give one of {x_left, x_center}')
-            if not one_is_not_none(y_bottom, y_center):
-                raise ValueError('Give one of {y_bottom, y_center}')
-            if not (
-                    all_are_none(x_left, y_bottom) or
-                    all_are_none(x_center, y_center)
-            ):
-                raise ValueError(
-                    'Give either {x_left, y_bottom} or {x_center, y_center}'
-                )
-
-            kwargs = drop_none_values(kwargs)
-            kwargs = apply_mappings(kwargs, kwarg_mappings)
-
-            if all_are_none(x_left, y_bottom):
-                x_c = kwargs.pop('x_center')
-                y_c = kwargs.pop('y_center')
-                w = kwargs['width']
-                h = kwargs['height']
-                a = kwargs['angle']
-                x_l = x_c - w / 2
-                y_b = y_c - h / 2
-                r = ((w / 2) ** 2 + (h / 2) ** 2) ** 0.5
-                theta = atan2(h, w)
-                xc_new = x_l + r * cos(theta + pi * a / 180)
-                yc_new = y_b + r * sin(theta + pi * a / 180)
-                kwargs['x'] = x_l + x_c - xc_new
-                kwargs['y'] = y_b + y_c - yc_new
-            else:
-                kwargs['x'] = kwargs.pop('x_left')
-                kwargs['y'] = kwargs.pop('y_bottom')
-
-            kwargs['xy'] = kwargs.pop('x'), kwargs.pop('y')
-
-            rectangle = Rectangle(**kwargs)
-            self._axes.add_artist(rectangle)
-
-        return self
-
-    def add_regular_polygon(
-            self,
-            x_center: FloatOrFloatIterable,
-            y_center: FloatOrFloatIterable,
-            num_vertices: IntOrIntIterable,
-            radius: FloatOrFloatIterable,
-            angle: FloatOrFloatIterable = 0,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            label: Optional[StrOrStrIterable] = None,
-            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None,
-            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a rectangle to the Axes.
-
-        :param x_center: The x-coordinate of the center of the polygon.
-        :param y_center: The y-coordinate of the center of the polygon.
-        :param num_vertices: Number of vertices.
-        :param radius: The distance from the center to each of the vertices.
-        :param angle: Rotation in degrees anti-clockwise about xy
-                            (default is 0.0)
-        :param alpha: Opacity.
-        :param cap_style: Cap style.
-        :param color: Use to set both the edge-color and the face-color.
-        :param edge_color: Edge color.
-        :param face_color: Face color.
-        :param fill: Whether to fill the rectangle.
-        :param join_style: Join style.
-        :param label: Label for the object in the legend.
-        :param line_style: Line style for edge.
-        :param line_width: Line width for edge.
-        :param z_order: z-order for the polygon.
-        """
-        for kwargs in smart_zip_kwargs(
-                x_center=x_center, y_center=y_center,
-                numVertices=num_vertices, radius=radius, angle=angle,
-                alpha=alpha, fill=fill, label=label,
-                color=color, edgecolor=edge_color, facecolor=face_color,
-                linestyle=line_style, linewidth=line_width,
-                capstyle=cap_style, joinstyle=join_style,
-                zorder=z_order,
-        ):
-            kwargs = drop_none_values(kwargs)
-            kwargs = apply_mappings(kwargs, kwarg_mappings)
-            kwargs['orientation'] = pi * kwargs.pop('angle') / 180
-            polygon = RegularPolygon(**kwargs)
-            self._axes.add_artist(polygon)
-
-        return self
-
-    def add_wedge(
-            self,
-            x_center: FloatOrFloatIterable,
-            y_center: FloatOrFloatIterable,
-            radius: FloatOrFloatIterable,
-            theta_start: FloatOrFloatIterable,
-            theta_end: FloatOrFloatIterable,
-            width: Optional[FloatOrFloatIterable] = None,
-            alpha: Optional[FloatOrFloatIterable] = None,
-            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
-            label: Optional[StrOrStrIterable] = None,
-            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None,
-            z_order: Optional[IntOrIntIterable] = None
-    ):
-        """
-        Add a wedge-shaped patch.
-
-        :param x_center: The x-coordinate of the center of the ellipse.
-        :param y_center: The y-coordinate of the center of the ellipse.
-        :param radius: (Outer) radius.
-        :param theta_start: Starting angle of the arc in degrees.
-                            Relative to angle, e.g. if angle = 45 and
-                            theta_start = 90 the absolute starting angle is 135.
-        :param theta_end: Ending angle of the arc in degrees.
-        :param width: If width is given, then a partial wedge is drawn from
-                      inner radius - width to outer radius.
-        :param alpha: Opacity.
-        :param cap_style: Cap style.
-        :param color: Use to set both the edge-color and the face-color.
-        :param edge_color: Edge color.
-        :param face_color: Face color.
-        :param fill: Whether to fill the rectangle.
-        :param join_style: Join style.
-        :param label: Label for the object in the legend.
-        :param line_style: Line style for edge.
-        :param line_width: Line width for edge.
-        :param z_order: z-order for the wedge.
-        """
-        for kwargs in smart_zip_kwargs(
-                x_center=x_center, y_center=y_center, r=radius,
-                theta1=theta_start, theta2=theta_end,
-                width=width, alpha=alpha, fill=fill,
-                color=color, edgecolor=edge_color, facecolor=face_color,
-                capstyle=cap_style, joinstyle=join_style, linestyle=line_style,
-                linewidth=line_width,
-                label=label, zorder=z_order,
-        ):
-            kwargs = drop_none_values(kwargs)
-            kwargs = apply_mappings(kwargs, kwarg_mappings)
-            kwargs['orientation'] = pi * kwargs.pop('angle') / 180
-            wedge = Wedge(**kwargs)
-            self._axes.add_artist(wedge)
-
-        return self
-
-    @property
-    def arcs(self) -> PatchListFormatter:
-        """
-        Return a list of the Arcs on the axes.
-        """
-        return PatchListFormatter([
-            a for a in self._axes.get_children()
-            if isinstance(a, Arc)
-        ])
-
-    @property
-    def arrows(self) -> PatchListFormatter:
-        """
-        Return a list of the Arrows on the axes.
-        """
-        return PatchListFormatter([
-            a for a in self._axes.get_children()
-            if isinstance(a, Arrow)
-        ])
-
-    @property
-    def circles(self) -> PatchListFormatter:
-        """
-        Return a list of the Circles on the axes.
-        """
-        return PatchListFormatter([
-            c for c in self._axes.get_children()
-            if isinstance(c, Circle)
-        ])
-
-    @property
-    def ellipses(self) -> PatchListFormatter:
-        """
-        Return a list of the Ellipses on the axes.
-        """
-        return PatchListFormatter([
-            e for e in self._axes.get_children()
-            if isinstance(e, Ellipse)
-        ])
-
-    @property
-    def fancy_arrows(self) -> PatchListFormatter:
-        """
-        Return a list of the FancyArrows on the axes.
-        """
-        return PatchListFormatter([
-            a for a in self._axes.get_children()
-            if isinstance(a, FancyArrow)
-        ])
-
-    @property
-    def fancy_arrow_patches(self) -> PatchListFormatter:
-        """
-        Return a list of the FancyArrowPatches on the axes.
-        """
-        return PatchListFormatter([
-            a for a in self._axes.get_children()
-            if isinstance(a, FancyArrowPatch)
-        ])
-
-    @property
-    def fancy_boxes(self) -> PatchListFormatter:
-        """
-        Return a list of the FancyBoxes on the axes.
-        """
-        return PatchListFormatter([
-            b for b in self._axes.get_children()
-            if isinstance(b, FancyBboxPatch)
-        ])
-
-    @property
-    def polygons(self) -> PatchListFormatter:
-        """
-        Return a list of the Polygons on the axes.
-        """
-        return PatchListFormatter([
-            p for p in self._axes.get_children()
-            if isinstance(p, Polygon)
-        ])
-
-    @property
-    def regular_polygons(self) -> PatchListFormatter:
-        """
-        Return a list of the RegularPolygons on the axes.
-        """
-        return PatchListFormatter([
-            r for r in self._axes.get_children()
-            if isinstance(r, RegularPolygon)
-        ])
-
-    @property
-    def wedges(self) -> PatchListFormatter:
-        """
-        Return a list of the Wedges on the axes.
-        """
-        return PatchListFormatter([
-            w for w in self._axes.get_children()
-            if isinstance(w, Wedge)
-        ])
-
-    # endregion
-
-    # region custom shapes
-
-    def add_v_density(
-            self,
-            x: float,
-            y_to_z: Series,
-            color: Optional[Color] = 'k',
-            color_min: Optional[Color] = None,
-            edge_color: Optional[Color] = None,
-            width: float = 0.8,
-            z_max: Optional[float] = None,
-            h_align: H_ALIGN = 'center'
-    ) -> 'AxesFormatter':
-        """
-        Add a vertical density bar to the plot.
-
-        :param x: The x-coordinate of the bar.
-        :param y_to_z: A mapping of the bar's y-coordinate to it density.
-        :param color: The color of the density bar.
-        :param color_min: Optional 2nd color to fade out to.
-        :param edge_color: Optional color for the outer edge of the density.
-        :param width: The bar width.
-        :param z_max: Value to scale down densities by to get to a range of
-                      0 to 1. Defaults to max value of y_to_z.
-        :param h_align: Horizontal alignment.
-                        One of {'left', 'center', 'right'}.
-        """
-        check_h_align(h_align)
-
-        if z_max is None:
-            z_max = y_to_z.max()
-        y = y_to_z.index.to_list()
-        y_lowers = y[: -1]
-        y_uppers = y[1:]
-
-        if h_align == 'left':
-            x_left = x
-        elif h_align == 'center':
-            x_left = x - width / 2
-        elif h_align == 'right':
-            x_left = x - width
-        else:
-            raise ValueError(f'h_align must be one of {H_ALIGN}')
-
-        alphas = (
-                y_to_z / z_max
-        ).rolling(2).mean().shift(-1).dropna().clip(0.0, 1.0)
-
-        if color_min is None:
-            color_min = color
-        colors = cross_fade(from_color=color_min, to_color=color,
-                            amount=alphas)
-        # add segments
-        for y_lower, y_upper, alpha, color in zip(
-                y_lowers, y_uppers, alphas, colors
-        ):
-            self.add_rectangle(
-                x_left=x_left, y_bottom=y_lower,
-                width=width, height=y_upper - y_lower,
-                face_color=color, alpha=alpha, line_width=0
-            )
-        # add edge
-        if edge_color is not None:
-            self.add_rectangle(
-                x_left=x_left, y_bottom=y_lowers[0],
-                width=width, height=y_uppers[-1] - y_lowers[0],
-                edge_color=edge_color, fill=False
-            )
-
-        return self
-
-    def add_h_density(
-            self, y: float,
-            x_to_z: Series,
-            color: Optional[Color] = 'k',
-            color_min: Optional[Color] = None,
-            edge_color: Optional[Color] = None,
-            height: float = 0.8,
-            z_max: Optional[float] = None,
-            v_align: V_ALIGN = 'center'
-    ) -> 'AxesFormatter':
-        """
-        Add a horizontal density bar to the plot.
-
-        :param y: The y-coordinate of the bar.
-        :param x_to_z: A mapping of the bar's x-coordinate to it density.
-        :param color: The color of the density bar.
-        :param color_min: Optional 2nd color to fade out to.
-        :param edge_color: Optional color for the outer edge of the density.
-        :param height: The bar width.
-        :param z_max: Value to scale down densities by to get to a range of
-                      0 to 1. Defaults to max value of x_to_z.
-        :param v_align: Vertical alignment.
-                        One of {'top', 'center', 'bottom'}.
-        """
-        check_v_align(v_align)
-
-        if z_max is None:
-            z_max = x_to_z.max()
-        x = x_to_z.index.to_list()
-        x_lefts = x[: -1]
-        x_rights = x[1:]
-
-        if v_align == 'bottom':
-            y_bottom = y
-        elif v_align == 'center':
-            y_bottom = y - height / 2
-        elif v_align == 'top':
-            y_bottom = y - height
-        else:
-            raise ValueError(f'v_align must be one of {V_ALIGN}')
-
-        alphas = (
-                x_to_z / z_max
-        ).rolling(2).mean().shift(-1).dropna().clip(0.0, 1.0)
-
-        if color_min is None:
-            color_min = color
-        colors = cross_fade(from_color=color_min, to_color=color,
-                            amount=alphas)
-        # add segments
-        for x_left, x_right, alpha, color in zip(
-                x_lefts, x_rights, alphas, colors
-        ):
-            self.add_rectangle(
-                x_left=x_left, y_bottom=y_bottom,
-                width=x_right-x_left, height=height,
-                face_color=color, alpha=alpha, line_width=0
-            )
-        # add edge
-        if edge_color is not None:
-            self.add_rectangle(
-                x_left=x_lefts[0], y_bottom=y_bottom,
-                width=x_rights[-1] - x_rights[0], height=height,
-                edge_color=edge_color, fill=False
-            )
-        return self
-
-    # endregion
-
-    # region plots
-
-    def add_v_bars(
-            self,
-            x: Union[str, FloatOrFloatIterable],
-            y: Union[str, FloatOrFloatIterable],
-            width: Union[str, FloatOrFloatIterable],
-            box_style: Union[BoxStyle, Iterable[BoxStyle]],
-            data: Optional[DataFrame] = None,
-            y_0: Optional[Union[str, FloatOrFloatIterable]] = 0.0,
-            h_align: H_ALIGN = 'center',
-            mutation_scale: Union[str, FloatOrFloatIterable] = 1,
-            mutation_aspect: Optional[Union[str, FloatOrFloatIterable]] = None,
-            alpha: Optional[Union[str, FloatOrFloatIterable]] = None,
-            cap_style: Optional[Union[
-                StrOrStrIterable, CAP_STYLE, Iterable[CAP_STYLE]
-            ]] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            line_style: Optional[Union[
-                StrOrStrIterable, LINE_STYLE, Iterable[LINE_STYLE]
-            ]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None
-    ) -> 'AxesFormatter':
-        """
-        Add vertical bars to the plot with the given BoxStyle.
-
-        :param x: X-coordinate for each bar, or name of column.
-        :param y: Y-coordinate of top of each bar, or name of column.
-        :param width: Width of each bar, or name of column.
-        :param box_style: The style of each box, or name of column.
-        :param data: Optional DataFrame to extract sequences of attributes.
-        :param y_0: Y-coordinate of bottom of each bar. Defaults to 0.
-        :param h_align: Horizontal alignment. One of {'left', 'center', 'right'}
-        :param mutation_scale: Scaling factor applied to the attributes of the
-                               box style (e.g. pad or rounding_size).
-        :param mutation_aspect: The height of the rectangle will be squeezed by
-                                this value before the mutation and the mutated
-                                box will be stretched by the inverse of it.
-                                For example, this allows different horizontal
-                                and vertical padding.
-        :param alpha: Opacity from 0 to 1.
-        :param cap_style: One of {'butt', 'round', 'projecting'}
-        :param color: Color for faces and edges.
-        :param edge_color: Color for edges.
-        :param face_color: Color for faces.
-        :param fill: Whether bars are filled.
-        :param line_style: Line style.
-        :param line_width: Line width.
-        """
-        check_h_align(h_align)
-
-        def get_data(item) -> Series:
-            if data is None:
-                return item
-            if isinstance(item, str) and item in data.columns:
-                return data[item]
-            else:
-                return item
-
-        def make_iterable(item):
-            if not isinstance(item, Iterable) or isinstance(item, str):
-                item = [item] * len(x)
-            return item
-
-        x = get_data(x)
-        y = make_iterable(get_data(y))
-        y_0 = make_iterable(get_data(y_0))
-        width = make_iterable(get_data(width))
-        box_style = make_iterable(get_data(box_style))
-        mutation_scale = make_iterable(get_data(mutation_scale))
-        mutation_aspect = make_iterable(get_data(mutation_aspect))
-        alpha = make_iterable(get_data(alpha))
-        cap_style = make_iterable(get_data(cap_style))
-        color = make_iterable(get_data(color))
-        edge_color = make_iterable(get_data(edge_color))
-        face_color = make_iterable(get_data(face_color))
-        fill = make_iterable(get_data(fill))
-        line_style = make_iterable(get_data(line_style))
-        line_width = make_iterable(get_data(line_width))
-
-        for (
-                x_i, y_i, y_0_i, w_i, bs_i,
-                ms_i, ma_i, a_i, cs_i,
-                c_i, ec_i, fc_i,
-                f_i, ls_i, lw_i
-        ) in zip(
-            x, y, y_0, width, box_style,
-            mutation_scale, mutation_aspect, alpha, cap_style,
-            color, edge_color, face_color,
-            fill, line_style, line_width
-        ):
-            if h_align == 'left':
-                x_p = x_i
-            elif h_align == 'center':
-                x_p = x_i - w_i / 2
-            else:
-                x_p = x_i - width
-
-            self.add_fancy_box_patch(
-                x=x_p, y=y_0_i, width=w_i, height=y_i - y_0_i,
-                box_style=bs_i,
-                mutation_scale=ms_i, mutation_aspect=ma_i,
-                alpha=a_i, cap_style=cs_i,
-                color=c_i, edge_color=ec_i, face_color=fc_i,
-                fill=f_i, line_style=ls_i, line_width=lw_i
-            )
-
-        return self
-
-    def add_v_pills(
-            self,
-            x: Union[str, FloatOrFloatIterable],
-            y: Union[str, FloatOrFloatIterable],
-            width: float,
-            data: Optional[DataFrame] = None,
-            y_0: Optional[Union[str, FloatOrFloatIterable]] = 0.0,
-            h_align: H_ALIGN = 'center',
-            alpha: Optional[Union[str, FloatOrFloatIterable]] = None,
-            color: Optional[ColorOrColorIterable] = None,
-            edge_color: Optional[ColorOrColorIterable] = None,
-            face_color: Optional[ColorOrColorIterable] = None,
-            fill: BoolOrBoolIterable = True,
-            line_style: Optional[Union[
-                StrOrStrIterable, LINE_STYLE, Iterable[LINE_STYLE]
-            ]] = None,
-            line_width: Optional[FloatOrFloatIterable] = None
-    ) -> 'AxesFormatter':
-        """
-        Add vertical bars to the plot with the given BoxStyle.
-
-        :param x: X-coordinate for each bar, or name of column.
-        :param y: Y-coordinate of top of each bar, or name of column.
-        :param width: Width of each bar, or name of column.
-        :param data: Optional DataFrame to extract sequences of attributes.
-        :param y_0: Y-coordinate of bottom of each bar. Defaults to 0.
-        :param h_align: One of {'left', 'center', 'right'}.
-        :param alpha: Opacity from 0 to 1.
-        :param color: Color for faces and edges.
-        :param edge_color: Color for edges.
-        :param face_color: Color for faces.
-        :param fill: Whether bars are filled.
-        :param line_style: Line style.
-        :param line_width: Line width.
-        """
-        mutation_aspect = (
-                (self.width() / self.height()) *
-                (self.get_y_height() / self.get_x_width())
-        )
-        self.add_v_bars(
-            data=data, x=x, y=y, width=width,
-            box_style=BoxStyle.Round(pad=0.0, rounding_size=width / 2),
-            y_0=y_0, h_align=h_align,
-            mutation_aspect=mutation_aspect,
-            alpha=alpha,
-            color=color, edge_color=edge_color, face_color=face_color,
-            fill=fill, line_style=line_style, line_width=line_width
-        )
-        return self
-
-    def add_line(
-            self,
-            x: FloatIterable, y: FloatIterable,
-            smooth: Union[bool, int] = False, smooth_order: int = 2,
-            alpha: Optional[float] = None,
-            color: Optional[Color] = None,
-            draw_style: Optional[Union[str, DRAW_STYLE]] = None,
-            label: Optional[str] = None,
-            line_style: Optional[LineStyle] = None,
-            line_width: Optional[float] = None,
-            marker: Optional[Union[str, MARKER_STYLE]] = None,
-            marker_edge_color: Optional[Color] = None,
-            marker_edge_width: Optional[float] = None,
-            marker_face_color: Optional[Color] = None,
-            marker_face_color_alt: Optional[Color] = None,
-            marker_size: Optional[float] = None,
-            z_order: Optional[int] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a line to the plot.
-
-        :param x: X-coordinates of the line.
-        :param y: Y-coordinates of the line.
-        :param smooth: True or False or number of points. True -> 1,000 points.
-        :param smooth_order: Order for smoothing e.g. 2 = quadratic, 3 = cubic
-        :param alpha: Opacity of the line.
-        :param color: Color of the line.
-        :param draw_style: Draw style. One of {'default', 'steps', 'steps-pre',
-                           'steps-mid', 'steps-post'}
-        :param label: Label.
-        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
-                           (offset, on-off-seq), ...}
-        :param line_width: Line width.
-        :param marker: Marker style.
-        :param marker_edge_color: Marker edge color.
-        :param marker_edge_width: Marker edge width.
-        :param marker_face_color: Marker face color.
-        :param marker_face_color_alt: Alt marker face color.
-        :param marker_size: Marker size.
-        :param z_order: z-order for the line.
-        """
-        if smooth is not False:
-            if smooth is True:
-                smooth = 1000
-            f_smooth = interp1d(x, y, kind=smooth_order)
-            x_smooth = linspace(min(x), max(x), smooth)
-            y_smooth = f_smooth(x_smooth)
-            x = x_smooth
-            y = y_smooth
-        if draw_style is not None:
-            draw_style = (
-                draw_style if isinstance(draw_style, str)
-                else DRAW_STYLE.get_name(draw_style)
-            )
-        if line_style is not None:
-            line_style = (
-                line_style if isinstance(line_style, str)
-                else LINE_STYLE.get_name(line_style)
-            )
-
-        self._axes.plot(
-            x, y, alpha=alpha, color=color,
-            drawstyle=draw_style,
-            label=label,
-            ls=line_style,
-            lw=line_width,
-            marker=marker,
-            markersize=marker_size,
-            mec=marker_edge_color,
-            mew=marker_edge_width,
-            mfc=marker_face_color,
-            mfcalt=marker_face_color_alt,
-            zorder=z_order
-        )
-        return self
-
-    # endregion
-
-    # endregion
-
-    def set_title_font_family(self, font_name: str) -> 'AxesFormatter':
-        """
-        Set the font family for the Axes title.
-
-        :param font_name: Name of the font.
-        """
-        self.title.set_font_family(font_name)
-        return self
-
-    # region limits
-
-    def get_x_lim(self) -> Tuple[float, float]:
-        """
-        Return the x-axis view limits.
-        """
-        return self._axes.get_xlim()
-
-    def get_y_lim(self) -> Tuple[float, float]:
-        """
-        Return the y-axis view limits.
-        """
-        return self._axes.get_ylim()
-
-    def set_x_lim(
-            self,
-            left: Optional[Union[float, date]] = None,
-            right: Optional[Union[float, date]] = None
-    ) -> 'AxesFormatter':
-        """
-        Set the limits of the x-axis.
-
-        :param left: Lower limit.
-        :param right: Upper limit.
-        """
-        self._axes.set_xlim(left=left, right=right)
-        return self
-
-    def set_y_lim(self, bottom: Optional[float] = None,
-                  top: Optional[float] = None) -> 'AxesFormatter':
-        """
-        Set the limits of the y-axis.
-
-        :param bottom: Lower limit.
-        :param top: Upper limit.
-        """
-        self._axes.set_ylim(bottom=bottom, top=top)
-        return self
-
-    def get_x_min(self) -> float:
-        """
-        Return the x-axis lower view limit.
-        """
-        return self.get_x_lim()[0]
-
-    def get_x_max(self) -> float:
-        """
-        Return the x-axis upper view limit.
-        """
-        return self.get_x_lim()[1]
-
-    def get_x_width(self) -> float:
-
-        return abs(self.get_x_max() - self.get_x_min())
-
-    def get_y_height(self) -> float:
-
-        return abs(self.get_y_max() - self.get_y_min())
-
-    def set_x_min(self, left: Union[float, date]) -> 'AxesFormatter':
-        """
-        Set the x-axis lower view limit.
-        """
-        self.set_x_lim(left, None)
-        return self
-
-    def set_x_max(self, right: Union[float, date] = None) -> 'AxesFormatter':
-        """
-        Set the x-axis upper view limit.
-        """
-        self.set_x_lim(None, right)
-        return self
-
-    def get_y_min(self) -> float:
-        """
-        Return the y-axis lower view limit.
-        """
-        return self.get_y_lim()[0]
-
-    def get_y_max(self) -> float:
-        """
-        Return the y-axis upper view limit.
-        """
-        return self.get_y_lim()[1]
-
-    def set_y_min(self, bottom: Union[float, date] = None) -> 'AxesFormatter':
-        """
-        Set the y-axis lower view limit.
-        """
-        self.set_y_lim(bottom, None)
-        return self
-
-    def set_y_max(self, top: Union[float, date] = None) -> 'AxesFormatter':
-        """
-        Set the y-axis upper view limit.
-        """
-        self.set_y_lim(None, top)
-        return self
-
-    def width(self, units: FIGURE_UNITS = 'inches') -> float:
-        """
-        Return the width of the subplot.
-
-        :param units: One of {'inches', 'pixels'}.
-        """
-        if units not in ('inches', 'pixels'):
-            raise ValueError("units not in ('inches', 'pixels')")
-        fig = self._axes.figure
-        bbox = self.axes.get_window_extent().transformed(
-            fig.dpi_scale_trans.inverted()
-        )
-        width = bbox.width
-        if units == 'pixels':
-            width *= fig.dpi
-        return width
-
-    def height(self, units: FIGURE_UNITS = 'inches') -> float:
-        """
-        Return the height of the subplot.
-
-        :param units: One of {'inches', 'pixels'}
-        """
-        if units not in ('inches', 'pixels'):
-            raise ValueError("units not in ('inches', 'pixels')")
-        fig = self._axes.figure
-        bbox = self.axes.get_window_extent().transformed(
-            fig.dpi_scale_trans.inverted()
-        )
-        height = bbox.height
-        if units == 'pixels':
-            height *= fig.dpi
-        return height
-
-    # endregion
-
-    # region frame
-
-    def show_frame(self) -> 'AxesFormatter':
-        """
-        Show the frame.
-        """
-        self._axes.set_frame_on(True)
-        return self
-
-    def hide_frame(self) -> 'AxesFormatter':
-        """
-        Hide the frame.
-        """
-        self._axes.set_frame_on(False)
-        return self
-
-    # endregion
-
-    # region grids
-
-    def grid(
-            self, value: bool = True,
-            which: WHICH_TICKS = 'major',
-            axis: WHICH_AXIS = 'both',
-            color: Optional[Color] = None,
-            line_width: Optional[float] = None,
-            line_style: Optional[LineStyle] = None
-    ) -> 'AxesFormatter':
-        """
-        Turn the grid on or off.
-
-        :param value: True or False. Defaults to True.
-        :param which: 'major', 'minor' or 'both'
-        :param axis: 'x', 'y' or 'both'
-        :param color: Color of the lines.
-        :param line_width: Line width.
-        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
-                           (offset, on-off-seq), ...}
-        """
-        kwargs = {}
-        if color is not None:
-            kwargs['color'] = color
-        if line_width is not None:
-            kwargs['lw'] = line_width
-        if line_style is not None:
-            kwargs['ls'] = LINE_STYLE.get_line_style(line_style)
-
-        self._axes.grid(b=value, which=which, axis=axis,
-                        **kwargs)
-        return self
-
-    def add_major_xy_grid(
-            self,
-            color: Optional[Color] = '#888888',
-            line_width: Optional[float] = None,
-            line_style: Optional[LineStyle] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a major grid to both axes.
-
-        :param color: Color of the lines.
-        :param line_width: Line width.
-        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
-                           (offset, on-off-seq), ...}
-        """
-        self.grid(
-            value=True, which='major', axis='both',
-            color=color, line_width=line_width, line_style=line_style
-        )
-        return self
-
-    def add_minor_xy_grid(
-            self,
-            color: Optional[Color] = '#bbbbbb',
-            line_width: Optional[float] = None,
-            line_style: Optional[LineStyle] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a minor grid to both axes.
-
-        :param color: Color of the lines.
-        :param line_width: Line width.
-        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
-                           (offset, on-off-seq), ...}
-        """
-        self.grid(
-            value=True, which='minor', axis='both',
-            color=color, line_width=line_width, line_style=line_style
-        )
-        return self
-
-    def add_major_x_grid(
-            self,
-            color: Optional[Color] = '#888888',
-            line_width: Optional[float] = None,
-            line_style: Optional[LineStyle] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a major grid to the x-axis.
-
-        :param color: Color of the lines.
-        :param line_width: Line width.
-        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
-                           (offset, on-off-seq), ...}
-        """
-        self.grid(
-            value=True, which='major', axis='x',
-            color=color, line_width=line_width, line_style=line_style
-        )
-        return self
-
-    def add_minor_x_grid(
-            self,
-            color: Optional[Color] = '#bbbbbb',
-            line_width: Optional[float] = None,
-            line_style: Optional[LineStyle] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a minor grid to the x-axis.
-
-        :param color: Color of the lines.
-        :param line_width: Line width.
-        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
-                           (offset, on-off-seq), ...}
-        """
-        self.grid(
-            value=True, which='minor', axis='x',
-            color=color, line_width=line_width, line_style=line_style
-        )
-        return self
-
-    def add_major_y_grid(
-            self,
-            color: Optional[Color] = '#888888',
-            line_width: Optional[float] = None,
-            line_style: Optional[LineStyle] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a major grid to the y-axis.
-
-        :param color: Color of the lines.
-        :param line_width: Line width.
-        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
-                           (offset, on-off-seq), ...}
-        """
-        self.grid(
-            value=True, which='major', axis='y',
-            color=color, line_width=line_width, line_style=line_style
-        )
-        return self
-
-    def add_minor_y_grid(
-            self,
-            color: Optional[Color] = '#bbbbbb',
-            line_width: Optional[float] = None,
-            line_style: Optional[LineStyle] = None
-    ) -> 'AxesFormatter':
-        """
-        Add a minor grid to the y-axis.
-
-        :param color: Color of the lines.
-        :param line_width: Line width.
-        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
-                           (offset, on-off-seq), ...}
-        """
-        self.grid(
-            value=True, which='minor', axis='y',
-            color=color, line_width=line_width, line_style=line_style
-        )
-        return self
-
-    # endregion
-
-    def set_aspect(self, aspect: ASPECT) -> 'AxesFormatter':
-        """
-        Set the aspect of the axis scaling, i.e. the ratio of y-unit to x-unit.
-        """
-        self._axes.set_aspect(aspect=aspect)
-        return self
-
-    def set_aspect_equal(self) -> 'AxesFormatter':
-        """
-        Set the aspect of the axis scaling to equal.
-        """
-        return self.set_aspect('equal')
-
-    def set_anchor(self, anchor: ANCHOR) -> 'AxesFormatter':
-        """
-        Define the anchor location.
-        """
-        self._axes.set_anchor(anchor=anchor)
-        return self
-
-    def set_anchor_north(self) -> 'AxesFormatter':
-        """
-        Set the anchor location to the top of the figure.
-        """
-        return self.set_anchor('N')
-
-    def set_anchor_east(self) -> 'AxesFormatter':
-        """
-        Set the anchor location to the right of the figure.
-        """
-        return self.set_anchor('E')
-
-    def set_anchor_south(self) -> 'AxesFormatter':
-        """
-        Set the anchor location to the bottom of the figure.
-        """
-        return self.set_anchor('S')
-
-    def set_anchor_west(self) -> 'AxesFormatter':
-        """
-        Set the anchor location to the left of the figure.
-        """
-        return self.set_anchor('W')
-
-    def set_anchor_center(self) -> 'AxesFormatter':
-        """
-        Set the anchor location to the middle of the figure.
-        """
-        return self.set_anchor('C')
-
-    def set_anchor_north_east(self) -> 'AxesFormatter':
-        """
-        Set the anchor location to the top right of the figure.
-        """
-        return self.set_anchor('NE')
-
-    def set_anchor_north_west(self) -> 'AxesFormatter':
-        """
-        Set the anchor location to the top left of the figure.
-        """
-        return self.set_anchor('NW')
-
-    def set_anchor_south_east(self) -> 'AxesFormatter':
-        """
-        Set the anchor location to the bottom right of the figure.
-        """
-        return self.set_anchor('SE')
-
-    def set_anchor_south_west(self) -> 'AxesFormatter':
-        """
-        Set the anchor location to the bottom left of the figure.
-        """
-        return self.set_anchor('SW')
-
-    def set_axis_below(self,
-                       value: bool = True) -> 'AxesFormatter':
-        """
-        Set whether axis ticks and gridlines are above or below most artists.
-
-        :param value: True or False
-        """
-        self._axes.set_axisbelow(b=value)
-        return self
-
-    def tight_layout(self) -> 'AxesFormatter':
-        """
-        Call the tight_layout method on the Axes' figure.
-        """
-        self._axes.figure.tight_layout()
-        return self
-
-    def invert_x_axis(self) -> 'AxesFormatter':
-        """
-        Invert the x-axis.
-        """
-        self.x_axis.invert()
-        return self
-
-    def invert_y_axis(self) -> 'AxesFormatter':
-        """
-        Invert the y-axis.
-        """
-        self.y_axis.invert()
-        return self
-
-    def save(self,
-             file_path: Union[str, Path],
-             file_type: Optional[str] = None) -> 'AxesFormatter':
-        """
-        Save the plot to disk.
-
-        :param file_path: The file path to save the plot object to.
-        :param file_type: The type of file to save.
-                          Defaults to png if can't be auto-detected from name.
-        """
-        save_plot(plot_object=self._axes,
-                  file_path=file_path,
-                  file_type=file_type)
-        return self
-
-
-    def add_legend(
-            self,
-            handles: Optional[List[PathCollection]] = None,
-            labels: Optional[List[str]] = None,
-            location: Optional[LegendLocation] = None,
-            n_cols: Optional[int] = None,
-            font_size: Optional[str] = None,
-            font_properties: Optional[Union[FontProperties, dict]] = None,
-            line_points: Optional[int] = None,
-            scatter_points: Optional[int] = None,
-            scatter_y_offsets: Optional[ArrayLike] = None,
-            marker_scale: Optional[float] = None,
-            frame_on: Optional[bool] = None,
-            shadow: Optional[bool] = None,
-            frame_alpha: Optional[float] = None,
-            face_color: Optional[Color] = None,
-            edge_color: Optional[Color] = None,
-            mode: Optional[str] = None,
-            title: Optional[str] = None,
-            title_font_size: Optional[FontSize] = None,
-            label_spacing: Optional[float] = None,
-            handle_length: Optional[float] = None,
-            handle_text_pad: Optional[float] = None,
-            border_axes_pad: Optional[float] = None,
-            column_spacing: Optional[float] = None
-    ) -> LegendFormatter:
-        """
-        Add a legend to the Axes.
-
-        :param handles: A list of Artists (lines, patches) to be added to the
-                        legend.
-        :param labels: A list of labels to show next to the artists. The length
-                       of handles and labels should be the same. If they are
-                       not, they are truncated to the smaller of both lengths.
-        :param location: The legend location.
-        :param n_cols: The number of columns that the legend has. Default is 1.
-        :param font_size: The font size of the legend. If the value is numeric
-                          the size will be the absolute font size in points.
-                          String values are relative to the current default font
-                          size. This argument is only used if font_properties is
-                          not specified.
-        :param font_properties: The font properties of the legend. If None
-                                (default), the current matplotlib.rcParams will
-                                be used.
-        :param line_points: The number of marker points in the legend when
-                            creating a legend entry for a Line2D (line).
-                            Default is None, which means using
-                            rcParams["legend.numpoints"] (default: 1).
-        :param scatter_points: The number of marker points in the legend when
-        creating a legend entry for a PathCollection (scatter plot). Default is
-        None, which means using rcParams["legend.scatterpoints"] (default: 1).
-        :param scatter_y_offsets: The vertical offset (relative to the font
-        size) for the markers created for a scatter plot legend entry. 0.0 is at
-        the base the legend text, and 1.0 is at the top. To draw all markers at
-        the same height, set to [0.5]. Default is [0.375, 0.5, 0.3125].
-        :param marker_scale: The relative size of legend markers compared with
-                             the originally drawn ones. Default is None, which
-                             means using rcParams["legend.markerscale"]
-                             (default: 1.0).
-        :param frame_on: Whether the legend should be drawn on a patch (frame).
-                         Default is None, which means using
-                         rcParams["legend.frameon"] (default: True).
-        :param shadow: Whether to draw a shadow behind the legend. Default is
-                       None, which means using rcParams["legend.shadow"]
-                       (default: False).
-        :param frame_alpha: The alpha transparency of the legend's background.
-                            Default is None, which means using
-                            rcParams["legend.framealpha"] (default: 0.8). If
-                            shadow is activated and framealpha is None, the
-                            default value is ignored.
-        :param face_color: The legend's background color. Default is None, which
-                           means using rcParams["legend.facecolor"]
-                           (default: 'inherit'). If "inherit", use
-                           rcParams["axes.facecolor"] (default: 'white').
-        :param edge_color: The legend's background patch edge color. Default is
-                           None, which means using rcParams["legend.edgecolor"]
-                           (default: '0.8'). If "inherit", use take
-                           rcParams["axes.edgecolor"] (default: 'black').
-        :param mode: If mode is set to "expand" the legend will be horizontally
-                     expanded to fill the axes area (or bbox_to_anchor if
-                     defines the legend's size).
-        :param title: The legend's title. Default is no title (None).
-        :param title_font_size: The fontsize of the legend's title. Default is
-                                the default fontsize.
-        :param label_spacing: The fractional whitespace inside the legend
-        border, in font-size units. Default is None, which means using
-        rcParams["legend.borderpad"] (default: 0.4).
-        :param handle_length: The length of the legend handles, in font-size
-        units. Default is None, which means using
-        rcParams["legend.handlelength"] (default: 2.0).
-        :param handle_text_pad: The pad between the legend handle and text, in
-        font-size units. Default is None, which means using
-        rcParams["legend.handletextpad"] (default: 0.8).
-        :param border_axes_pad: The pad between the axes and legend border, in
-        font-size units. Default is None, which means using
-        rcParams["legend.borderaxespad"] (default: 0.5).
-        :param column_spacing: The spacing between columns, in font-size units.
-        Default is None, which means using rcParams["legend.columnspacing"]
-        (default: 2.0).
-        """
-        kwargs = {}
-        for kwarg, mpl_arg in zip(
-            [handles, labels, n_cols, font_properties, font_size,
-             line_points, scatter_points, scatter_y_offsets, marker_scale,
-             frame_on, shadow, frame_alpha, face_color, edge_color,
-             mode, title, title_font_size, label_spacing, handle_length,
-             handle_text_pad, border_axes_pad, column_spacing, location],
-            ['handles', 'labels', 'ncol', 'prop', 'fontsize',
-             'numpoints', 'scatterpoints', 'scatteryoffsets', 'markerscale',
-             'frameon', 'shadow', 'framealpha', 'facecolor', 'edgecolor',
-             'mode', 'title', 'title_fontsize', 'labelspacing', 'handlelength',
-             'handletextpad', 'borderaxespad', 'columnspacing', 'loc']
-        ):
-            if kwarg is not None:
-                kwargs[mpl_arg] = kwarg
-        self._legend = LegendFormatter(self._axes.legend(**kwargs))
-        return self._legend
-
-    def twin_x(self) -> 'AxesFormatter':
-
-        return AxesFormatter(self.axes.twinx())
-
-    def twin_y(self) -> 'AxesFormatter':
-
-        return AxesFormatter(self.axes.twiny())
-
-    def show(self) -> 'AxesFormatter':
-        """
-        Show the figure for the axes.
-        """
-        plt.show()
-        return self
+from datetime import date
+from math import pi, atan2
+from typing import Optional, Union, List, Tuple, Iterable, TYPE_CHECKING, \
+    Callable
+
+import matplotlib.pyplot as plt
+from mpl_format.compound_types import ArrayLike
+from mpl_format.compound_types import FloatOrFloatIterable, StrOrStrIterable, \
+    DictOrDictIterable, BoolOrBoolIterable, FloatIterable, Scalar, \
+    IntOrIntIterable, NdArrayIterable
+from mpl_format.utils.type_checks import all_are_none, one_is_not_none
+from matplotlib.axes import Axes
+from matplotlib.collections import PathCollection
+from matplotlib.figure import Figure
+from matplotlib.font_manager import FontProperties
+from matplotlib.patches import \
+    Arc, Arrow, BoxStyle, Circle, Ellipse, \
+    FancyArrow, FancyArrowPatch, FancyBboxPatch, \
+    Patch, Polygon, Rectangle, RegularPolygon, Wedge
+from matplotlib.path import Path
+
+from mpl_format.enums.font_size import FONT_SIZE
+from numpy import ndarray, linspace
+from numpy.ma import cos, sin
+from pandas import DataFrame, Series
+from scipy.interpolate import interp1d
+
+from mpl_format.axes.axis_formatter import AxisFormatter
+from mpl_format.axes.axis_utils import new_axes
+from mpl_format.axes.ticks_formatter import TicksFormatter
+from mpl_format.compound_types import FontSize, Color, LegendLocation, \
+    StringMapper, ColorOrColorIterable, FontStretch, FontWeight, \
+    FontSizeIterable, FontStretchIterable, FontStyle, FontStyleIterable, \
+    FontVariant, FontVariantIterable, CapStyle, CapStyleIterable, \
+    JoinStyleIterable, JoinStyle, LineStyleIterable, LineStyle, \
+    ArrowStyleIterable, ArrowStyle, ConnectionStyleIterable, ConnectionStyle, \
+    PathIterable, PatchIterable, BoxStyleTypeIterable
+from mpl_format.enums.box_style import BOX_STYLE, BoxStyleType
+from mpl_format.enums.cap_style import CAP_STYLE
+from mpl_format.enums.connection_style import CONNECTION_STYLE
+from mpl_format.enums.draw_style import DRAW_STYLE
+from mpl_format.enums.font_weight import FONT_WEIGHT
+from mpl_format.enums.line_style import LINE_STYLE
+from mpl_format.enums.mappings import kwarg_mappings
+from mpl_format.enums.marker_style import MARKER_STYLE
+from mpl_format.legend.legend_formatter import LegendFormatter
+from mpl_format.literals import H_ALIGN, V_ALIGN, ROTATION_MODE, WHICH_TICKS, \
+    FIGURE_UNITS, WHICH_AXIS, LINE_STYLE_STR, ASPECT, ANCHOR
+from mpl_format.patches.patch_list_formatter import PatchListFormatter
+from mpl_format.text.text_formatter import TextFormatter
+from mpl_format.text.text_utils import wrap_text
+from mpl_format.utils.arg_checks import check_h_align, check_v_align
+from mpl_format.utils.arg_transforms import smart_zip_kwargs, \
+    drop_none_values, apply_mappings
+from mpl_format.utils.color_utils import cross_fade
+from mpl_format.utils.io_utils import save_plot
+
+if TYPE_CHECKING:
+    from mpl_format.figures.figure_formatter import FigureFormatter
+
+
+class AxesFormatter(object):
+
+    def __init__(self, axes: Optional[Axes] = None,
+                 width: Optional[Scalar] = None,
+                 height: Optional[Scalar] = None,
+                 constrained_layout: bool = False):
+        """
+        Create a new AxesFormatter
+
+        :param axes: The matplotlib Axes instance to wrap.
+        :param width: Width of new Axes, if none are given.
+        :param height: Height of new Axes, if none are given.
+        :param constrained_layout: Option for constrained_layout of new Axes.
+        """
+        if axes is None:
+            self._axes: Axes = new_axes(
+                width=width, height=height,
+                constrained_layout=constrained_layout
+            )
+        else:
+            self._axes: Axes = axes
+        self._x_axis: AxisFormatter = AxisFormatter(
+            axis=self._axes.xaxis, direction='x', axes=self._axes
+        )
+        self._y_axis: AxisFormatter = AxisFormatter(
+            axis=self._axes.yaxis, direction='y', axes=self._axes
+        )
+        self._title: TextFormatter = TextFormatter(self._axes.title)
+        legend = self._axes.get_legend()
+        if legend is None:
+            self._legend = None
+        else:
+            self._legend = LegendFormatter(legend)
+        self._ticks: TicksFormatter = TicksFormatter(
+            axis='both', which='both', axes=self._axes)
+        self._major_ticks: TicksFormatter = TicksFormatter(
+            axis='both', which='major', axes=self._axes)
+        self._minor_ticks: TicksFormatter = TicksFormatter(
+            axis='both', which='minor', axes=self._axes)
+        self._x_ticks: TicksFormatter = TicksFormatter(
+            axis='x', which='both', axes=self._axes)
+        self._x_major_ticks: TicksFormatter = TicksFormatter(
+            axis='x', which='major', axes=self._axes)
+        self._x_minor_ticks: TicksFormatter = TicksFormatter(
+            axis='x', which='minor', axes=self._axes)
+        self._y_ticks: TicksFormatter = TicksFormatter(
+            axis='y', which='both', axes=self._axes)
+        self._y_major_ticks: TicksFormatter = TicksFormatter(
+            axis='y', which='major', axes=self._axes)
+        self._y_minor_ticks = TicksFormatter(
+            axis='y', which='minor', axes=self._axes)
+
+    @staticmethod
+    def gca() -> 'AxesFormatter':
+
+        return AxesFormatter(axes=plt.gca())
+
+    @staticmethod
+    def find_in_figure(
+            figure: Figure,
+            match: Callable[['AxesFormatter'], bool]
+    ):
+        """
+        Return and AxesFormatter matching the first Axes in the instance where
+        an AxesFormatter wrapping the Axes matches the lambda function.
+
+        :param figure: Figure e.g. plt.gcf()
+        :param match: Method that return True for the matching Axes.
+        """
+        for axes in figure.axes:
+            axf = AxesFormatter(axes)
+            if match(axf):
+                return axf
+        raise ValueError('No matching Axes')
+
+    # region properties
+
+    @property
+    def axes(self) -> Axes:
+        """
+        Return the wrapped Axes instance.
+        """
+        return self._axes
+
+    @property
+    def x_axis(self) -> AxisFormatter:
+        """
+        Return an AxisFormatter for the x-axis of the wrapped Axes.
+        """
+        return self._x_axis
+
+    @property
+    def y_axis(self) -> AxisFormatter:
+        """
+        Return an AxisFormatter for the y-axis of the wrapped Axes.
+        """
+        return self._y_axis
+
+    @property
+    def legend(self) -> LegendFormatter:
+        """
+        Return a LegendFormatter for the legend of the wrapped Axes,
+        if there is one.
+        """
+        return self._legend
+
+    @property
+    def title(self) -> TextFormatter:
+        return self._title
+
+    @property
+    def figure(self) -> 'FigureFormatter':
+
+        from mpl_format.figures.figure_formatter import FigureFormatter
+        return FigureFormatter(self._axes)
+
+    @property
+    def ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the ticks on both axes.
+        """
+        return self._ticks
+    
+    @property
+    def x_ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the ticks on the x-axis.
+        """
+        return self._x_ticks
+
+    @property
+    def y_ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the ticks on the y-axis.
+        """
+        return self._y_ticks
+
+    @property
+    def major_ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the major ticks on both axes.
+        """
+        return self._major_ticks
+
+    @property
+    def x_major_ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the major ticks on the x-axis.
+        """
+        return self._x_major_ticks
+
+    @property
+    def y_major_ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the major ticks on the y-axis.
+        """
+        return self._y_major_ticks
+
+    @property
+    def minor_ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the minor ticks on both axes.
+        """
+        return self._minor_ticks
+
+    @property
+    def x_minor_ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the minor ticks on the x-axis.
+        """
+        return self._x_minor_ticks
+
+    @property
+    def y_minor_ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the minor ticks on the y-axis.
+        """
+        return self._y_minor_ticks
+    
+    # endregion
+
+    # region set text
+
+    def set_title_text(self, text: str) -> 'AxesFormatter':
+        """
+        Set the text of the Axes title.
+
+        :param text: The text to use for the Axes title.
+        """
+        self.title.set_text(text)
+        return self
+
+    def map_title_text(
+            self, mapping: StringMapper
+    ) -> 'AxesFormatter':
+        """
+        Map the label text for the title using a dictionary or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        self.title.map(mapping=mapping)
+        return self
+
+    def get_x_label_text(self) -> str:
+
+        return self.x_axis.get_label_text()
+
+    def set_x_label_text(self, text: str) -> 'AxesFormatter':
+        """
+        Set the text for the x-axis label.
+
+        :param text: The text to use for the Axis label.
+        """
+        self.x_axis.set_label_text(text)
+        return self
+
+    def get_y_label_text(self) -> str:
+
+        return self.y_axis.get_label_text()
+
+    def set_y_label_text(self, text: str) -> 'AxesFormatter':
+        """
+        Set the text for the y-axis label.
+
+        :param text: The text to use for the Axis label.
+        """
+        self.y_axis.set_label_text(text)
+        return self
+
+    def set_text(self, title: Optional[str] = None,
+                 x_label: Optional[str] = None,
+                 y_label: Optional[str] = None) -> 'AxesFormatter':
+        """
+        Set text properties for elements of the Axes.
+
+        :param title: Text for the title.
+        :param x_label: Text for the x-axis label.
+        :param y_label: Text for the y-axis label.
+        """
+        if title is not None:
+            self.set_title_text(title)
+        if x_label is not None:
+            self.x_axis.set_label_text(x_label)
+        if y_label is not None:
+            self.y_axis.set_label_text(y_label)
+        return self
+
+    # endregion
+
+    # region wrap text
+
+    def wrap_title(self, max_width: int) -> 'AxesFormatter':
+        """
+        Wrap the text for the title if it exceeds a given width of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        self.set_title_text(wrap_text(self.title.text, max_width=max_width))
+        return self
+
+    def wrap_x_label(self, max_width: int) -> 'AxesFormatter':
+        """
+        Wrap the text for the x-axis label if it exceeds a given width of
+        characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        self.x_axis.wrap_label(max_width=max_width)
+        return self
+
+    def wrap_y_label(self, max_width: int) -> 'AxesFormatter':
+        """
+        Wrap the text for the y-axis label if it exceeds a given width of
+        characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        self.y_axis.wrap_label(max_width=max_width)
+        return self
+
+    def wrap_axis_labels(self, max_width: int) -> 'AxesFormatter':
+        """
+        Wrap the texts for the x and y-axis labels if they exceeds a given width
+        of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        self.wrap_x_label(max_width=max_width)
+        self.wrap_y_label(max_width=max_width)
+        return self
+
+    # endregion
+
+    # region set font sizes
+
+    def _get_font_size(self, font_size: FontSize):
+
+        if isinstance(font_size, FONT_SIZE):
+            return font_size.get_name()
+        else:
+            return font_size
+
+    def set_title_size(self, font_size: FontSize) -> 'AxesFormatter':
+        """
+        Set the font size for the title of the wrapped Axes.
+
+        :param font_size: Size of the font in points, or size name.
+        """
+        self.title.set_size(self._get_font_size(font_size))
+        return self
+
+    def set_x_label_size(self, font_size: FontSize) -> 'AxesFormatter':
+        """
+        Set the font size for the x-axis label.
+
+        :param font_size: Size of the font in points, or size name.
+        """
+        self.x_axis.set_label_size(self._get_font_size(font_size))
+        return self
+
+    def set_y_label_size(self, font_size: FontSize) -> 'AxesFormatter':
+        """
+        Set the font size for the x-axis label.
+
+        :param font_size: Size of the font in points, or size name.
+        """
+        self.y_axis.set_label_size(self._get_font_size(font_size))
+        return self
+
+    def set_axis_label_sizes(self, font_size: FontSize) -> 'AxesFormatter':
+        """
+        Set the font size for the axis labels.
+
+        :param font_size: Size of the font in points, or size name.
+        """
+        self.set_x_label_size(font_size)
+        self.set_y_label_size(font_size)
+        return self
+
+    def set_font_sizes(
+            self,
+            title: Optional[FontSize] = None,
+            axis_labels: Optional[FontSize] = None,
+            tick_labels: Optional[FontSize] = None,
+            legend: Optional[FontSize] = None,
+            figure_title: Optional[FontSize] = None,
+            x_axis_label: Optional[FontSize] = None,
+            y_axis_label: Optional[FontSize] = None,
+            major_tick_labels: Optional[FontSize] = None,
+            minor_tick_labels: Optional[FontSize] = None,
+            x_tick_labels: Optional[FontSize] = None,
+            x_major_tick_labels: Optional[FontSize] = None,
+            x_minor_tick_labels: Optional[FontSize] = None,
+            y_tick_labels: Optional[FontSize] = None,
+            y_major_tick_labels: Optional[FontSize] = None,
+            y_minor_tick_labels: Optional[FontSize] = None,
+    ) -> 'AxesFormatter':
+        """
+        Set font sizes for different axes elements.
+        """
+        ax = self._axes
+        # title
+        if title is not None:
+            self.set_title_size(title)
+        # axis labels
+        if axis_labels is not None:
+            self.set_axis_label_sizes(axis_labels)
+        if x_axis_label is not None:
+            self.set_x_label_size(x_axis_label)
+        if y_axis_label is not None:
+            self.set_y_label_size(y_axis_label)
+        # tick labels
+        if tick_labels is not None:
+            self.ticks.set_label_size(tick_labels)
+        if major_tick_labels is not None:
+            self.major_ticks.set_label_size(major_tick_labels)
+        if minor_tick_labels is not None:
+            self.minor_ticks.set_label_size(minor_tick_labels)
+        if x_tick_labels is not None:
+            self.x_ticks.set_label_size(tick_labels)
+        if x_major_tick_labels is not None:
+            self.x_major_ticks.set_label_size(x_major_tick_labels)
+        if x_minor_tick_labels is not None:
+            self.x_minor_ticks.set_label_size(x_minor_tick_labels)
+        if y_tick_labels is not None:
+            self.y_ticks.set_label_size(tick_labels)
+        if y_major_tick_labels is not None:
+            self.y_major_ticks.set_label_size(y_major_tick_labels)
+        if y_minor_tick_labels is not None:
+            self.y_minor_ticks.set_label_size(y_major_tick_labels)
+        if legend is not None:
+            if isinstance(legend, FONT_SIZE):
+                legend = legend.get_name()
+            ax.legend(fontsize=legend)
+        if figure_title is not None:
+            if isinstance(figure_title, FONT_SIZE):
+                figure_title = figure_title.get_name()
+            ax.figure.suptitle(ax.get_title(), fontsize=figure_title)
+
+        return self
+
+    # endregion
+
+    # region map labels
+
+    def map_x_axis_label(
+            self, mapping: StringMapper
+    ) -> 'AxesFormatter':
+        """
+        Map the label text for the x-axis using a dictionary or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        self.x_axis.map_label_text(mapping)
+        return self
+
+    def map_y_axis_label(
+            self, mapping: StringMapper
+    ) -> 'AxesFormatter':
+        """
+        Map the label text for the y-axis using a dictionary or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        self.y_axis.map_label_text(mapping)
+        return self
+
+    def map_axis_labels(
+            self, mapping: StringMapper
+    ) -> 'AxesFormatter':
+        """
+        Map the label text for the x and y axes using a dictionary or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        self.map_x_axis_label(mapping)
+        self.map_y_axis_label(mapping)
+        return self
+
+    # endregion
+
+    # region remove
+
+    def remove_title(self) -> 'AxesFormatter':
+        """
+        Remove the title from the Axes.
+        """
+        self.set_title_text('')
+        return self
+
+    def remove_legend(self) -> 'AxesFormatter':
+        """
+        Remove the legend from the Axes.
+        """
+        legend = self._axes.get_legend()
+        if legend is not None:
+            legend.remove()
+            self._legend = None
+        return self
+
+    def remove_x_ticks(self) -> 'AxesFormatter':
+        """
+        Remove x-ticks from the Axes.
+        """
+        self._axes.set_xticks([])
+        return self
+
+    def remove_y_ticks(self) -> 'AxesFormatter':
+        """
+        Remove y-ticks from the Axes.
+        """
+        self._axes.set_yticks([])
+        return self
+
+    def remove_axes_ticks(self) -> 'AxesFormatter':
+        """
+        Remove x- and y- ticks from the Axes.
+        """
+        self.remove_x_ticks()
+        self.remove_y_ticks()
+        return self
+
+    def remove_x_label(self) -> 'AxesFormatter':
+        """
+        Remove the label from the x-axis.
+        """
+        self.x_axis.remove_label()
+        return self
+
+    def remove_y_label(self) -> 'AxesFormatter':
+        """
+        Remove the label from the y-axis.
+        """
+        self.y_axis.remove_label()
+        return self
+
+    def remove_axes_labels(self) -> 'AxesFormatter':
+        """
+        Remove the labels from the x- and y- axes.
+        """
+        self.remove_x_label()
+        self.remove_y_label()
+        return self
+
+    # endregion
+
+    # region rotation
+
+    def rotate_x_label(self,
+                       rotation: int,
+                       how: ROTATION_MODE = 'absolute') -> 'AxesFormatter':
+        """
+        Set the rotation of the x-axis label.
+
+        :param rotation: The rotation value to set in degrees.
+        :param how: 'absolute' or 'relative'
+        """
+        self.x_axis.rotate_label(rotation, how)
+        return self
+
+    def rotate_y_label(self,
+                       rotation: int,
+                       how: ROTATION_MODE = 'absolute') -> 'AxesFormatter':
+        """
+        Set the rotation of the x-axis label.
+
+        :param rotation: The rotation value to set in degrees.
+        :param how: 'absolute' or 'relative'
+        """
+        self.y_axis.rotate_label(rotation, how)
+        return self
+
+    # endregion
+
+    # region spans
+
+    def add_h_line(self, y: Union[float, str, date] = 0,
+                   x_min: Union[float, str] = 0,
+                   x_max: Union[float, str] = 1,
+                   color: Optional[Color] = None,
+                   alpha: Optional[float] = None,
+                   line_style: Optional[LineStyle] = None,
+                   line_width: Optional[float] = None,
+                   label: Optional[str] = None,
+                   marker_edge_color: Optional[Color] = None,
+                   marker_edge_width: Optional[Color] = None,
+                   marker_face_color: Optional[Color] = None,
+                   marker_size: Optional[float] = None) -> 'AxesFormatter':
+        """
+        Add a horizontal line to the plot.
+
+        :param y: y position in data coordinates of the horizontal line
+        :param x_min: Between 0 and 1, 0 being the far left of the plot,
+                      1 the far right of the plot
+        :param x_max: Between 0 and 1, 0 being the far left of the plot,
+                      1 the far right of the plot
+        :param color: Color of the line
+        :param alpha: Opacity of the line
+        :param line_style: One of {'-', '--', '-.', ':', ''}
+        :param line_width: Width of the line
+        :param label: Text for the label
+        :param marker_edge_color: Color for the edges of the line markers
+        :param marker_edge_width: Width for the edges of the line markers
+        :param marker_face_color: Color for the markers
+        :param marker_size: Size of the markers.
+        """
+        line_style = LINE_STYLE.get_line_style(line_style)
+        kwargs = {}
+        for arg, mpl_arg in zip(
+            [color, line_style, line_width,
+             marker_edge_color, marker_edge_width,
+             marker_face_color, marker_size,
+             alpha, label],
+            ['c', 'ls', 'lw', 'mec', 'mew', 'mfc', 'ms', 'alpha', 'label']
+        ):
+            if arg is not None:
+                kwargs[mpl_arg] = arg
+
+        self._axes.axhline(
+            y=y, xmin=x_min, xmax=x_max,
+            **kwargs
+        )
+        return self
+
+    def add_v_line(self, x: Union[float, str, date] = 0,
+                   y_min: Union[float, str] = 0,
+                   y_max: Union[float, str] = 1,
+                   color: Optional[Color] = None, alpha: Optional[float] = None,
+                   line_style: Optional[Union[
+                       LineStyle, LineStyleIterable]] = None,
+                   line_width: Optional[float] = None,
+                   label: Optional[str] = None,
+                   marker_edge_color: Optional[Color] = None,
+                   marker_edge_width: Optional[Color] = None,
+                   marker_face_color: Optional[Color] = None,
+                   marker_size: Optional[float] = None) -> 'AxesFormatter':
+        """
+        Add a vertical line to the plot.
+
+        :param x: x position in data coordinates of the vertical line
+        :param y_min: Should be between 0 and 1, with 0 being the bottom of the
+                      plot, and 1 the top of the plot
+        :param y_max: Should be between 0 and 1, with 0 being the bottom of the
+                      plot, and 1 the top of the plot
+        :param color: Color of the line
+        :param alpha: Opacity of the line
+        :param line_style: One of {'-', '--', '-.', ':', ''}
+        :param line_width: Width of the line
+        :param label: Text for the label
+        :param marker_edge_color: Color for the edges of the line markers
+        :param marker_edge_width: Width for the edges of the line markers
+        :param marker_face_color: Color for the markers
+        :param marker_size: Size of the markers.
+        """
+        line_style = LINE_STYLE.get_line_style(line_style)
+        kwargs = {}
+        for arg, mpl_arg in zip(
+            [color, line_style, line_width, marker_edge_color,
+             marker_edge_width, marker_face_color, marker_size,
+             alpha, label],
+            ['c', 'ls', 'lw', 'mec',
+             'mew', 'mfc', 'ms',
+             'alpha', 'label']
+        ):
+            if arg is not None:
+                kwargs[mpl_arg] = arg
+
+        self._axes.axvline(
+            x=x, ymin=y_min, ymax=y_max,
+            **kwargs
+        )
+        return self
+
+    def add_h_lines(self, y: FloatOrFloatIterable,
+                    x_min: FloatOrFloatIterable,
+                    x_max: FloatOrFloatIterable,
+                    colors='k',
+                    line_styles: LINE_STYLE_STR = 'solid',
+                    label: Optional[str] = '') -> 'AxesFormatter':
+        """
+        Plot horizontal lines at each y from x_min to x_max.
+
+        :param y: x-indexes where to plot the lines.
+        :param x_min: Beginning of each or all lines.
+        :param x_max: End of each or all lines.
+        :param colors: Line colors.
+        :param line_styles: One of {'solid', 'dashed', 'dashdot', 'dotted'}
+        :param label: Label.
+        """
+        self._axes.hlines(y=y, xmin=x_min, xmax=x_max,
+                          colors=colors, linestyles=line_styles,
+                          label=label)
+        return self
+
+    def add_v_lines(self, x: FloatOrFloatIterable,
+                    y_min: FloatOrFloatIterable,
+                    y_max: FloatOrFloatIterable,
+                    colors='k',
+                    line_styles: LINE_STYLE_STR = 'solid',
+                    label: Optional[str] = '') -> 'AxesFormatter':
+        """
+        Plot vertical lines at each x from y_min to y_max.
+
+        :param x: x-indexes where to plot the lines.
+        :param y_min: Beginning of each or all lines.
+        :param y_max: End of each or all lines.
+        :param colors: Line colors.
+        :param line_styles: One of {'solid', 'dashed', 'dashdot', 'dotted'}
+        :param label: Label.
+        """
+        self._axes.vlines(x=x, ymin=y_min, ymax=y_max,
+                          colors=colors, linestyles=line_styles,
+                          label=label)
+        return self
+
+    def fill_between(self, x: Union[ArrayLike, str],
+                     y1: Union[float, ArrayLike, str],
+                     y2: Union[float, ArrayLike, str],
+                     data: Optional[DataFrame] = None,
+                     where: Optional[ArrayLike] = None,
+                     interpolate: bool = False,
+                     step: Optional[str] = None,
+                     color: Optional[Color] = None,
+                     alpha: Optional[float] = None,
+                     line_style: Optional[LineStyle] = None,
+                     line_width: Optional[float] = None,
+                     edge_color: Optional[Color] = None,
+                     face_color: Optional[Color] = None) -> 'AxesFormatter':
+        """
+        Make filled polygons between two curves.
+
+        :param x: N-length array of, or name of column with the x data.
+        :param y1: N-length array, scalar, or name of column with the y1 data.
+        :param y2: N-length array, scalar, or name of column with the y2 data.
+        :param data: Optional DataFrame with x, y1 and y2 columns.
+        :param where: If None, default to fill between everywhere. If not None,
+                      it is an N-length numpy boolean array and the fill will
+                      only happen over the regions where where==True.
+        :param interpolate: If True, interpolate between the two lines to find
+                            the precise point of intersection. Otherwise, the
+                            start and end points of the filled region will only
+                            occur on explicit values in the x array.
+        :param step: One of {‘pre’, ‘post’, ‘mid’}. If not None, fill with step
+                     logic.
+        :param color: matplotlib color arg or sequence of rgba tuples
+        :param alpha: Opacity.
+        :param line_style: One of {'-', '--', '-.', ':', ''}
+        :param line_width: float or sequence of floats
+        :param edge_color: matplotlib color spec or sequence of specs
+        :param face_color: matplotlib color spec or sequence of specs
+        """
+        line_style = LINE_STYLE.get_line_style(line_style)
+        # get arrays from DataFrame
+        if data is not None:
+            if isinstance(x, str):
+                x = data[x]
+            if isinstance(y1, str):
+                y1 = data[y1]
+            if isinstance(y2, str):
+                y2 = data[y2]
+        # convert args to matplotlib names
+        kwargs = {}
+        for arg, mpl_arg in zip(
+            [color, alpha, line_style, line_width, edge_color, face_color],
+            ['color', 'alpha', 'line_style',
+             'line_width', 'edge_color', 'face_color']
+        ):
+            if arg is not None:
+                kwargs[mpl_arg] = arg
+        # call matplotlib method
+        self._axes.fill_between(
+            x=x, y1=y1, y2=y2,
+            where=where, interpolate=interpolate,
+            step=step,
+            **kwargs
+        )
+        return self
+
+    # endregion
+
+    # region colors
+
+    def set_face_color(self, color: Color) -> 'AxesFormatter':
+
+        self._axes.set_facecolor(color)
+        return self
+
+    def get_frame_color(self) -> Union[Color, List[Color]]:
+        """
+        Return the color of the frame if all edges are the same color,
+        otherwise a list of the top, bottom, left and right colors.
+        """
+        colors = self.get_frame_colors()
+        if len(set(colors)) == 1:
+            return colors[0]
+        else:
+            return self.get_frame_colors()
+
+    def set_frame_color(self, color: Color) -> 'AxesFormatter':
+
+        for pos in ['top', 'bottom', 'left', 'right']:
+            self._axes.spines[pos].set_edgecolor(color)
+        return self
+
+    def get_frame_colors(self) -> List[Color]:
+        """
+        Return the colors of the top, bottom, left and right edges of the Axes.
+        """
+        return [
+            self._axes.spines[pos].get_edgecolor()
+            for pos in ['top', 'bottom', 'left', 'right']
+        ]
+
+    # endregion
+
+    # region shapes
+
+    # region patches
+
+    def add_text(
+            self,
+            x: Union[FloatOrFloatIterable, date, Iterable[date]],
+            y: Union[FloatOrFloatIterable, date, Iterable[date]],
+            text: StrOrStrIterable,
+            max_width: Optional[IntOrIntIterable] = None,
+            font_dict: Optional[DictOrDictIterable] = None,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            h_align: Optional[StrOrStrIterable] = None,
+            v_align: Optional[StrOrStrIterable] = None,
+            m_align: Optional[StrOrStrIterable] = None,
+            rotation: Optional[
+                Union[IntOrIntIterable, StrOrStrIterable]] = None,
+            rotation_mode: Optional[StrOrStrIterable] = None,
+            line_spacing: Optional[FloatOrFloatIterable] = None,
+            font_family: Optional[StrOrStrIterable] = None,
+            font_size: Optional[Union[FontSize, FontSizeIterable]] = None,
+            font_stretch: Optional[
+                Union[FontStretch, FontStretchIterable]] = None,
+            font_style: Optional[Union[FontStyle, FontStyleIterable]] = None,
+            font_variant: Optional[
+                Union[FontVariant, FontVariantIterable]] = None,
+            font_weight: Optional[Union[FontWeight, FONT_WEIGHT]] = None,
+            wrap: Optional[BoolOrBoolIterable] = None,
+            bbox_style: Optional[StrOrStrIterable] = None,
+            bbox_alpha: Optional[FloatOrFloatIterable] = None,
+            bbox_cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            bbox_color: Optional[ColorOrColorIterable] = None,
+            bbox_edge_color: Optional[ColorOrColorIterable] = None,
+            bbox_face_color: Optional[ColorOrColorIterable] = None,
+            bbox_fill: Optional[BoolOrBoolIterable] = None,
+            bbox_join_style: Optional[
+                Union[JoinStyle, JoinStyleIterable]] = None,
+            bbox_line_style: Optional[
+                Union[LineStyle, LineStyleIterable]] = None,
+            bbox_line_width: Optional[FloatOrFloatIterable] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a single or multiple text blocks to the plot.
+
+        :param x: x-coordinate(s) of the text.
+        :param y: y-coordinate(s) of the text.
+        :param text: String or iterable of text strings to add.
+        :param max_width: Max number of characters to wrap lines at.
+        :param font_dict: A dictionary to override the default text properties.
+                          If font_dict is None, the defaults are determined by
+                          your rc parameters.
+        :param alpha: Text opacity.
+        :param color: Text color.
+        :param h_align: Horizontal alignment.
+        :param v_align: Vertical alignment.
+        :param m_align: Multi-line alignment.
+        :param rotation: float or {'vertical', 'horizontal'}
+        :param rotation_mode: {None, 'default', 'anchor'}
+        :param line_spacing:
+        :param font_family:
+        :param font_size: float or {'xx-small', 'x-small', 'small', 'medium',
+                                    'large', 'x-large', 'xx-large'}
+        :param font_stretch: {a numeric value in range 0-1000,
+                             'ultra-condensed', 'extra-condensed', 'condensed',
+                             'semi-condensed', 'normal', 'semi-expanded',
+                             'expanded', 'extra-expanded', 'ultra-expanded'}
+        :param font_style: {'normal', 'italic', 'oblique'}
+        :param font_variant: {'normal', 'small-caps'}
+        :param font_weight: {a numeric value in range 0-1000, 'ultralight',
+                             'light', 'normal', 'regular', 'book', 'medium',
+                             'roman', 'semibold', 'demibold', 'demi', 'bold',
+                             'heavy', 'extra bold', 'black'}
+        :param wrap: Set whether the text can be wrapped.
+        :param bbox_alpha: Opacity.
+        :param bbox_style: Box style.
+        :param bbox_cap_style: Cap style.
+        :param bbox_color: Use to set both the edge-color and the face-color.
+        :param bbox_edge_color: Edge color.
+        :param bbox_face_color: Face color.
+        :param bbox_fill: Whether to fill the rectangle.
+        :param bbox_join_style: Join style.
+        :param bbox_line_style: Line style for edge.
+        :param bbox_line_width: Line width for edge.
+        :param z_order: z-order for the text.
+        """
+        for kwargs in smart_zip_kwargs(
+                x=x, y=y, s=text,
+                fontdict=font_dict, max_width=max_width,
+                alpha=alpha, color=color,
+                ha=h_align, va=v_align, ma=m_align,
+                rotation=rotation, rotation_mode=rotation_mode,
+                linespacing=line_spacing,
+                fontfamily=font_family, fontsize=font_size,
+                fontstretch=font_stretch, fontstyle=font_style,
+                fontvariant=font_variant, fontweight=font_weight,
+                wrap=wrap, zorder=z_order,
+                bbox__boxstyle=bbox_style, bbox__alpha=bbox_alpha,
+                bbox__capstyle=bbox_cap_style, bbox__color=bbox_color,
+                bbox__edgecolor=bbox_edge_color,
+                bbox__facecolor=bbox_face_color,
+                bbox__fill=bbox_fill, bbox__joinstyle=bbox_join_style,
+                bbox__linestyle=bbox_line_style, bbox__linewidth=bbox_line_width
+        ):
+            # main kwargs
+            kwargs = drop_none_values(kwargs)
+            kwargs = apply_mappings(kwargs, kwarg_mappings)
+            # bbox kwargs
+            bbox_kwargs = {}
+            for kw, arg in kwargs.items():
+                if kw.startswith('bbox__'):
+                    bbox_kwargs[kw[6:]] = arg
+            kwargs = {kw: arg for kw, arg in kwargs.items()
+                      if not kw.startswith('bbox__')}
+            if bbox_kwargs:
+                bbox_kwargs = apply_mappings(bbox_kwargs, kwarg_mappings)
+                kwargs['bbox'] = bbox_kwargs
+            # max width
+            mw = kwargs.pop('max_width', None)
+            if mw is not None:
+                kwargs['s'] = wrap_text(text=kwargs['s'], max_width=mw)
+            # add text
+            self._axes.text(**drop_none_values(kwargs))
+
+        return self
+
+    def add_arc(
+            self,
+            x_center: FloatOrFloatIterable,
+            y_center: FloatOrFloatIterable,
+            width: FloatOrFloatIterable,
+            height: FloatOrFloatIterable,
+            angle: FloatOrFloatIterable = 0.0,
+            theta_start: FloatOrFloatIterable = 0.0,
+            theta_end: FloatOrFloatIterable = 360.0,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
+            label: Optional[StrOrStrIterable] = None,
+            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ):
+        """
+        Add an elliptical arc, i.e. a segment of an ellipse.
+
+        :param x_center: The x-coordinate of the center of the ellipse.
+        :param y_center: The y-coordinate of the center of the ellipse.
+        :param width: The length of the horizontal axis.
+        :param height: The length of the vertical axis.
+        :param angle: Rotation of the ellipse in degrees (counterclockwise).
+        :param theta_start: Starting angle of the arc in degrees.
+                            Relative to angle, e.g. if angle = 45 and
+                            theta_start = 90 the absolute starting angle is 135.
+        :param theta_end: Ending angle of the arc in degrees.
+        :param alpha: Opacity.
+        :param cap_style: Cap style.
+        :param color: Use to set both the edge-color and the face-color.
+        :param edge_color: Edge color.
+        :param join_style: Join style.
+        :param label: Label for the object in the legend.
+        :param line_style: Line style for edge.
+        :param line_width: Line width for edge.
+        :param z_order: z-order for the arc.
+        """
+        for kwargs in smart_zip_kwargs(
+            x_center=x_center, y_center=y_center,
+            width=width, height=height, angle=angle,
+            theta1=theta_start, theta2=theta_end,
+            alpha=alpha, capstyle=cap_style, color=color, edgecolor=edge_color,
+            joinstyle=join_style, label=label,
+            linestyle=line_style, linewidth=line_width, zorder=z_order
+        ):
+            kwargs = drop_none_values(kwargs)
+            kwargs['xy'] = kwargs.pop('x_center'), kwargs.pop('y_center')
+            arc = Arc(**kwargs)
+            self._axes.add_artist(arc)
+
+        return self
+
+    def add_arrow(
+            self,
+            x_tail: FloatOrFloatIterable,
+            y_tail: FloatOrFloatIterable,
+            x_head: Optional[FloatOrFloatIterable] = None,
+            y_head: Optional[FloatOrFloatIterable] = None,
+            dx: Optional[FloatOrFloatIterable] = None,
+            dy: Optional[FloatOrFloatIterable] = None,
+            width: Optional[FloatOrFloatIterable] = None,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
+            label: StrOrStrIterable = None,
+            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ):
+        """
+        Add an an arrow patch.
+
+        :param x_tail: The x-coordinate of the arrow tail.
+        :param y_tail: The y-coordinate of the arrow tail.
+        :param x_head: The x-coordinate of the arrow head.
+        :param y_head: The y-coordinate of the arrow head.
+        :param dx: Arrow length in the x direction. Only used if x_head is None.
+        :param dy: Arrow length in the y direction. Only used if y_head is None.
+        :param width: Width of full arrow tail. default: 0.001
+        :param alpha: Opacity.
+        :param cap_style: Cap style.
+        :param color: Use to set both the edge-color and the face-color.
+        :param edge_color: Edge color.
+        :param face_color: Face color.
+        :param fill: Whether to fill the rectangle.
+        :param join_style: Join style.
+        :param label: Label for the object in the legend.
+        :param line_style: Line style for edge.
+        :param line_width: Line width for edge.
+        :param z_order: z-order for the arrow.
+        """
+        if not one_is_not_none(dx, x_head):
+            raise ValueError('Must give dx or x_head')
+        if not one_is_not_none(dy, y_head):
+            raise ValueError('Must give dy or y_head')
+        for kwargs in smart_zip_kwargs(
+                x=x_tail, y=y_tail, x_head=x_head, y_head=y_head,
+                dx=dx, dy=dy, width=width,
+                alpha=alpha, capstyle=cap_style,
+                color=color, edgecolor=edge_color, facecolor=face_color,
+                fill=fill, joinstyle=join_style, label=label,
+                linestyle=line_style, linewidth=line_width,
+                zorder=z_order
+        ):
+            kwargs = drop_none_values(kwargs)
+            kwargs = apply_mappings(kwargs, kwarg_mappings)
+            if kwargs['x_head'] is not None:
+                kwargs['dx'] = kwargs['x_head'] - kwargs['x']
+                kwargs.pop('x_head')
+            if kwargs['y_head'] is not None:
+                kwargs['dy'] = kwargs['y_head'] - kwargs['y']
+                kwargs.pop('y_head')
+            arrow = Arrow(**kwargs)
+            self._axes.add_artist(arrow)
+
+        return self
+
+    def add_circle(
+            self,
+            x_center: FloatOrFloatIterable,
+            y_center: FloatOrFloatIterable,
+            radius: FloatOrFloatIterable,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            label: Optional[StrOrStrIterable] = None,
+            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None,
+            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a rectangle to the Axes.
+
+        :param x_center: The left rectangle coordinate.
+        :param y_center: The bottom rectangle coordinate.
+        :param radius: The radius of the circle.
+        :param alpha: Opacity.
+        :param color: Use to set both the edge-color and the face-color.
+        :param edge_color: Edge color.
+        :param face_color: Face color.
+        :param fill: Whether to fill the rectangle.
+        :param join_style: Join style.
+        :param label: Label for the object in the legend.
+        :param line_style: Line style for edge.
+        :param line_width: Line width for edge.
+        :param cap_style: Cap style.
+        :param z_order: z-order for the circle.
+        """
+        for kwargs in smart_zip_kwargs(
+                x_center=x_center, y_center=y_center, radius=radius,
+                alpha=alpha, capstyle=cap_style,
+                color=color, edgecolor=edge_color, facecolor=face_color,
+                fill=fill, joinstyle=join_style, label=label,
+                linestyle=line_style, linewidth=line_width,
+                zorder=z_order
+        ):
+            kwargs = drop_none_values(kwargs)
+            kwargs = apply_mappings(kwargs, kwarg_mappings)
+            kwargs['xy'] = kwargs.pop('x_center'), kwargs.pop('y_center')
+            circle = Circle(**kwargs)
+            self._axes.add_artist(circle)
+
+        return self
+
+    def add_ellipse(
+            self,
+            x_center: FloatOrFloatIterable,
+            y_center: FloatOrFloatIterable,
+            width: FloatOrFloatIterable,
+            height: FloatOrFloatIterable,
+            angle: FloatOrFloatIterable = 0.0,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
+            label: Optional[StrOrStrIterable] = None,
+            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ):
+        """
+        Add an elliptical arc, i.e. a segment of an ellipse.
+
+        :param x_center: The x-coordinate of the center of the ellipse.
+        :param y_center: The y-coordinate of the center of the ellipse.
+        :param width: The length (diameter) of the horizontal axis.
+        :param height: The length (diameter) of the vertical axis.
+        :param angle: Rotation of the ellipse in degrees (counter-clockwise).
+        :param alpha: Opacity.
+        :param cap_style: Cap style.
+        :param color: Use to set both the edge-color and the face-color.
+        :param edge_color: Edge color.
+        :param face_color: Face color.
+        :param fill: Whether to fill the rectangle.
+        :param join_style: Join style.
+        :param label: Label for the object in the legend.
+        :param line_style: Line style for edge.
+        :param line_width: Line width for edge.
+        :param z_order: z-order for the ellipse.
+        """
+        for kwargs in smart_zip_kwargs(
+            x_center=x_center, y_center=y_center,
+            width=width, height=height, angle=angle,
+            alpha=alpha, capstyle=cap_style,
+            color=color, edgecolor=edge_color, facecolor=face_color,
+            fill=fill, joinstyle=join_style, label=label,
+            linestyle=line_style, linewidth=line_width, zorder=z_order
+        ):
+            kwargs = drop_none_values(kwargs)
+            kwargs = apply_mappings(kwargs, kwarg_mappings)
+            kwargs['xy'] = kwargs.pop('x_center'), kwargs.pop('y_center')
+            ellipse = Ellipse(**kwargs)
+            self._axes.add_artist(ellipse)
+
+        return self
+
+    def add_fancy_arrow(
+            self,
+            x_tail: FloatOrFloatIterable,
+            y_tail: FloatOrFloatIterable,
+            x_head: Optional[FloatOrFloatIterable] = None,
+            y_head: Optional[FloatOrFloatIterable] = None,
+            dx: Optional[FloatOrFloatIterable] = None,
+            dy: Optional[FloatOrFloatIterable] = None,
+            tail_width: FloatOrFloatIterable = 0.001,
+            length_includes_head: BoolOrBoolIterable = False,
+            head_width: Optional[FloatOrFloatIterable] = None,
+            head_length: Optional[FloatOrFloatIterable] = None,
+            shape: StrOrStrIterable = 'full',
+            overhang: FloatOrFloatIterable = 0.0,
+            head_starts_at_zero: BoolOrBoolIterable = False,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
+            label: Optional[StrOrStrIterable] = None,
+            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ):
+        """
+        Like Arrow, but lets you set head width and head height independently.
+
+        :param x_tail: The x-coordinate of the arrow tail.
+        :param y_tail: The y-coordinate of the arrow tail.
+        :param x_head: The x-coordinate of the arrow head.
+        :param y_head: The y-coordinate of the arrow head.
+        :param dx: Arrow length in the x direction. Only used if x_head is None.
+        :param dy: Arrow length in the y direction. Only used if y_head is None.
+        :param tail_width: Width of full arrow tail.
+        :param length_includes_head: True if head is to be counted in
+                                     calculating the length.
+        :param head_width: Total width of the full arrow head
+        :param head_length: Length of arrow head
+        :param shape: Draw the left-half, right-half, or full arrow.
+                      One of ['full', 'left', 'right'].
+        :param overhang: Fraction that the arrow is swept back
+                         (0 overhang means triangular shape).
+                         Can be negative or greater than one.
+        :param head_starts_at_zero: If True, the head starts being drawn at
+                                    coordinate 0 instead of ending at
+                                    coordinate 0.
+        :param alpha: Opacity.
+        :param cap_style: Cap style.
+        :param color: Use to set both the edge-color and the face-color.
+        :param edge_color: Edge color.
+        :param face_color: Face color.
+        :param fill: Whether to fill the rectangle.
+        :param join_style: Join style.
+        :param label: Label for the object in the legend.
+        :param line_style: Line style for edge.
+        :param line_width: Line width for edge.
+        :param z_order: z-order for the arrow.
+        """
+        if not one_is_not_none(dx, x_head):
+            raise ValueError('Must give dx or x_head')
+        if not one_is_not_none(dy, y_head):
+            raise ValueError('Must give dy or y_head')
+        for kwargs in smart_zip_kwargs(
+                x=x_tail, y=y_tail, x_head=x_head, y_head=y_head,
+                dx=dx, dy=dy, width=tail_width,
+                length_includes_head=length_includes_head,
+                head_width=head_width, head_length=head_length,
+                shape=shape, overhang=overhang,
+                head_starts_at_zero=head_starts_at_zero,
+                alpha=alpha, capstyle=cap_style,
+                color=color, edgecolor=edge_color, facecolor=face_color,
+                fill=fill, joinstyle=join_style, label=label,
+                linestyle=line_style, linewidth=line_width,
+                zorder=z_order
+        ):
+            kwargs = drop_none_values(kwargs)
+            kwargs = apply_mappings(kwargs, kwarg_mappings)
+            if kwargs['x_head'] is not None:
+                kwargs['dx'] = kwargs['x_head'] - kwargs['x']
+                kwargs.pop('x_head')
+            if kwargs['y_head'] is not None:
+                kwargs['dy'] = kwargs['y_head'] - kwargs['y']
+                kwargs.pop('y_head')
+            arrow = FancyArrow(**kwargs)
+            self._axes.add_artist(arrow)
+
+        return self
+
+    def add_fancy_arrow_patch(
+            self,
+            x: FloatOrFloatIterable,
+            y: FloatOrFloatIterable,
+            dx: FloatOrFloatIterable,
+            dy: FloatOrFloatIterable,
+            path: Optional[Union[Path, PathIterable]] = None,
+            arrow_style: Union[ArrowStyle, ArrowStyleIterable] = 'simple',
+            connection_style: Union[
+                ConnectionStyle, ConnectionStyleIterable
+            ] = CONNECTION_STYLE.arc_3,
+            tail_patch: Optional[Union[Patch, PatchIterable]] = None,
+            head_patch: Optional[Union[Patch, PatchIterable]] = None,
+            tail_shrink_factor: Optional[FloatOrFloatIterable] = 2,
+            head_shrink_factor: Optional[FloatOrFloatIterable] = 2,
+            mutation_scale: Optional[FloatOrFloatIterable] = 1,
+            mutation_aspect: Optional[FloatOrFloatIterable] = None,
+            dpi_cor: Optional[FloatOrFloatIterable] = 1,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
+            label: Optional[StrOrStrIterable] = None,
+            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ):
+        """
+        Like Arrow, but lets you set head width and head height independently.
+
+        :param x: The x-coordinate of the arrow tail.
+        :param y: The y-coordinate of the arrow tail.
+        :param dx: Arrow length in the x direction.
+        :param dy: Arrow length in the y direction.
+        :param path: If provided, an arrow is drawn along this path and
+                     tail_patch, head_patch, tail_shrink_factor, and
+                     head_shrink_factor are ignored.
+        :param arrow_style: Describes how the fancy arrow will be drawn.
+                            It can be string of the available arrowstyle names,
+                            with optional comma-separated attributes,
+                            or an ArrowStyle instance.
+                            The optional attributes are meant to be scaled with
+                            the mutation_scale.
+        :param connection_style: Describes how the arrow ends are connected.
+        :param tail_patch: Optional tail patch.
+        :param head_patch: Optional head patch.
+        :param tail_shrink_factor: Shrinking factor of the tail.
+        :param head_shrink_factor: Shrinking factor of the head.
+        :param mutation_scale: Value with which attributes of arrowstyle
+                               (e.g., head_length) will be scaled.
+        :param mutation_aspect: The height of the rectangle will be squeezed by
+                                this value before the mutation and the mutated
+                                box will be stretched by the inverse of it.
+        :param dpi_cor: dpi_cor is currently used for linewidth-related things
+                        and shrink factor. Mutation scale is affected by this.
+        :param alpha: Opacity.
+        :param cap_style: Cap style.
+        :param color: Use to set both the edge-color and the face-color.
+        :param edge_color: Edge color.
+        :param face_color: Face color.
+        :param fill: Whether to fill the rectangle.
+        :param join_style: Join style.
+        :param label: Label for the object in the legend.
+        :param line_style: Line style for edge.
+        :param line_width: Line width for edge.
+        :param z_order: z-order for the arrow.
+        """
+        for kwargs in smart_zip_kwargs(
+                x=x, y=y, dx=dx, dy=dy, path=path,
+                arrowstyle=arrow_style, connectionstyle=connection_style,
+                patchA=tail_patch, patchB=head_patch,
+                shrinkA=tail_shrink_factor, shrinkB=head_shrink_factor,
+                mutation_scale=mutation_scale, mutation_aspect=mutation_aspect,
+                dpi_cor=dpi_cor,
+                alpha=alpha, capstyle=cap_style,
+                color=color, edgecolor=edge_color, facecolor=face_color,
+                fill=fill, joinstyle=join_style, label=label,
+                linestyle=line_style, linewidth=line_width,
+                zorder=z_order
+        ):
+            x = kwargs.pop('x')
+            y = kwargs.pop('y')
+            dx = kwargs.pop('dx')
+            dy = kwargs.pop('dy')
+            kwargs['posA'] = x, y
+            kwargs['posB'] = x + dx, y + dy
+            kwargs = drop_none_values(kwargs)
+            kwargs = apply_mappings(kwargs, kwarg_mappings)
+            arrow = FancyArrowPatch(**kwargs)
+            self._axes.add_artist(arrow)
+
+        return self
+
+    def add_fancy_box_patch(
+            self,
+            x: FloatOrFloatIterable,
+            y: FloatOrFloatIterable,
+            width: FloatOrFloatIterable,
+            height: FloatOrFloatIterable,
+            box_style: Union[
+                BoxStyleType, BoxStyleTypeIterable] = BOX_STYLE.round,
+            mutation_scale: Optional[FloatOrFloatIterable] = 1,
+            mutation_aspect: Optional[FloatOrFloatIterable] = None,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
+            label: Optional[StrOrStrIterable] = None,
+            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ):
+        """
+        A fancy box around a rectangle with lower left at xy = (x, y)
+        with specified width and height.
+
+        :param x: The left coord of the rectangle.
+        :param y: The bottom coord of the rectangle.
+        :param width: The rectangle width.
+        :param height: The rectangle height.
+        :param box_style: The box style.
+        :param mutation_scale: Value with which attributes of arrowstyle
+                               (e.g. head_length) will be scaled.
+        :param mutation_aspect: The height of the rectangle will be squeezed by
+                                this value before the mutation and the mutated
+                                box will be stretched by the inverse of it.
+        :param alpha: Opacity.
+        :param cap_style: Cap style.
+        :param color: Use to set both the edge-color and the face-color.
+        :param edge_color: Edge color.
+        :param face_color: Face color.
+        :param fill: Whether to fill the rectangle.
+        :param join_style: Join style.
+        :param label: Label for the object in the legend.
+        :param line_style: Line style for edge.
+        :param line_width: Line width for edge.
+        :param z_order: z-order for the box.
+        """
+        for kwargs in smart_zip_kwargs(
+                x=x, y=y, width=width, height=height,
+                boxstyle=box_style,
+                mutation_scale=mutation_scale, mutation_aspect=mutation_aspect,
+                alpha=alpha, fill=fill,
+                color=color, edgecolor=edge_color, facecolor=face_color,
+                capstyle=cap_style, joinstyle=join_style,
+                label=label,
+                linestyle=line_style, linewidth=line_width,
+                zorder=z_order,
+        ):
+            kwargs = drop_none_values(kwargs)
+            kwargs = apply_mappings(kwargs, kwarg_mappings)
+            kwargs['xy'] = kwargs.pop('x'), kwargs.pop('y')
+            fancy_box = FancyBboxPatch(**kwargs)
+            self._axes.add_artist(fancy_box)
+
+        return self
+
+    def add_polygon(
+            self,
+            xy: Union[ndarray, NdArrayIterable],
+            closed: BoolOrBoolIterable = True,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            label: Optional[StrOrStrIterable] = None,
+            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None,
+            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a general polygon patch.
+
+        :param xy: A numpy array with shape Nx2.
+        :param closed: If True, the polygon will be closed so the starting and
+                       ending points are the same.
+        :param alpha: Opacity.
+        :param cap_style: Cap style.
+        :param color: Use to set both the edge-color and the face-color.
+        :param edge_color: Edge color.
+        :param face_color: Face color.
+        :param fill: Whether to fill the rectangle.
+        :param join_style: Join style.
+        :param label: Label for the object in the legend.
+        :param line_style: Line style for edge.
+        :param line_width: Line width for edge.
+        :param z_order: z-order for the polygon.
+        """
+        for kwargs in smart_zip_kwargs(
+                xy=xy, closed=closed,
+                alpha=alpha, color=color, edgecolor=edge_color,
+                facecolor=face_color, fill=fill,
+                label=label,
+                linestyle=line_style, linewidth=line_width,
+                capstyle=cap_style, joinstyle=join_style,
+                zorder=z_order,
+        ):
+            kwargs = drop_none_values(kwargs)
+            kwargs = apply_mappings(kwargs, kwarg_mappings)
+            polygon = Polygon(**kwargs)
+            self._axes.add_artist(polygon)
+
+        return self
+
+    def add_rectangle(
+            self,
+            width: FloatOrFloatIterable, 
+            height: FloatOrFloatIterable,
+            angle: FloatOrFloatIterable = 0.0,
+            x_left: Optional[FloatOrFloatIterable] = None, 
+            y_bottom: Optional[FloatOrFloatIterable] = None,
+            x_center: Optional[FloatOrFloatIterable] = None, 
+            y_center: Optional[FloatOrFloatIterable] = None,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
+            label: Optional[StrOrStrIterable] = None,
+            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a rectangle to the Axes.
+
+        :param x_left: The left rectangle coordinate.
+        :param y_bottom: The bottom rectangle coordinate.
+        :param width: Rectangle width.
+        :param height: Rectangle height.
+        :param x_left: The left rectangle coordinate.
+        :param y_bottom: The bottom rectangle coordinate.
+        :param x_center: The center rectangle x-coordinate.
+        :param y_center: The center rectangle y-coordinate.
+        :param angle: Rotation in degrees anti-clockwise about xy (default=0.0)
+        :param alpha: Opacity.
+        :param cap_style: Cap style.
+        :param color: Use to set both the edge-color and the face-color.
+        :param edge_color: Edge color.
+        :param face_color: Face color.
+        :param fill: Whether to fill the rectangle.
+        :param join_style: Join style.
+        :param label: Label for the object in the legend.
+        :param line_style: Line style for edge.
+        :param line_width: Line width for edge.
+        :param z_order: z-order for the rectangle.
+        """
+        for kwargs in smart_zip_kwargs(
+                width=width, height=height, angle=angle,
+                x_left=x_left, y_bottom=y_bottom,
+                x_center=x_center, y_center=y_center,
+                alpha=alpha, fill=fill, label=label,
+                color=color, edgecolor=edge_color, facecolor=face_color,
+                capstyle=cap_style, joinstyle=join_style,
+                linestyle=line_style, linewidth=line_width,
+                zorder=z_order
+        ):
+
+            if not one_is_not_none(x_left, x_center):
+                raise ValueError('Give one of {x_left, x_center}')
+            if not one_is_not_none(y_bottom, y_center):
+                raise ValueError('Give one of {y_bottom, y_center}')
+            if not (
+                    all_are_none(x_left, y_bottom) or
+                    all_are_none(x_center, y_center)
+            ):
+                raise ValueError(
+                    'Give either {x_left, y_bottom} or {x_center, y_center}'
+                )
+
+            kwargs = drop_none_values(kwargs)
+            kwargs = apply_mappings(kwargs, kwarg_mappings)
+
+            if all_are_none(x_left, y_bottom):
+                x_c = kwargs.pop('x_center')
+                y_c = kwargs.pop('y_center')
+                w = kwargs['width']
+                h = kwargs['height']
+                a = kwargs['angle']
+                x_l = x_c - w / 2
+                y_b = y_c - h / 2
+                r = ((w / 2) ** 2 + (h / 2) ** 2) ** 0.5
+                theta = atan2(h, w)
+                xc_new = x_l + r * cos(theta + pi * a / 180)
+                yc_new = y_b + r * sin(theta + pi * a / 180)
+                kwargs['x'] = x_l + x_c - xc_new
+                kwargs['y'] = y_b + y_c - yc_new
+            else:
+                kwargs['x'] = kwargs.pop('x_left')
+                kwargs['y'] = kwargs.pop('y_bottom')
+
+            kwargs['xy'] = kwargs.pop('x'), kwargs.pop('y')
+
+            rectangle = Rectangle(**kwargs)
+            self._axes.add_artist(rectangle)
+
+        return self
+
+    def add_regular_polygon(
+            self,
+            x_center: FloatOrFloatIterable,
+            y_center: FloatOrFloatIterable,
+            num_vertices: IntOrIntIterable,
+            radius: FloatOrFloatIterable,
+            angle: FloatOrFloatIterable = 0,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            label: Optional[StrOrStrIterable] = None,
+            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None,
+            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a rectangle to the Axes.
+
+        :param x_center: The x-coordinate of the center of the polygon.
+        :param y_center: The y-coordinate of the center of the polygon.
+        :param num_vertices: Number of vertices.
+        :param radius: The distance from the center to each of the vertices.
+        :param angle: Rotation in degrees anti-clockwise about xy
+                            (default is 0.0)
+        :param alpha: Opacity.
+        :param cap_style: Cap style.
+        :param color: Use to set both the edge-color and the face-color.
+        :param edge_color: Edge color.
+        :param face_color: Face color.
+        :param fill: Whether to fill the rectangle.
+        :param join_style: Join style.
+        :param label: Label for the object in the legend.
+        :param line_style: Line style for edge.
+        :param line_width: Line width for edge.
+        :param z_order: z-order for the polygon.
+        """
+        for kwargs in smart_zip_kwargs(
+                x_center=x_center, y_center=y_center,
+                numVertices=num_vertices, radius=radius, angle=angle,
+                alpha=alpha, fill=fill, label=label,
+                color=color, edgecolor=edge_color, facecolor=face_color,
+                linestyle=line_style, linewidth=line_width,
+                capstyle=cap_style, joinstyle=join_style,
+                zorder=z_order,
+        ):
+            kwargs = drop_none_values(kwargs)
+            kwargs = apply_mappings(kwargs, kwarg_mappings)
+            kwargs['orientation'] = pi * kwargs.pop('angle') / 180
+            polygon = RegularPolygon(**kwargs)
+            self._axes.add_artist(polygon)
+
+        return self
+
+    def add_wedge(
+            self,
+            x_center: FloatOrFloatIterable,
+            y_center: FloatOrFloatIterable,
+            radius: FloatOrFloatIterable,
+            theta_start: FloatOrFloatIterable,
+            theta_end: FloatOrFloatIterable,
+            width: Optional[FloatOrFloatIterable] = None,
+            alpha: Optional[FloatOrFloatIterable] = None,
+            cap_style: Optional[Union[CapStyle, CapStyleIterable]] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            join_style: Optional[Union[JoinStyle, JoinStyleIterable]] = None,
+            label: Optional[StrOrStrIterable] = None,
+            line_style: Optional[Union[LineStyle, LineStyleIterable]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None,
+            z_order: Optional[IntOrIntIterable] = None
+    ):
+        """
+        Add a wedge-shaped patch.
+
+        :param x_center: The x-coordinate of the center of the ellipse.
+        :param y_center: The y-coordinate of the center of the ellipse.
+        :param radius: (Outer) radius.
+        :param theta_start: Starting angle of the arc in degrees.
+                            Relative to angle, e.g. if angle = 45 and
+                            theta_start = 90 the absolute starting angle is 135.
+        :param theta_end: Ending angle of the arc in degrees.
+        :param width: If width is given, then a partial wedge is drawn from
+                      inner radius - width to outer radius.
+        :param alpha: Opacity.
+        :param cap_style: Cap style.
+        :param color: Use to set both the edge-color and the face-color.
+        :param edge_color: Edge color.
+        :param face_color: Face color.
+        :param fill: Whether to fill the rectangle.
+        :param join_style: Join style.
+        :param label: Label for the object in the legend.
+        :param line_style: Line style for edge.
+        :param line_width: Line width for edge.
+        :param z_order: z-order for the wedge.
+        """
+        for kwargs in smart_zip_kwargs(
+                x_center=x_center, y_center=y_center, r=radius,
+                theta1=theta_start, theta2=theta_end,
+                width=width, alpha=alpha, fill=fill,
+                color=color, edgecolor=edge_color, facecolor=face_color,
+                capstyle=cap_style, joinstyle=join_style, linestyle=line_style,
+                linewidth=line_width,
+                label=label, zorder=z_order,
+        ):
+            kwargs = drop_none_values(kwargs)
+            kwargs = apply_mappings(kwargs, kwarg_mappings)
+            kwargs['orientation'] = pi * kwargs.pop('angle') / 180
+            wedge = Wedge(**kwargs)
+            self._axes.add_artist(wedge)
+
+        return self
+
+    @property
+    def arcs(self) -> PatchListFormatter:
+        """
+        Return a list of the Arcs on the axes.
+        """
+        return PatchListFormatter([
+            a for a in self._axes.get_children()
+            if isinstance(a, Arc)
+        ])
+
+    @property
+    def arrows(self) -> PatchListFormatter:
+        """
+        Return a list of the Arrows on the axes.
+        """
+        return PatchListFormatter([
+            a for a in self._axes.get_children()
+            if isinstance(a, Arrow)
+        ])
+
+    @property
+    def circles(self) -> PatchListFormatter:
+        """
+        Return a list of the Circles on the axes.
+        """
+        return PatchListFormatter([
+            c for c in self._axes.get_children()
+            if isinstance(c, Circle)
+        ])
+
+    @property
+    def ellipses(self) -> PatchListFormatter:
+        """
+        Return a list of the Ellipses on the axes.
+        """
+        return PatchListFormatter([
+            e for e in self._axes.get_children()
+            if isinstance(e, Ellipse)
+        ])
+
+    @property
+    def fancy_arrows(self) -> PatchListFormatter:
+        """
+        Return a list of the FancyArrows on the axes.
+        """
+        return PatchListFormatter([
+            a for a in self._axes.get_children()
+            if isinstance(a, FancyArrow)
+        ])
+
+    @property
+    def fancy_arrow_patches(self) -> PatchListFormatter:
+        """
+        Return a list of the FancyArrowPatches on the axes.
+        """
+        return PatchListFormatter([
+            a for a in self._axes.get_children()
+            if isinstance(a, FancyArrowPatch)
+        ])
+
+    @property
+    def fancy_boxes(self) -> PatchListFormatter:
+        """
+        Return a list of the FancyBoxes on the axes.
+        """
+        return PatchListFormatter([
+            b for b in self._axes.get_children()
+            if isinstance(b, FancyBboxPatch)
+        ])
+
+    @property
+    def polygons(self) -> PatchListFormatter:
+        """
+        Return a list of the Polygons on the axes.
+        """
+        return PatchListFormatter([
+            p for p in self._axes.get_children()
+            if isinstance(p, Polygon)
+        ])
+
+    @property
+    def regular_polygons(self) -> PatchListFormatter:
+        """
+        Return a list of the RegularPolygons on the axes.
+        """
+        return PatchListFormatter([
+            r for r in self._axes.get_children()
+            if isinstance(r, RegularPolygon)
+        ])
+
+    @property
+    def wedges(self) -> PatchListFormatter:
+        """
+        Return a list of the Wedges on the axes.
+        """
+        return PatchListFormatter([
+            w for w in self._axes.get_children()
+            if isinstance(w, Wedge)
+        ])
+
+    # endregion
+
+    # region custom shapes
+
+    def add_v_density(
+            self,
+            x: float,
+            y_to_z: Series,
+            color: Optional[Color] = 'k',
+            color_min: Optional[Color] = None,
+            edge_color: Optional[Color] = None,
+            width: float = 0.8,
+            z_max: Optional[float] = None,
+            h_align: H_ALIGN = 'center'
+    ) -> 'AxesFormatter':
+        """
+        Add a vertical density bar to the plot.
+
+        :param x: The x-coordinate of the bar.
+        :param y_to_z: A mapping of the bar's y-coordinate to it density.
+        :param color: The color of the density bar.
+        :param color_min: Optional 2nd color to fade out to.
+        :param edge_color: Optional color for the outer edge of the density.
+        :param width: The bar width.
+        :param z_max: Value to scale down densities by to get to a range of
+                      0 to 1. Defaults to max value of y_to_z.
+        :param h_align: Horizontal alignment.
+                        One of {'left', 'center', 'right'}.
+        """
+        check_h_align(h_align)
+
+        if z_max is None:
+            z_max = y_to_z.max()
+        y = y_to_z.index.to_list()
+        y_lowers = y[: -1]
+        y_uppers = y[1:]
+
+        if h_align == 'left':
+            x_left = x
+        elif h_align == 'center':
+            x_left = x - width / 2
+        elif h_align == 'right':
+            x_left = x - width
+        else:
+            raise ValueError(f'h_align must be one of {H_ALIGN}')
+
+        alphas = (
+                y_to_z / z_max
+        ).rolling(2).mean().shift(-1).dropna().clip(0.0, 1.0)
+
+        if color_min is None:
+            color_min = color
+        colors = cross_fade(from_color=color_min, to_color=color,
+                            amount=alphas)
+        # add segments
+        for y_lower, y_upper, alpha, color in zip(
+                y_lowers, y_uppers, alphas, colors
+        ):
+            self.add_rectangle(
+                x_left=x_left, y_bottom=y_lower,
+                width=width, height=y_upper - y_lower,
+                face_color=color, alpha=alpha, line_width=0
+            )
+        # add edge
+        if edge_color is not None:
+            self.add_rectangle(
+                x_left=x_left, y_bottom=y_lowers[0],
+                width=width, height=y_uppers[-1] - y_lowers[0],
+                edge_color=edge_color, fill=False
+            )
+
+        return self
+
+    def add_h_density(
+            self, y: float,
+            x_to_z: Series,
+            color: Optional[Color] = 'k',
+            color_min: Optional[Color] = None,
+            edge_color: Optional[Color] = None,
+            height: float = 0.8,
+            z_max: Optional[float] = None,
+            v_align: V_ALIGN = 'center'
+    ) -> 'AxesFormatter':
+        """
+        Add a horizontal density bar to the plot.
+
+        :param y: The y-coordinate of the bar.
+        :param x_to_z: A mapping of the bar's x-coordinate to it density.
+        :param color: The color of the density bar.
+        :param color_min: Optional 2nd color to fade out to.
+        :param edge_color: Optional color for the outer edge of the density.
+        :param height: The bar width.
+        :param z_max: Value to scale down densities by to get to a range of
+                      0 to 1. Defaults to max value of x_to_z.
+        :param v_align: Vertical alignment.
+                        One of {'top', 'center', 'bottom'}.
+        """
+        check_v_align(v_align)
+
+        if z_max is None:
+            z_max = x_to_z.max()
+        x = x_to_z.index.to_list()
+        x_lefts = x[: -1]
+        x_rights = x[1:]
+
+        if v_align == 'bottom':
+            y_bottom = y
+        elif v_align == 'center':
+            y_bottom = y - height / 2
+        elif v_align == 'top':
+            y_bottom = y - height
+        else:
+            raise ValueError(f'v_align must be one of {V_ALIGN}')
+
+        alphas = (
+                x_to_z / z_max
+        ).rolling(2).mean().shift(-1).dropna().clip(0.0, 1.0)
+
+        if color_min is None:
+            color_min = color
+        colors = cross_fade(from_color=color_min, to_color=color,
+                            amount=alphas)
+        # add segments
+        for x_left, x_right, alpha, color in zip(
+                x_lefts, x_rights, alphas, colors
+        ):
+            self.add_rectangle(
+                x_left=x_left, y_bottom=y_bottom,
+                width=x_right-x_left, height=height,
+                face_color=color, alpha=alpha, line_width=0
+            )
+        # add edge
+        if edge_color is not None:
+            self.add_rectangle(
+                x_left=x_lefts[0], y_bottom=y_bottom,
+                width=x_rights[-1] - x_rights[0], height=height,
+                edge_color=edge_color, fill=False
+            )
+        return self
+
+    # endregion
+
+    # region plots
+
+    def add_v_bars(
+            self,
+            x: Union[str, FloatOrFloatIterable],
+            y: Union[str, FloatOrFloatIterable],
+            width: Union[str, FloatOrFloatIterable],
+            box_style: Union[BoxStyle, Iterable[BoxStyle]],
+            data: Optional[DataFrame] = None,
+            y_0: Optional[Union[str, FloatOrFloatIterable]] = 0.0,
+            h_align: H_ALIGN = 'center',
+            mutation_scale: Union[str, FloatOrFloatIterable] = 1,
+            mutation_aspect: Optional[Union[str, FloatOrFloatIterable]] = None,
+            alpha: Optional[Union[str, FloatOrFloatIterable]] = None,
+            cap_style: Optional[Union[
+                StrOrStrIterable, CAP_STYLE, Iterable[CAP_STYLE]
+            ]] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            line_style: Optional[Union[
+                StrOrStrIterable, LINE_STYLE, Iterable[LINE_STYLE]
+            ]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None
+    ) -> 'AxesFormatter':
+        """
+        Add vertical bars to the plot with the given BoxStyle.
+
+        :param x: X-coordinate for each bar, or name of column.
+        :param y: Y-coordinate of top of each bar, or name of column.
+        :param width: Width of each bar, or name of column.
+        :param box_style: The style of each box, or name of column.
+        :param data: Optional DataFrame to extract sequences of attributes.
+        :param y_0: Y-coordinate of bottom of each bar. Defaults to 0.
+        :param h_align: Horizontal alignment. One of {'left', 'center', 'right'}
+        :param mutation_scale: Scaling factor applied to the attributes of the
+                               box style (e.g. pad or rounding_size).
+        :param mutation_aspect: The height of the rectangle will be squeezed by
+                                this value before the mutation and the mutated
+                                box will be stretched by the inverse of it.
+                                For example, this allows different horizontal
+                                and vertical padding.
+        :param alpha: Opacity from 0 to 1.
+        :param cap_style: One of {'butt', 'round', 'projecting'}
+        :param color: Color for faces and edges.
+        :param edge_color: Color for edges.
+        :param face_color: Color for faces.
+        :param fill: Whether bars are filled.
+        :param line_style: Line style.
+        :param line_width: Line width.
+        """
+        check_h_align(h_align)
+
+        def get_data(item) -> Series:
+            if data is None:
+                return item
+            if isinstance(item, str) and item in data.columns:
+                return data[item]
+            else:
+                return item
+
+        def make_iterable(item):
+            if not isinstance(item, Iterable) or isinstance(item, str):
+                item = [item] * len(x)
+            return item
+
+        x = get_data(x)
+        y = make_iterable(get_data(y))
+        y_0 = make_iterable(get_data(y_0))
+        width = make_iterable(get_data(width))
+        box_style = make_iterable(get_data(box_style))
+        mutation_scale = make_iterable(get_data(mutation_scale))
+        mutation_aspect = make_iterable(get_data(mutation_aspect))
+        alpha = make_iterable(get_data(alpha))
+        cap_style = make_iterable(get_data(cap_style))
+        color = make_iterable(get_data(color))
+        edge_color = make_iterable(get_data(edge_color))
+        face_color = make_iterable(get_data(face_color))
+        fill = make_iterable(get_data(fill))
+        line_style = make_iterable(get_data(line_style))
+        line_width = make_iterable(get_data(line_width))
+
+        for (
+                x_i, y_i, y_0_i, w_i, bs_i,
+                ms_i, ma_i, a_i, cs_i,
+                c_i, ec_i, fc_i,
+                f_i, ls_i, lw_i
+        ) in zip(
+            x, y, y_0, width, box_style,
+            mutation_scale, mutation_aspect, alpha, cap_style,
+            color, edge_color, face_color,
+            fill, line_style, line_width
+        ):
+            if h_align == 'left':
+                x_p = x_i
+            elif h_align == 'center':
+                x_p = x_i - w_i / 2
+            else:
+                x_p = x_i - width
+
+            self.add_fancy_box_patch(
+                x=x_p, y=y_0_i, width=w_i, height=y_i - y_0_i,
+                box_style=bs_i,
+                mutation_scale=ms_i, mutation_aspect=ma_i,
+                alpha=a_i, cap_style=cs_i,
+                color=c_i, edge_color=ec_i, face_color=fc_i,
+                fill=f_i, line_style=ls_i, line_width=lw_i
+            )
+
+        return self
+
+    def add_v_pills(
+            self,
+            x: Union[str, FloatOrFloatIterable],
+            y: Union[str, FloatOrFloatIterable],
+            width: float,
+            data: Optional[DataFrame] = None,
+            y_0: Optional[Union[str, FloatOrFloatIterable]] = 0.0,
+            h_align: H_ALIGN = 'center',
+            alpha: Optional[Union[str, FloatOrFloatIterable]] = None,
+            color: Optional[ColorOrColorIterable] = None,
+            edge_color: Optional[ColorOrColorIterable] = None,
+            face_color: Optional[ColorOrColorIterable] = None,
+            fill: BoolOrBoolIterable = True,
+            line_style: Optional[Union[
+                StrOrStrIterable, LINE_STYLE, Iterable[LINE_STYLE]
+            ]] = None,
+            line_width: Optional[FloatOrFloatIterable] = None
+    ) -> 'AxesFormatter':
+        """
+        Add vertical bars to the plot with the given BoxStyle.
+
+        :param x: X-coordinate for each bar, or name of column.
+        :param y: Y-coordinate of top of each bar, or name of column.
+        :param width: Width of each bar, or name of column.
+        :param data: Optional DataFrame to extract sequences of attributes.
+        :param y_0: Y-coordinate of bottom of each bar. Defaults to 0.
+        :param h_align: One of {'left', 'center', 'right'}.
+        :param alpha: Opacity from 0 to 1.
+        :param color: Color for faces and edges.
+        :param edge_color: Color for edges.
+        :param face_color: Color for faces.
+        :param fill: Whether bars are filled.
+        :param line_style: Line style.
+        :param line_width: Line width.
+        """
+        mutation_aspect = (
+                (self.width() / self.height()) *
+                (self.get_y_height() / self.get_x_width())
+        )
+        self.add_v_bars(
+            data=data, x=x, y=y, width=width,
+            box_style=BoxStyle.Round(pad=0.0, rounding_size=width / 2),
+            y_0=y_0, h_align=h_align,
+            mutation_aspect=mutation_aspect,
+            alpha=alpha,
+            color=color, edge_color=edge_color, face_color=face_color,
+            fill=fill, line_style=line_style, line_width=line_width
+        )
+        return self
+
+    def add_line(
+            self,
+            x: FloatIterable, y: FloatIterable,
+            smooth: Union[bool, int] = False, smooth_order: int = 2,
+            alpha: Optional[float] = None,
+            color: Optional[Color] = None,
+            draw_style: Optional[Union[str, DRAW_STYLE]] = None,
+            label: Optional[str] = None,
+            line_style: Optional[LineStyle] = None,
+            line_width: Optional[float] = None,
+            marker: Optional[Union[str, MARKER_STYLE]] = None,
+            marker_edge_color: Optional[Color] = None,
+            marker_edge_width: Optional[float] = None,
+            marker_face_color: Optional[Color] = None,
+            marker_face_color_alt: Optional[Color] = None,
+            marker_size: Optional[float] = None,
+            z_order: Optional[int] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a line to the plot.
+
+        :param x: X-coordinates of the line.
+        :param y: Y-coordinates of the line.
+        :param smooth: True or False or number of points. True -> 1,000 points.
+        :param smooth_order: Order for smoothing e.g. 2 = quadratic, 3 = cubic
+        :param alpha: Opacity of the line.
+        :param color: Color of the line.
+        :param draw_style: Draw style. One of {'default', 'steps', 'steps-pre',
+                           'steps-mid', 'steps-post'}
+        :param label: Label.
+        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
+                           (offset, on-off-seq), ...}
+        :param line_width: Line width.
+        :param marker: Marker style.
+        :param marker_edge_color: Marker edge color.
+        :param marker_edge_width: Marker edge width.
+        :param marker_face_color: Marker face color.
+        :param marker_face_color_alt: Alt marker face color.
+        :param marker_size: Marker size.
+        :param z_order: z-order for the line.
+        """
+        if smooth is not False:
+            if smooth is True:
+                smooth = 1000
+            f_smooth = interp1d(x, y, kind=smooth_order)
+            x_smooth = linspace(min(x), max(x), smooth)
+            y_smooth = f_smooth(x_smooth)
+            x = x_smooth
+            y = y_smooth
+        if draw_style is not None:
+            draw_style = (
+                draw_style if isinstance(draw_style, str)
+                else DRAW_STYLE.get_name(draw_style)
+            )
+        if line_style is not None:
+            line_style = (
+                line_style if isinstance(line_style, str)
+                else LINE_STYLE.get_name(line_style)
+            )
+
+        self._axes.plot(
+            x, y, alpha=alpha, color=color,
+            drawstyle=draw_style,
+            label=label,
+            ls=line_style,
+            lw=line_width,
+            marker=marker,
+            markersize=marker_size,
+            mec=marker_edge_color,
+            mew=marker_edge_width,
+            mfc=marker_face_color,
+            mfcalt=marker_face_color_alt,
+            zorder=z_order
+        )
+        return self
+
+    # endregion
+
+    # endregion
+
+    def set_title_font_family(self, font_name: str) -> 'AxesFormatter':
+        """
+        Set the font family for the Axes title.
+
+        :param font_name: Name of the font.
+        """
+        self.title.set_font_family(font_name)
+        return self
+
+    # region limits
+
+    def get_x_lim(self) -> Tuple[float, float]:
+        """
+        Return the x-axis view limits.
+        """
+        return self._axes.get_xlim()
+
+    def get_y_lim(self) -> Tuple[float, float]:
+        """
+        Return the y-axis view limits.
+        """
+        return self._axes.get_ylim()
+
+    def set_x_lim(
+            self,
+            left: Optional[Union[float, date]] = None,
+            right: Optional[Union[float, date]] = None
+    ) -> 'AxesFormatter':
+        """
+        Set the limits of the x-axis.
+
+        :param left: Lower limit.
+        :param right: Upper limit.
+        """
+        self._axes.set_xlim(left=left, right=right)
+        return self
+
+    def set_y_lim(self, bottom: Optional[float] = None,
+                  top: Optional[float] = None) -> 'AxesFormatter':
+        """
+        Set the limits of the y-axis.
+
+        :param bottom: Lower limit.
+        :param top: Upper limit.
+        """
+        self._axes.set_ylim(bottom=bottom, top=top)
+        return self
+
+    def get_x_min(self) -> float:
+        """
+        Return the x-axis lower view limit.
+        """
+        return self.get_x_lim()[0]
+
+    def get_x_max(self) -> float:
+        """
+        Return the x-axis upper view limit.
+        """
+        return self.get_x_lim()[1]
+
+    def get_x_width(self) -> float:
+
+        return abs(self.get_x_max() - self.get_x_min())
+
+    def get_y_height(self) -> float:
+
+        return abs(self.get_y_max() - self.get_y_min())
+
+    def set_x_min(self, left: Union[float, date]) -> 'AxesFormatter':
+        """
+        Set the x-axis lower view limit.
+        """
+        self.set_x_lim(left, None)
+        return self
+
+    def set_x_max(self, right: Union[float, date] = None) -> 'AxesFormatter':
+        """
+        Set the x-axis upper view limit.
+        """
+        self.set_x_lim(None, right)
+        return self
+
+    def get_y_min(self) -> float:
+        """
+        Return the y-axis lower view limit.
+        """
+        return self.get_y_lim()[0]
+
+    def get_y_max(self) -> float:
+        """
+        Return the y-axis upper view limit.
+        """
+        return self.get_y_lim()[1]
+
+    def set_y_min(self, bottom: Union[float, date] = None) -> 'AxesFormatter':
+        """
+        Set the y-axis lower view limit.
+        """
+        self.set_y_lim(bottom, None)
+        return self
+
+    def set_y_max(self, top: Union[float, date] = None) -> 'AxesFormatter':
+        """
+        Set the y-axis upper view limit.
+        """
+        self.set_y_lim(None, top)
+        return self
+
+    def width(self, units: FIGURE_UNITS = 'inches') -> float:
+        """
+        Return the width of the subplot.
+
+        :param units: One of {'inches', 'pixels'}.
+        """
+        if units not in ('inches', 'pixels'):
+            raise ValueError("units not in ('inches', 'pixels')")
+        fig = self._axes.figure
+        bbox = self.axes.get_window_extent().transformed(
+            fig.dpi_scale_trans.inverted()
+        )
+        width = bbox.width
+        if units == 'pixels':
+            width *= fig.dpi
+        return width
+
+    def height(self, units: FIGURE_UNITS = 'inches') -> float:
+        """
+        Return the height of the subplot.
+
+        :param units: One of {'inches', 'pixels'}
+        """
+        if units not in ('inches', 'pixels'):
+            raise ValueError("units not in ('inches', 'pixels')")
+        fig = self._axes.figure
+        bbox = self.axes.get_window_extent().transformed(
+            fig.dpi_scale_trans.inverted()
+        )
+        height = bbox.height
+        if units == 'pixels':
+            height *= fig.dpi
+        return height
+
+    # endregion
+
+    # region frame
+
+    def show_frame(self) -> 'AxesFormatter':
+        """
+        Show the frame.
+        """
+        self._axes.set_frame_on(True)
+        return self
+
+    def hide_frame(self) -> 'AxesFormatter':
+        """
+        Hide the frame.
+        """
+        self._axes.set_frame_on(False)
+        return self
+
+    # endregion
+
+    # region grids
+
+    def grid(
+            self, value: bool = True,
+            which: WHICH_TICKS = 'major',
+            axis: WHICH_AXIS = 'both',
+            color: Optional[Color] = None,
+            line_width: Optional[float] = None,
+            line_style: Optional[LineStyle] = None
+    ) -> 'AxesFormatter':
+        """
+        Turn the grid on or off.
+
+        :param value: True or False. Defaults to True.
+        :param which: 'major', 'minor' or 'both'
+        :param axis: 'x', 'y' or 'both'
+        :param color: Color of the lines.
+        :param line_width: Line width.
+        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
+                           (offset, on-off-seq), ...}
+        """
+        kwargs = {}
+        if color is not None:
+            kwargs['color'] = color
+        if line_width is not None:
+            kwargs['lw'] = line_width
+        if line_style is not None:
+            kwargs['ls'] = LINE_STYLE.get_line_style(line_style)
+        try:
+            # older matplotlib versions
+            self._axes.grid(b=value, which=which, axis=axis,
+                            **kwargs)
+        except:
+            # newer matplotlib versions
+            self._axes.grid(visible=value, which=which, axis=axis,
+                            **kwargs)
+        return self
+
+    def add_major_xy_grid(
+            self,
+            color: Optional[Color] = '#888888',
+            line_width: Optional[float] = None,
+            line_style: Optional[LineStyle] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a major grid to both axes.
+
+        :param color: Color of the lines.
+        :param line_width: Line width.
+        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
+                           (offset, on-off-seq), ...}
+        """
+        self.grid(
+            value=True, which='major', axis='both',
+            color=color, line_width=line_width, line_style=line_style
+        )
+        return self
+
+    def add_minor_xy_grid(
+            self,
+            color: Optional[Color] = '#bbbbbb',
+            line_width: Optional[float] = None,
+            line_style: Optional[LineStyle] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a minor grid to both axes.
+
+        :param color: Color of the lines.
+        :param line_width: Line width.
+        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
+                           (offset, on-off-seq), ...}
+        """
+        self.grid(
+            value=True, which='minor', axis='both',
+            color=color, line_width=line_width, line_style=line_style
+        )
+        return self
+
+    def add_major_x_grid(
+            self,
+            color: Optional[Color] = '#888888',
+            line_width: Optional[float] = None,
+            line_style: Optional[LineStyle] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a major grid to the x-axis.
+
+        :param color: Color of the lines.
+        :param line_width: Line width.
+        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
+                           (offset, on-off-seq), ...}
+        """
+        self.grid(
+            value=True, which='major', axis='x',
+            color=color, line_width=line_width, line_style=line_style
+        )
+        return self
+
+    def add_minor_x_grid(
+            self,
+            color: Optional[Color] = '#bbbbbb',
+            line_width: Optional[float] = None,
+            line_style: Optional[LineStyle] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a minor grid to the x-axis.
+
+        :param color: Color of the lines.
+        :param line_width: Line width.
+        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
+                           (offset, on-off-seq), ...}
+        """
+        self.grid(
+            value=True, which='minor', axis='x',
+            color=color, line_width=line_width, line_style=line_style
+        )
+        return self
+
+    def add_major_y_grid(
+            self,
+            color: Optional[Color] = '#888888',
+            line_width: Optional[float] = None,
+            line_style: Optional[LineStyle] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a major grid to the y-axis.
+
+        :param color: Color of the lines.
+        :param line_width: Line width.
+        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
+                           (offset, on-off-seq), ...}
+        """
+        self.grid(
+            value=True, which='major', axis='y',
+            color=color, line_width=line_width, line_style=line_style
+        )
+        return self
+
+    def add_minor_y_grid(
+            self,
+            color: Optional[Color] = '#bbbbbb',
+            line_width: Optional[float] = None,
+            line_style: Optional[LineStyle] = None
+    ) -> 'AxesFormatter':
+        """
+        Add a minor grid to the y-axis.
+
+        :param color: Color of the lines.
+        :param line_width: Line width.
+        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
+                           (offset, on-off-seq), ...}
+        """
+        self.grid(
+            value=True, which='minor', axis='y',
+            color=color, line_width=line_width, line_style=line_style
+        )
+        return self
+
+    # endregion
+
+    def set_aspect(self, aspect: ASPECT) -> 'AxesFormatter':
+        """
+        Set the aspect of the axis scaling, i.e. the ratio of y-unit to x-unit.
+        """
+        self._axes.set_aspect(aspect=aspect)
+        return self
+
+    def set_aspect_equal(self) -> 'AxesFormatter':
+        """
+        Set the aspect of the axis scaling to equal.
+        """
+        return self.set_aspect('equal')
+
+    def set_anchor(self, anchor: ANCHOR) -> 'AxesFormatter':
+        """
+        Define the anchor location.
+        """
+        self._axes.set_anchor(anchor=anchor)
+        return self
+
+    def set_anchor_north(self) -> 'AxesFormatter':
+        """
+        Set the anchor location to the top of the figure.
+        """
+        return self.set_anchor('N')
+
+    def set_anchor_east(self) -> 'AxesFormatter':
+        """
+        Set the anchor location to the right of the figure.
+        """
+        return self.set_anchor('E')
+
+    def set_anchor_south(self) -> 'AxesFormatter':
+        """
+        Set the anchor location to the bottom of the figure.
+        """
+        return self.set_anchor('S')
+
+    def set_anchor_west(self) -> 'AxesFormatter':
+        """
+        Set the anchor location to the left of the figure.
+        """
+        return self.set_anchor('W')
+
+    def set_anchor_center(self) -> 'AxesFormatter':
+        """
+        Set the anchor location to the middle of the figure.
+        """
+        return self.set_anchor('C')
+
+    def set_anchor_north_east(self) -> 'AxesFormatter':
+        """
+        Set the anchor location to the top right of the figure.
+        """
+        return self.set_anchor('NE')
+
+    def set_anchor_north_west(self) -> 'AxesFormatter':
+        """
+        Set the anchor location to the top left of the figure.
+        """
+        return self.set_anchor('NW')
+
+    def set_anchor_south_east(self) -> 'AxesFormatter':
+        """
+        Set the anchor location to the bottom right of the figure.
+        """
+        return self.set_anchor('SE')
+
+    def set_anchor_south_west(self) -> 'AxesFormatter':
+        """
+        Set the anchor location to the bottom left of the figure.
+        """
+        return self.set_anchor('SW')
+
+    def set_axis_below(self,
+                       value: bool = True) -> 'AxesFormatter':
+        """
+        Set whether axis ticks and gridlines are above or below most artists.
+
+        :param value: True or False
+        """
+        self._axes.set_axisbelow(b=value)
+        return self
+
+    def tight_layout(self) -> 'AxesFormatter':
+        """
+        Call the tight_layout method on the Axes' figure.
+        """
+        self._axes.figure.tight_layout()
+        return self
+
+    def invert_x_axis(self) -> 'AxesFormatter':
+        """
+        Invert the x-axis.
+        """
+        self.x_axis.invert()
+        return self
+
+    def invert_y_axis(self) -> 'AxesFormatter':
+        """
+        Invert the y-axis.
+        """
+        self.y_axis.invert()
+        return self
+
+    def save(self,
+             file_path: Union[str, Path],
+             file_type: Optional[str] = None) -> 'AxesFormatter':
+        """
+        Save the plot to disk.
+
+        :param file_path: The file path to save the plot object to.
+        :param file_type: The type of file to save.
+                          Defaults to png if can't be auto-detected from name.
+        """
+        save_plot(plot_object=self._axes,
+                  file_path=file_path,
+                  file_type=file_type)
+        return self
+
+
+    def add_legend(
+            self,
+            handles: Optional[List[PathCollection]] = None,
+            labels: Optional[List[str]] = None,
+            location: Optional[LegendLocation] = None,
+            n_cols: Optional[int] = None,
+            font_size: Optional[str] = None,
+            font_properties: Optional[Union[FontProperties, dict]] = None,
+            line_points: Optional[int] = None,
+            scatter_points: Optional[int] = None,
+            scatter_y_offsets: Optional[ArrayLike] = None,
+            marker_scale: Optional[float] = None,
+            frame_on: Optional[bool] = None,
+            shadow: Optional[bool] = None,
+            frame_alpha: Optional[float] = None,
+            face_color: Optional[Color] = None,
+            edge_color: Optional[Color] = None,
+            mode: Optional[str] = None,
+            title: Optional[str] = None,
+            title_font_size: Optional[FontSize] = None,
+            label_spacing: Optional[float] = None,
+            handle_length: Optional[float] = None,
+            handle_text_pad: Optional[float] = None,
+            border_axes_pad: Optional[float] = None,
+            column_spacing: Optional[float] = None
+    ) -> LegendFormatter:
+        """
+        Add a legend to the Axes.
+
+        :param handles: A list of Artists (lines, patches) to be added to the
+                        legend.
+        :param labels: A list of labels to show next to the artists. The length
+                       of handles and labels should be the same. If they are
+                       not, they are truncated to the smaller of both lengths.
+        :param location: The legend location.
+        :param n_cols: The number of columns that the legend has. Default is 1.
+        :param font_size: The font size of the legend. If the value is numeric
+                          the size will be the absolute font size in points.
+                          String values are relative to the current default font
+                          size. This argument is only used if font_properties is
+                          not specified.
+        :param font_properties: The font properties of the legend. If None
+                                (default), the current matplotlib.rcParams will
+                                be used.
+        :param line_points: The number of marker points in the legend when
+                            creating a legend entry for a Line2D (line).
+                            Default is None, which means using
+                            rcParams["legend.numpoints"] (default: 1).
+        :param scatter_points: The number of marker points in the legend when
+        creating a legend entry for a PathCollection (scatter plot). Default is
+        None, which means using rcParams["legend.scatterpoints"] (default: 1).
+        :param scatter_y_offsets: The vertical offset (relative to the font
+        size) for the markers created for a scatter plot legend entry. 0.0 is at
+        the base the legend text, and 1.0 is at the top. To draw all markers at
+        the same height, set to [0.5]. Default is [0.375, 0.5, 0.3125].
+        :param marker_scale: The relative size of legend markers compared with
+                             the originally drawn ones. Default is None, which
+                             means using rcParams["legend.markerscale"]
+                             (default: 1.0).
+        :param frame_on: Whether the legend should be drawn on a patch (frame).
+                         Default is None, which means using
+                         rcParams["legend.frameon"] (default: True).
+        :param shadow: Whether to draw a shadow behind the legend. Default is
+                       None, which means using rcParams["legend.shadow"]
+                       (default: False).
+        :param frame_alpha: The alpha transparency of the legend's background.
+                            Default is None, which means using
+                            rcParams["legend.framealpha"] (default: 0.8). If
+                            shadow is activated and framealpha is None, the
+                            default value is ignored.
+        :param face_color: The legend's background color. Default is None, which
+                           means using rcParams["legend.facecolor"]
+                           (default: 'inherit'). If "inherit", use
+                           rcParams["axes.facecolor"] (default: 'white').
+        :param edge_color: The legend's background patch edge color. Default is
+                           None, which means using rcParams["legend.edgecolor"]
+                           (default: '0.8'). If "inherit", use take
+                           rcParams["axes.edgecolor"] (default: 'black').
+        :param mode: If mode is set to "expand" the legend will be horizontally
+                     expanded to fill the axes area (or bbox_to_anchor if
+                     defines the legend's size).
+        :param title: The legend's title. Default is no title (None).
+        :param title_font_size: The fontsize of the legend's title. Default is
+                                the default fontsize.
+        :param label_spacing: The fractional whitespace inside the legend
+        border, in font-size units. Default is None, which means using
+        rcParams["legend.borderpad"] (default: 0.4).
+        :param handle_length: The length of the legend handles, in font-size
+        units. Default is None, which means using
+        rcParams["legend.handlelength"] (default: 2.0).
+        :param handle_text_pad: The pad between the legend handle and text, in
+        font-size units. Default is None, which means using
+        rcParams["legend.handletextpad"] (default: 0.8).
+        :param border_axes_pad: The pad between the axes and legend border, in
+        font-size units. Default is None, which means using
+        rcParams["legend.borderaxespad"] (default: 0.5).
+        :param column_spacing: The spacing between columns, in font-size units.
+        Default is None, which means using rcParams["legend.columnspacing"]
+        (default: 2.0).
+        """
+        kwargs = {}
+        for kwarg, mpl_arg in zip(
+            [handles, labels, n_cols, font_properties, font_size,
+             line_points, scatter_points, scatter_y_offsets, marker_scale,
+             frame_on, shadow, frame_alpha, face_color, edge_color,
+             mode, title, title_font_size, label_spacing, handle_length,
+             handle_text_pad, border_axes_pad, column_spacing, location],
+            ['handles', 'labels', 'ncol', 'prop', 'fontsize',
+             'numpoints', 'scatterpoints', 'scatteryoffsets', 'markerscale',
+             'frameon', 'shadow', 'framealpha', 'facecolor', 'edgecolor',
+             'mode', 'title', 'title_fontsize', 'labelspacing', 'handlelength',
+             'handletextpad', 'borderaxespad', 'columnspacing', 'loc']
+        ):
+            if kwarg is not None:
+                kwargs[mpl_arg] = kwarg
+        self._legend = LegendFormatter(self._axes.legend(**kwargs))
+        return self._legend
+
+    def twin_x(self) -> 'AxesFormatter':
+
+        return AxesFormatter(self.axes.twinx())
+
+    def twin_y(self) -> 'AxesFormatter':
+
+        return AxesFormatter(self.axes.twiny())
+
+    def show(self) -> 'AxesFormatter':
+        """
+        Show the figure for the axes.
+        """
+        plt.show()
+        return self
```

### Comparing `mpl_format-0.317/mpl_format/axes/axis_formatter.py` & `mpl_format-0.318/mpl_format/axes/axis_formatter.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,485 +1,485 @@
-from typing import Optional, Tuple
-
-from matplotlib.axes import Axes
-from matplotlib.axis import Axis
-from matplotlib.dates import DateFormatter
-from matplotlib.text import Text
-from matplotlib.ticker import FuncFormatter, MultipleLocator, FixedLocator
-
-from mpl_format.axes.ticks_formatter import TicksFormatter
-from mpl_format.compound_types import FontSize, StringMapper
-from mpl_format.literals import ROTATION_MODE, AXIS_SCALE, WHICH_AXIS
-from mpl_format.text.text_formatter import TextFormatter
-from mpl_format.text.text_list_formatter import TextListFormatter
-from mpl_format.utils.number_utils import format_as_integer
-
-
-class AxisFormatter(object):
-
-    def __init__(self, axis: Axis, direction: WHICH_AXIS, axes: Axes):
-        """
-        Create a new AxisFormatter
-
-        :param axis: The matplotlib Axis instance to wrap.
-        :param direction: 'x' or 'y'
-        :param axes: Parent Axes instance.
-        """
-        self._axis: Axis = axis
-        self._direction: str = direction
-        self._axes: Axes = axes
-        self._label: TextFormatter = TextFormatter(self._axis.label)
-        self._ticks: TicksFormatter = TicksFormatter(
-            axis=direction, which='both', axes=self._axes)
-        self._major_ticks: TicksFormatter = TicksFormatter(
-            axis=direction, which='major', axes=self._axes)
-        self._minor_ticks: TicksFormatter = TicksFormatter(
-            axis=direction, which='minor', axes=self._axes)
-
-    # region properties
-
-    @property
-    def axis(self) -> Axis:
-        """
-        Return the wrapped matplotlib Axis object.
-        """
-        return self._axis
-
-    @property
-    def label(self) -> TextFormatter:
-        """
-        Return a TextFormatter wrapping the axis label.
-        """
-        return self._label
-
-    @property
-    def tick_labels(self) -> TextListFormatter:
-
-        return TextListFormatter([
-            TextFormatter(text) for text in self._axis.get_ticklabels()
-        ])
-
-    @property
-    def ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the ticks on the axis.
-        """
-        return self._ticks
-
-    @property
-    def major_ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the major ticks on the axis.
-        """
-        return self._major_ticks
-
-    @property
-    def minor_ticks(self) -> TicksFormatter:
-        """
-        Return a TicksFormatter for the minor ticks on the axis.
-        """
-        return self._minor_ticks
-
-    # endregion
-
-    # region labels
-
-    def get_label_text(self) -> str:
-
-        return self.axis.get_label_text()
-
-    def set_label_text(self, text: str) -> 'AxisFormatter':
-        """
-        Set the text of the Axis label.
-
-        :param text: Text for the Axis label.
-        """
-        self.label.set_text(text)
-        return self
-
-    def set_label_font_family(self, font_name: str) -> 'AxisFormatter':
-        """
-        Set the font family for the Axis label.
-
-        :param font_name: Name of the font to use.
-        """
-        self.label.set_font_family(font_name)
-        return self
-
-    def replace_label_text(self, old: str, new: str) -> 'AxisFormatter':
-        """
-        Replace the old label text with the new.
-
-        :param old: The old label text to replace.
-        :param new: The new label text to replace.
-        """
-        self.label.replace(old=old, new=new)
-        return self
-
-    def map_label_text(
-            self, mapping: StringMapper
-    ) -> 'AxisFormatter':
-        """
-        Map the label text using a dictionary or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        self.label.map(mapping)
-        return self
-
-    def rotate_label(
-            self, rotation: int,
-            how: ROTATION_MODE = 'absolute'
-    ) -> 'AxisFormatter':
-        """
-        Set the rotation of the axis label.
-
-        :param rotation: The rotation value to set in degrees.
-        :param how: 'absolute' or 'relative'
-        """
-        self.label.rotate(rotation, how)
-        return self
-
-    def remove_label(self) -> 'AxisFormatter':
-        """
-        Remove the Axis label.
-        """
-        self.set_label_text('')
-        return self
-
-    def wrap_label(self, max_width: int) -> 'AxisFormatter':
-        """
-        Wrap the axis label text if it exceeds a given width of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        self.label.wrap(max_width=max_width)
-        return self
-
-    def set_label_size(self, font_size: FontSize) -> 'AxisFormatter':
-        """
-        Set the font size for the axis label.
-
-        :param font_size: The font size in points or size name.
-        """
-        self.label.set_size(font_size)
-        return self
-
-    # endregion
-
-    # region tick labels
-
-    def set_format_integer(self,
-                           categorical: bool = False,
-                           kmbt: bool = False) -> 'AxisFormatter':
-        """
-        Format an axis with currency symbols and separators.
-
-        :param categorical: Whether the axis is displaying categorical items
-                            e.g. for bar plots.
-        :param kmbt: Whether to abbreviate numbers using K, M, B and T for
-                     thousands, millions, billions and trillions.
-        """
-        def to_integer(text: Text):
-            if isinstance(text, Text):
-                t = text.get_text()
-            else:
-                t = str(text)
-            if t == '':
-                return ''
-            number = float(t)
-            return format_as_integer(number=number, kmbt=kmbt)
-
-        if not categorical:
-            tick = FuncFormatter(lambda x, pos: to_integer(x))
-            self._axis.set_major_formatter(tick)
-        else:
-            self._axis.set_ticklabels([
-                to_integer(text) for text in self._axis.get_ticklabels()
-            ])
-
-        return self
-
-    def set_format_currency(
-            self,
-            symbol: str = '$',
-            num_decimals: int = 0,
-            categorical: bool = False,
-            kmbt: bool = False
-    ) -> 'AxisFormatter':
-        """
-        Format an axis with currency symbols and separators.
-
-        :param symbol: The currency symbol to use.
-        :param num_decimals: The number of decimal places to use
-                             (typically 0 or 2).
-        :param categorical: Whether the axis is displaying categorical items
-                            e.g. for bar plots.
-        :param kmbt: Whether to abbreviate numbers using K, M, B and T for
-                     thousands, millions, billions and trillions.
-        """
-
-        def to_currency(text: Text):
-            if isinstance(text, Text):
-                t = text.get_text()
-            else:
-                t = str(text)
-            if t == '':
-                return ''
-            number = float(t)
-            if not kmbt:
-                return f'{symbol}{number:,.{num_decimals}f}'
-            else:
-                for power, abbrev in zip(
-                        [12, 9, 6, 3],
-                        ['T', 'B', 'M', 'K']
-                ):
-                    if number >= 10 ** power:
-                        num = number / 10 ** power
-                        if num == int(num):
-                            num = int(num)
-                        return f'{symbol}{num:,}{abbrev}'
-                if number == int(number):
-                    number = int(number)
-                return f'{symbol}{number:,.{num_decimals}f}'
-
-        if not categorical:
-            tick = FuncFormatter(lambda x, pos: to_currency(x))
-            self._axis.set_major_formatter(tick)
-        else:
-            self._axis.set_ticklabels([
-                to_currency(text) for text in self._axis.get_ticklabels()
-            ])
-
-        return self
-
-    def set_format_percent(
-            self,
-            num_decimals: int = 0,
-            multiply_100: bool = True,
-            categorical: bool = False
-    ) -> 'AxisFormatter':
-        """
-        Format an axis as a percentage.
-
-        :param num_decimals: Number of decimal places for the resulting label.
-        :param multiply_100: Whether to multiply the existing value by 100
-                             before formatting.
-        :param categorical: Whether the axis is displaying categorical items
-                            e.g. for bar plots.
-        """
-        if not categorical:
-            def percent_formatter(value, pos):
-                value = float(value)
-                if multiply_100:
-                    value *= 100
-                return f'{value:.{num_decimals}f}%'
-            self._axis.set_major_formatter(FuncFormatter(percent_formatter))
-        else:
-            def to_percent(text: Text):
-                t = text.get_text()
-                if t == '':
-                    return ''
-                number = float(t)
-                if multiply_100:
-                    number *= 100
-                return f'{number:.{num_decimals}f}%'
-            self._axis.set_ticklabels([
-                to_percent(text) for text in self._axis.get_ticklabels()
-            ])
-
-        return self
-
-    def set_format_date(self, date_format: str):
-        """
-        Format the appearance of tick labels on a date axis.
-
-        :param date_format: Format for the date. See https://strftime.org/
-        """
-        self.axis.set_major_formatter(DateFormatter(date_format))
-
-    # endregion
-
-    # region set scale
-
-    def set_scale(self, scale: AXIS_SCALE) -> 'AxisFormatter':
-        """
-        Set the scale for the Axis.
-
-        :param scale: One of ['log', 'linear', 'symlog', 'logit']
-        """
-        if self._direction == 'x':
-            self._axes.set_xscale(value=scale)
-        else:
-            self._axes.set_yscale(value=scale)
-        return self
-
-    def set_scale_log(self) -> 'AxisFormatter':
-        """
-        Set the scale of the axis to logarithmic.
-        """
-        self.set_scale('log')
-        return self
-
-    def set_scale_linear(self) -> 'AxisFormatter':
-        """
-        Set the scale of the axis to logarithmic.
-        """
-        self.set_scale('linear')
-        return self
-
-    def set_scale_symmetrical_log(self) -> 'AxisFormatter':
-        """
-        Set the scale of the axis to symmetrical logarithmic.
-        """
-        self.set_scale('symlog')
-        return self
-
-    def set_scale_logit(self) -> 'AxisFormatter':
-        """
-        Set the scale of the axis to logit.
-        """
-        self.set_scale('logit')
-        return self
-
-    # endregion
-
-    # region inversion
-
-    def set_inverted(self, inverted: bool = True) -> 'AxisFormatter':
-        """
-        Set the Axis inversion property.
-
-        :param inverted: True or False.
-        """
-        self._axis.set_inverted(inverted=inverted)
-        return self
-
-    def invert(self) -> 'AxisFormatter':
-        """
-        Flip the Axis inversion property.
-        """
-        self._axis.set_inverted(inverted=not self._axis.get_inverted())
-        return self
-
-    # endregion
-
-    # region tick spacing
-
-    def set_tick_spacing(
-            self, major: float,
-            minor: Optional[float] = None,
-            major_offset: float = 0,
-            categorical: bool = False
-    ) -> 'AxisFormatter':
-        """
-        Set the spacing of ticks on the Axis.
-
-        :param major: Spacing for major ticks.
-        :param minor: Optional spacing for minor ticks.
-        :param major_offset: Optional offset index to start major ticks.
-                             Only applies if categorical is True.
-        :param categorical: Whether the axis is displaying categorical items
-                            e.g. for bar plots.
-        """
-        if categorical:
-            self._axis.set_major_locator(
-                FixedLocator([
-                    t for t in self._axis.get_ticklocs()
-                    if (t - major_offset) % major == 0
-                ])
-            )
-            if minor is not None:
-                self._axis.set_minor_locator(MultipleLocator(minor))
-        else:
-            self._axis.set_major_locator(MultipleLocator(base=major))
-            if minor is not None:
-                self._axis.set_minor_locator(MultipleLocator(base=minor))
-
-        return self
-
-    def keep_ticks(
-            self,
-            label_spacing: Optional[int] = None,
-            tick_spacing: Optional[int] = None,
-            start: int = 0, end: Optional[int] = None
-    ) -> 'AxisFormatter':
-        """
-        Keep only some tick labels and locations of a categorical axis.
-
-        :param label_spacing: Spacing of labels to keep.
-        :param tick_spacing: Spacing of ticks to keep.
-        :param start: Index of the first label to keep.
-        :param end: Index of the last label to keep,
-                    if it is n * spacing from start.
-        """
-        if label_spacing is not None:
-            labels = self._axis.get_ticklabels()
-            num_labels = len(labels)
-            if end is None or end > num_labels - 1:
-                end = num_labels - 1
-            self._axis.set_ticklabels([
-                label.get_text() if (
-                        start <= i <= end and (i - start) % label_spacing == 0
-                ) else Text()
-                for i, label in enumerate(labels)
-            ])
-        if tick_spacing is not None:
-            locations = self._axis.get_ticklocs()
-            self._axis.set_ticks([
-                location for i, location in enumerate(locations)
-                if (i - start) % tick_spacing == 0
-            ])
-        return self
-
-    # endregion
-
-    # region limits
-
-    def get_lim(self) -> Tuple[float, float]:
-        """
-        Return the axis view limits.
-        """
-        if self._direction == 'x':
-            return self._axes.get_xlim()
-        else:
-            return self._axes.get_ylim()
-
-    def get_min(self) -> float:
-        """
-        Return the axis lower view limit.
-        """
-        if self._direction == 'x':
-            return self._axes.get_xlim()[0]
-        else:
-            return self._axes.get_ylim()[0]
-
-    def get_max(self) -> float:
-        """
-        Return the axis upper view limit.
-        """
-        if self._direction == 'x':
-            return self._axes.get_xlim()[1]
-        else:
-            return self._axes.get_ylim()[1]
-
-    def set_min(self, value: float = None) -> 'AxisFormatter':
-        """
-        Set the axis lower view limit.
-        """
-        if self._direction == 'x':
-            self._axes.set_xlim(value, None)
-        else:
-            self._axes.set_ylim(value, None)
-        return self
-
-    def set_max(self, value: float = None) -> 'AxisFormatter':
-        """
-        Set the axis upper view limit.
-        """
-        if self._direction == 'x':
-            self._axes.set_xlim(None, value)
-        else:
-            self._axes.set_ylim(None, value)
-        return self
-
-    # endregion
+from typing import Optional, Tuple
+
+from matplotlib.axes import Axes
+from matplotlib.axis import Axis
+from matplotlib.dates import DateFormatter
+from matplotlib.text import Text
+from matplotlib.ticker import FuncFormatter, MultipleLocator, FixedLocator
+
+from mpl_format.axes.ticks_formatter import TicksFormatter
+from mpl_format.compound_types import FontSize, StringMapper
+from mpl_format.literals import ROTATION_MODE, AXIS_SCALE, WHICH_AXIS
+from mpl_format.text.text_formatter import TextFormatter
+from mpl_format.text.text_list_formatter import TextListFormatter
+from mpl_format.utils.number_utils import format_as_integer
+
+
+class AxisFormatter(object):
+
+    def __init__(self, axis: Axis, direction: WHICH_AXIS, axes: Axes):
+        """
+        Create a new AxisFormatter
+
+        :param axis: The matplotlib Axis instance to wrap.
+        :param direction: 'x' or 'y'
+        :param axes: Parent Axes instance.
+        """
+        self._axis: Axis = axis
+        self._direction: str = direction
+        self._axes: Axes = axes
+        self._label: TextFormatter = TextFormatter(self._axis.label)
+        self._ticks: TicksFormatter = TicksFormatter(
+            axis=direction, which='both', axes=self._axes)
+        self._major_ticks: TicksFormatter = TicksFormatter(
+            axis=direction, which='major', axes=self._axes)
+        self._minor_ticks: TicksFormatter = TicksFormatter(
+            axis=direction, which='minor', axes=self._axes)
+
+    # region properties
+
+    @property
+    def axis(self) -> Axis:
+        """
+        Return the wrapped matplotlib Axis object.
+        """
+        return self._axis
+
+    @property
+    def label(self) -> TextFormatter:
+        """
+        Return a TextFormatter wrapping the axis label.
+        """
+        return self._label
+
+    @property
+    def tick_labels(self) -> TextListFormatter:
+
+        return TextListFormatter([
+            TextFormatter(text) for text in self._axis.get_ticklabels()
+        ])
+
+    @property
+    def ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the ticks on the axis.
+        """
+        return self._ticks
+
+    @property
+    def major_ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the major ticks on the axis.
+        """
+        return self._major_ticks
+
+    @property
+    def minor_ticks(self) -> TicksFormatter:
+        """
+        Return a TicksFormatter for the minor ticks on the axis.
+        """
+        return self._minor_ticks
+
+    # endregion
+
+    # region labels
+
+    def get_label_text(self) -> str:
+
+        return self.axis.get_label_text()
+
+    def set_label_text(self, text: str) -> 'AxisFormatter':
+        """
+        Set the text of the Axis label.
+
+        :param text: Text for the Axis label.
+        """
+        self.label.set_text(text)
+        return self
+
+    def set_label_font_family(self, font_name: str) -> 'AxisFormatter':
+        """
+        Set the font family for the Axis label.
+
+        :param font_name: Name of the font to use.
+        """
+        self.label.set_font_family(font_name)
+        return self
+
+    def replace_label_text(self, old: str, new: str) -> 'AxisFormatter':
+        """
+        Replace the old label text with the new.
+
+        :param old: The old label text to replace.
+        :param new: The new label text to replace.
+        """
+        self.label.replace(old=old, new=new)
+        return self
+
+    def map_label_text(
+            self, mapping: StringMapper
+    ) -> 'AxisFormatter':
+        """
+        Map the label text using a dictionary or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        self.label.map(mapping)
+        return self
+
+    def rotate_label(
+            self, rotation: int,
+            how: ROTATION_MODE = 'absolute'
+    ) -> 'AxisFormatter':
+        """
+        Set the rotation of the axis label.
+
+        :param rotation: The rotation value to set in degrees.
+        :param how: 'absolute' or 'relative'
+        """
+        self.label.rotate(rotation, how)
+        return self
+
+    def remove_label(self) -> 'AxisFormatter':
+        """
+        Remove the Axis label.
+        """
+        self.set_label_text('')
+        return self
+
+    def wrap_label(self, max_width: int) -> 'AxisFormatter':
+        """
+        Wrap the axis label text if it exceeds a given width of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        self.label.wrap(max_width=max_width)
+        return self
+
+    def set_label_size(self, font_size: FontSize) -> 'AxisFormatter':
+        """
+        Set the font size for the axis label.
+
+        :param font_size: The font size in points or size name.
+        """
+        self.label.set_size(font_size)
+        return self
+
+    # endregion
+
+    # region tick labels
+
+    def set_format_integer(self,
+                           categorical: bool = False,
+                           kmbt: bool = False) -> 'AxisFormatter':
+        """
+        Format an axis with currency symbols and separators.
+
+        :param categorical: Whether the axis is displaying categorical items
+                            e.g. for bar plots.
+        :param kmbt: Whether to abbreviate numbers using K, M, B and T for
+                     thousands, millions, billions and trillions.
+        """
+        def to_integer(text: Text):
+            if isinstance(text, Text):
+                t = text.get_text()
+            else:
+                t = str(text)
+            if t == '':
+                return ''
+            number = float(t)
+            return format_as_integer(number=number, kmbt=kmbt)
+
+        if not categorical:
+            tick = FuncFormatter(lambda x, pos: to_integer(x))
+            self._axis.set_major_formatter(tick)
+        else:
+            self._axis.set_ticklabels([
+                to_integer(text) for text in self._axis.get_ticklabels()
+            ])
+
+        return self
+
+    def set_format_currency(
+            self,
+            symbol: str = '$',
+            num_decimals: int = 0,
+            categorical: bool = False,
+            kmbt: bool = False
+    ) -> 'AxisFormatter':
+        """
+        Format an axis with currency symbols and separators.
+
+        :param symbol: The currency symbol to use.
+        :param num_decimals: The number of decimal places to use
+                             (typically 0 or 2).
+        :param categorical: Whether the axis is displaying categorical items
+                            e.g. for bar plots.
+        :param kmbt: Whether to abbreviate numbers using K, M, B and T for
+                     thousands, millions, billions and trillions.
+        """
+
+        def to_currency(text: Text):
+            if isinstance(text, Text):
+                t = text.get_text()
+            else:
+                t = str(text)
+            if t == '':
+                return ''
+            number = float(t)
+            if not kmbt:
+                return f'{symbol}{number:,.{num_decimals}f}'
+            else:
+                for power, abbrev in zip(
+                        [12, 9, 6, 3],
+                        ['T', 'B', 'M', 'K']
+                ):
+                    if number >= 10 ** power:
+                        num = number / 10 ** power
+                        if num == int(num):
+                            num = int(num)
+                        return f'{symbol}{num:,}{abbrev}'
+                if number == int(number):
+                    number = int(number)
+                return f'{symbol}{number:,.{num_decimals}f}'
+
+        if not categorical:
+            tick = FuncFormatter(lambda x, pos: to_currency(x))
+            self._axis.set_major_formatter(tick)
+        else:
+            self._axis.set_ticklabels([
+                to_currency(text) for text in self._axis.get_ticklabels()
+            ])
+
+        return self
+
+    def set_format_percent(
+            self,
+            num_decimals: int = 0,
+            multiply_100: bool = True,
+            categorical: bool = False
+    ) -> 'AxisFormatter':
+        """
+        Format an axis as a percentage.
+
+        :param num_decimals: Number of decimal places for the resulting label.
+        :param multiply_100: Whether to multiply the existing value by 100
+                             before formatting.
+        :param categorical: Whether the axis is displaying categorical items
+                            e.g. for bar plots.
+        """
+        if not categorical:
+            def percent_formatter(value, pos):
+                value = float(value)
+                if multiply_100:
+                    value *= 100
+                return f'{value:.{num_decimals}f}%'
+            self._axis.set_major_formatter(FuncFormatter(percent_formatter))
+        else:
+            def to_percent(text: Text):
+                t = text.get_text()
+                if t == '':
+                    return ''
+                number = float(t)
+                if multiply_100:
+                    number *= 100
+                return f'{number:.{num_decimals}f}%'
+            self._axis.set_ticklabels([
+                to_percent(text) for text in self._axis.get_ticklabels()
+            ])
+
+        return self
+
+    def set_format_date(self, date_format: str):
+        """
+        Format the appearance of tick labels on a date axis.
+
+        :param date_format: Format for the date. See https://strftime.org/
+        """
+        self.axis.set_major_formatter(DateFormatter(date_format))
+
+    # endregion
+
+    # region set scale
+
+    def set_scale(self, scale: AXIS_SCALE) -> 'AxisFormatter':
+        """
+        Set the scale for the Axis.
+
+        :param scale: One of ['log', 'linear', 'symlog', 'logit']
+        """
+        if self._direction == 'x':
+            self._axes.set_xscale(value=scale)
+        else:
+            self._axes.set_yscale(value=scale)
+        return self
+
+    def set_scale_log(self) -> 'AxisFormatter':
+        """
+        Set the scale of the axis to logarithmic.
+        """
+        self.set_scale('log')
+        return self
+
+    def set_scale_linear(self) -> 'AxisFormatter':
+        """
+        Set the scale of the axis to logarithmic.
+        """
+        self.set_scale('linear')
+        return self
+
+    def set_scale_symmetrical_log(self) -> 'AxisFormatter':
+        """
+        Set the scale of the axis to symmetrical logarithmic.
+        """
+        self.set_scale('symlog')
+        return self
+
+    def set_scale_logit(self) -> 'AxisFormatter':
+        """
+        Set the scale of the axis to logit.
+        """
+        self.set_scale('logit')
+        return self
+
+    # endregion
+
+    # region inversion
+
+    def set_inverted(self, inverted: bool = True) -> 'AxisFormatter':
+        """
+        Set the Axis inversion property.
+
+        :param inverted: True or False.
+        """
+        self._axis.set_inverted(inverted=inverted)
+        return self
+
+    def invert(self) -> 'AxisFormatter':
+        """
+        Flip the Axis inversion property.
+        """
+        self._axis.set_inverted(inverted=not self._axis.get_inverted())
+        return self
+
+    # endregion
+
+    # region tick spacing
+
+    def set_tick_spacing(
+            self, major: float,
+            minor: Optional[float] = None,
+            major_offset: float = 0,
+            categorical: bool = False
+    ) -> 'AxisFormatter':
+        """
+        Set the spacing of ticks on the Axis.
+
+        :param major: Spacing for major ticks.
+        :param minor: Optional spacing for minor ticks.
+        :param major_offset: Optional offset index to start major ticks.
+                             Only applies if categorical is True.
+        :param categorical: Whether the axis is displaying categorical items
+                            e.g. for bar plots.
+        """
+        if categorical:
+            self._axis.set_major_locator(
+                FixedLocator([
+                    t for t in self._axis.get_ticklocs()
+                    if (t - major_offset) % major == 0
+                ])
+            )
+            if minor is not None:
+                self._axis.set_minor_locator(MultipleLocator(minor))
+        else:
+            self._axis.set_major_locator(MultipleLocator(base=major))
+            if minor is not None:
+                self._axis.set_minor_locator(MultipleLocator(base=minor))
+
+        return self
+
+    def keep_ticks(
+            self,
+            label_spacing: Optional[int] = None,
+            tick_spacing: Optional[int] = None,
+            start: int = 0, end: Optional[int] = None
+    ) -> 'AxisFormatter':
+        """
+        Keep only some tick labels and locations of a categorical axis.
+
+        :param label_spacing: Spacing of labels to keep.
+        :param tick_spacing: Spacing of ticks to keep.
+        :param start: Index of the first label to keep.
+        :param end: Index of the last label to keep,
+                    if it is n * spacing from start.
+        """
+        if label_spacing is not None:
+            labels = self._axis.get_ticklabels()
+            num_labels = len(labels)
+            if end is None or end > num_labels - 1:
+                end = num_labels - 1
+            self._axis.set_ticklabels([
+                label.get_text() if (
+                        start <= i <= end and (i - start) % label_spacing == 0
+                ) else Text()
+                for i, label in enumerate(labels)
+            ])
+        if tick_spacing is not None:
+            locations = self._axis.get_ticklocs()
+            self._axis.set_ticks([
+                location for i, location in enumerate(locations)
+                if (i - start) % tick_spacing == 0
+            ])
+        return self
+
+    # endregion
+
+    # region limits
+
+    def get_lim(self) -> Tuple[float, float]:
+        """
+        Return the axis view limits.
+        """
+        if self._direction == 'x':
+            return self._axes.get_xlim()
+        else:
+            return self._axes.get_ylim()
+
+    def get_min(self) -> float:
+        """
+        Return the axis lower view limit.
+        """
+        if self._direction == 'x':
+            return self._axes.get_xlim()[0]
+        else:
+            return self._axes.get_ylim()[0]
+
+    def get_max(self) -> float:
+        """
+        Return the axis upper view limit.
+        """
+        if self._direction == 'x':
+            return self._axes.get_xlim()[1]
+        else:
+            return self._axes.get_ylim()[1]
+
+    def set_min(self, value: float = None) -> 'AxisFormatter':
+        """
+        Set the axis lower view limit.
+        """
+        if self._direction == 'x':
+            self._axes.set_xlim(value, None)
+        else:
+            self._axes.set_ylim(value, None)
+        return self
+
+    def set_max(self, value: float = None) -> 'AxisFormatter':
+        """
+        Set the axis upper view limit.
+        """
+        if self._direction == 'x':
+            self._axes.set_xlim(None, value)
+        else:
+            self._axes.set_ylim(None, value)
+        return self
+
+    # endregion
```

### Comparing `mpl_format-0.317/mpl_format/axes/ticks_formatter.py` & `mpl_format-0.318/mpl_format/axes/ticks_formatter.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,416 +1,416 @@
-from datetime import date
-from itertools import product
-from typing import Union, List, Tuple, Iterator, Iterable, Callable
-
-import matplotlib.pyplot as plt
-from mpl_format.compound_types import FloatIterable
-from matplotlib.axes import Axes
-from matplotlib.axis import Axis
-
-from mpl_format.compound_types import Color, FontSize, StringMapper
-from mpl_format.enums import FONT_SIZE
-from mpl_format.enums.line_style import LINE_STYLE
-from mpl_format.literals import WHICH_TICKS, WHICH_AXIS
-from mpl_format.text.text_utils import wrap_text, map_text
-
-
-class TicksFormatter(object):
-
-    def __init__(self, axis: WHICH_AXIS, which: WHICH_TICKS, axes: Axes):
-        """
-        Create a new TicksFormatter.
-
-        :param axis: One of {'x', 'y', 'both'}
-        :param which: One of {'major', 'minor', 'both'}
-        :param axes: Axes to operate on.
-        """
-        self._axis: str = axis
-        self._which = which
-        self._axes: Axes = axes
-
-    def reset(self) -> 'TicksFormatter':
-        """
-        Set all parameters to defaults.
-        """
-        self._axes.tick_params(
-            axis=self._axis,
-            which=self._which,
-            reset=True
-        )
-        return self
-
-    @property
-    def _is_minor(self) -> bool:
-        return self._which == 'minor'
-
-    # region locations, values and labels
-
-    def set_locations(
-            self,
-            locations: Union[FloatIterable, Iterable[date]]
-    ) -> 'TicksFormatter':
-        """
-        Set the locations of the ticks.
-
-        :param locations: List of locations where the ticks should be located.
-        """
-        x_axis = self._axes.xaxis
-        y_axis = self._axes.yaxis
-        if self._axis in ('x', 'both'):
-            x_axis.set_ticks(ticks=locations, minor=self._is_minor)
-        if self._axis in ('y', 'both'):
-            y_axis.set_ticks(ticks=locations, minor=self._is_minor)
-        return self
-
-    def set_labels(self, labels: Iterable[str]) -> 'TicksFormatter':
-        """
-        Set the labels for the ticks.
-
-        :param labels: List of labels to annotate each tick value.
-        """
-        x_axis = self._axes.xaxis
-        y_axis = self._axes.yaxis
-        if self._axis in ('x', 'both'):
-            x_axis.set_ticklabels(ticklabels=labels, minor=self._is_minor)
-        if self._axis in ('y', 'both'):
-            y_axis.set_ticklabels(ticklabels=labels, minor=self._is_minor)
-        return self
-
-    def get_labels(
-            self,
-            fix_negatives: bool = True
-    ) -> List[str]:
-        """
-        Get the labels for the ticks.
-
-        :param fix_negatives: Whether to replace the negative sign that
-                              matplotlib uses with an actual negative sign.
-        """
-        plt.draw()
-        if self._axis == 'x':
-            x_labels = self._axes.xaxis.get_ticklabels(which=self._which)
-            if fix_negatives:
-                x_labels = [label.get_text().replace('\u2212', '-')
-                            for label in x_labels]
-            return x_labels
-        elif self._axis == 'y':
-            y_labels = self._axes.yaxis.get_ticklabels(which=self._which)
-            if fix_negatives:
-                y_labels = [label.get_text().replace('\u2212', '-')
-                            for label in y_labels]
-            return y_labels
-        else:  # 'both'
-            raise TypeError("Can't return labels for more than one axis")
-
-    def get_label_values(
-            self,
-    ) -> List[float]:
-        """
-        Get the values of the labels for the ticks (assuming the labels are
-        strings of actual values e.g. ['0', '1.5'].
-        """
-        if self._axis == 'x':
-            return [float(label) for label in
-                    self.get_labels(fix_negatives=True)]
-        elif self._axis == 'y':
-            return [float(label) for label in
-                    self.get_labels(fix_negatives=True)]
-        else:  # 'both'
-            raise TypeError("Can't return labels for more than one axis")
-
-    # endregion
-
-    # region direction
-
-    def set_direction(self, direction: str) -> 'TicksFormatter':
-        """
-        Puts ticks inside the axes, outside the axes, or both.
-
-        :param direction: One of {'in', 'out', 'inout', 'in_out'}
-        """
-        direction = {
-            'in': 'in',
-            'out': 'out',
-            'inout': 'inout',
-            'in_out': 'inout'
-        }[direction]
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               direction=direction)
-        return self
-
-    def set_direction_in(self) -> 'TicksFormatter':
-        """
-        Puts ticks inside the axes.
-        """
-        self.set_direction('in')
-        return self
-
-    def set_direction_out(self) -> 'TicksFormatter':
-        """
-        Puts ticks outside the axes.
-        """
-        self.set_direction('out')
-        return self
-
-    def set_direction_in_out(self) -> 'TicksFormatter':
-        """
-        Puts ticks inside and outside the axes.
-        """
-        self.set_direction('in_out')
-        return self
-
-    # endregion
-
-    def set_length(self, length: float) -> 'TicksFormatter':
-        """
-        Set the tick length in points.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               length=length)
-        return self
-
-    def set_width(self, width: float) -> 'TicksFormatter':
-        """
-        Set the tick width in points.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               width=width)
-        return self
-
-    def set_padding(self, padding: float) -> 'TicksFormatter':
-        """
-        Set the distance in points between tick and label.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               pad=padding)
-        return self
-
-    def set_color(self, color: Color) -> 'TicksFormatter':
-        """
-        Set the tick color.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               color=color)
-        return self
-
-    def set_colors(self, color: Color) -> 'TicksFormatter':
-        """
-        Set tick color and the label color to the same value.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               colors=color)
-        return self
-
-    def set_z_order(self, z_order: float) -> 'TicksFormatter':
-        """
-        Set the tick and label z-order.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               zorder=z_order)
-        return self
-
-    # region show ticks
-
-    def show_top(self, show: bool = True) -> 'TicksFormatter':
-        """
-        Whether to draw ticks at the top of the plot.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               top=show)
-        return self
-
-    def show_bottom(self, show: bool = True) -> 'TicksFormatter':
-        """
-        Whether to draw ticks at the bottom of the plot.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               bottom=show)
-        return self
-
-    def show_left(self, show: bool = True) -> 'TicksFormatter':
-        """
-        Whether to draw ticks at the left of the plot.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               left=show)
-        return self
-
-    def show_right(self, show: bool = True) -> 'TicksFormatter':
-        """
-        Whether to draw ticks at the right of the plot.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               right=show)
-        return self
-
-    # endregion
-
-    # region labels
-
-    def set_label_size(self, label_size: FontSize) -> 'TicksFormatter':
-        """
-        Set the tick label font size in points or as a string (e.g., 'large').
-        """
-        if isinstance(label_size, FONT_SIZE):
-            label_size = label_size.get_name()
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               labelsize=label_size)
-        return self
-
-    def set_label_color(self, color: Color) -> 'TicksFormatter':
-        """
-        Set the tick label color.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               labelcolor=color)
-        return self
-
-    def set_label_rotation(self, rotation: float) -> 'TicksFormatter':
-        """
-        Set the tick label rotation.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               rotation=rotation)
-        return self
-
-    def _iter_axis_minor(self) -> Iterator[Tuple[Axis, bool]]:
-        """
-        Iterate over the axes, and the major / minor components
-        attached to the ticks.
-        """
-        axes: List[Axis] = []
-        axis: Axis
-        if self._axis in ('x', 'both'):
-            axes.append(self._axes.xaxis)
-        if self._axis in ('y', 'both'):
-            axes.append(self._axes.yaxis)
-        minors: List[bool] = []
-        if self._which in ('minor', 'both'):
-            minors.append(True)
-        if self._which in ('major', 'both'):
-            minors.append(False)
-        for axis, minor in product(axes, minors):
-            yield axis, minor
-
-    def wrap_label_text(self, max_width: int) -> 'TicksFormatter':
-        """
-        Wrap the text for each tick label with new lines if it exceeds
-        a given width of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        for axis, minor in self._iter_axis_minor():
-            tick_labels = axis.get_ticklabels(minor=minor)
-            if all(t.get_text() == '' for t in tick_labels):
-                continue  # non categorical tick-labels e.g. line plot
-            axis.set_ticklabels(
-                ticklabels=[wrap_text(text, max_width)
-                            for text in tick_labels],
-                minor=minor
-            )
-        return self
-
-    def map_label_text(self, mapping: StringMapper) -> 'TicksFormatter':
-        """
-        Map the tick label text using a dictionary or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        plt.draw()  # make sure labels are drawn
-        for axis, minor in self._iter_axis_minor():
-            labels = [label.get_text()
-                      for label in axis.get_ticklabels(minor=minor)]
-            axis.set_ticklabels(
-                ticklabels=map_text(labels, mapping),
-                minor=minor
-            )
-        return self
-
-    def map_label_values(
-            self, mapping: Callable[[float], float]
-    ) -> 'TicksFormatter':
-        """
-        Map the values of tick label text using a dictionary or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        self.set_labels([
-            str(mapping(value)) for value in self.get_label_values()
-        ])
-        return self
-
-    # region show labels
-
-    def show_top_labels(self, show: bool = True) -> 'TicksFormatter':
-        """
-        Whether to draw tick labels at the top of the plot.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               labeltop=show)
-        return self
-
-    def show_bottom_labels(self, show: bool = True) -> 'TicksFormatter':
-        """
-        Whether to draw tick labels at the bottom of the plot.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               labelbottom=show)
-        return self
-
-    def show_left_labels(self, show: bool = True) -> 'TicksFormatter':
-        """
-        Whether to draw tick labels at the left of the plot.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               labelleft=show)
-        return self
-
-    def show_right_labels(self, show: bool = True) -> 'TicksFormatter':
-        """
-        Whether to draw tick labels at the right of the plot.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               labelright=show)
-        return self
-
-    # endregion
-
-    # endregion
-
-    # region grid
-
-    def set_grid_color(self, color: Color) -> 'TicksFormatter':
-        """
-        Set the grid line color.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               grid_color=color)
-        return self
-
-    def set_grid_alpha(self, alpha: float) -> 'TicksFormatter':
-        """
-        Set the transparency of grid lines: 0 (transparent) to 1 (opaque).
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               grid_alpha=alpha)
-        return self
-
-    def set_grid_line_width(self, line_width: float) -> 'TicksFormatter':
-        """
-        Set the width of grid lines in points.
-        """
-        self._axes.tick_params(axis=self._axis, which=self._which,
-                               grid_linewidth=line_width)
-        return self
-
-    def set_grid_line_style(self, line_style: Union[str, LINE_STYLE]):
-        """
-        Set the line style of the grid lines.
-        """
-        self._axes.tick_params(
-            axis=self._axis, which=self._which,
-            grid_linestyle=LINE_STYLE.get_line_style(line_style)
-        )
-        return self
-
-    # endregion
+from datetime import date
+from itertools import product
+from typing import Union, List, Tuple, Iterator, Iterable, Callable
+
+import matplotlib.pyplot as plt
+from mpl_format.compound_types import FloatIterable
+from matplotlib.axes import Axes
+from matplotlib.axis import Axis
+
+from mpl_format.compound_types import Color, FontSize, StringMapper
+from mpl_format.enums import FONT_SIZE
+from mpl_format.enums.line_style import LINE_STYLE
+from mpl_format.literals import WHICH_TICKS, WHICH_AXIS
+from mpl_format.text.text_utils import wrap_text, map_text
+
+
+class TicksFormatter(object):
+
+    def __init__(self, axis: WHICH_AXIS, which: WHICH_TICKS, axes: Axes):
+        """
+        Create a new TicksFormatter.
+
+        :param axis: One of {'x', 'y', 'both'}
+        :param which: One of {'major', 'minor', 'both'}
+        :param axes: Axes to operate on.
+        """
+        self._axis: str = axis
+        self._which = which
+        self._axes: Axes = axes
+
+    def reset(self) -> 'TicksFormatter':
+        """
+        Set all parameters to defaults.
+        """
+        self._axes.tick_params(
+            axis=self._axis,
+            which=self._which,
+            reset=True
+        )
+        return self
+
+    @property
+    def _is_minor(self) -> bool:
+        return self._which == 'minor'
+
+    # region locations, values and labels
+
+    def set_locations(
+            self,
+            locations: Union[FloatIterable, Iterable[date]]
+    ) -> 'TicksFormatter':
+        """
+        Set the locations of the ticks.
+
+        :param locations: List of locations where the ticks should be located.
+        """
+        x_axis = self._axes.xaxis
+        y_axis = self._axes.yaxis
+        if self._axis in ('x', 'both'):
+            x_axis.set_ticks(ticks=locations, minor=self._is_minor)
+        if self._axis in ('y', 'both'):
+            y_axis.set_ticks(ticks=locations, minor=self._is_minor)
+        return self
+
+    def set_labels(self, labels: Iterable[str]) -> 'TicksFormatter':
+        """
+        Set the labels for the ticks.
+
+        :param labels: List of labels to annotate each tick value.
+        """
+        x_axis = self._axes.xaxis
+        y_axis = self._axes.yaxis
+        if self._axis in ('x', 'both'):
+            x_axis.set_ticklabels(ticklabels=labels, minor=self._is_minor)
+        if self._axis in ('y', 'both'):
+            y_axis.set_ticklabels(ticklabels=labels, minor=self._is_minor)
+        return self
+
+    def get_labels(
+            self,
+            fix_negatives: bool = True
+    ) -> List[str]:
+        """
+        Get the labels for the ticks.
+
+        :param fix_negatives: Whether to replace the negative sign that
+                              matplotlib uses with an actual negative sign.
+        """
+        plt.draw()
+        if self._axis == 'x':
+            x_labels = self._axes.xaxis.get_ticklabels(which=self._which)
+            if fix_negatives:
+                x_labels = [label.get_text().replace('\u2212', '-')
+                            for label in x_labels]
+            return x_labels
+        elif self._axis == 'y':
+            y_labels = self._axes.yaxis.get_ticklabels(which=self._which)
+            if fix_negatives:
+                y_labels = [label.get_text().replace('\u2212', '-')
+                            for label in y_labels]
+            return y_labels
+        else:  # 'both'
+            raise TypeError("Can't return labels for more than one axis")
+
+    def get_label_values(
+            self,
+    ) -> List[float]:
+        """
+        Get the values of the labels for the ticks (assuming the labels are
+        strings of actual values e.g. ['0', '1.5'].
+        """
+        if self._axis == 'x':
+            return [float(label) for label in
+                    self.get_labels(fix_negatives=True)]
+        elif self._axis == 'y':
+            return [float(label) for label in
+                    self.get_labels(fix_negatives=True)]
+        else:  # 'both'
+            raise TypeError("Can't return labels for more than one axis")
+
+    # endregion
+
+    # region direction
+
+    def set_direction(self, direction: str) -> 'TicksFormatter':
+        """
+        Puts ticks inside the axes, outside the axes, or both.
+
+        :param direction: One of {'in', 'out', 'inout', 'in_out'}
+        """
+        direction = {
+            'in': 'in',
+            'out': 'out',
+            'inout': 'inout',
+            'in_out': 'inout'
+        }[direction]
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               direction=direction)
+        return self
+
+    def set_direction_in(self) -> 'TicksFormatter':
+        """
+        Puts ticks inside the axes.
+        """
+        self.set_direction('in')
+        return self
+
+    def set_direction_out(self) -> 'TicksFormatter':
+        """
+        Puts ticks outside the axes.
+        """
+        self.set_direction('out')
+        return self
+
+    def set_direction_in_out(self) -> 'TicksFormatter':
+        """
+        Puts ticks inside and outside the axes.
+        """
+        self.set_direction('in_out')
+        return self
+
+    # endregion
+
+    def set_length(self, length: float) -> 'TicksFormatter':
+        """
+        Set the tick length in points.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               length=length)
+        return self
+
+    def set_width(self, width: float) -> 'TicksFormatter':
+        """
+        Set the tick width in points.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               width=width)
+        return self
+
+    def set_padding(self, padding: float) -> 'TicksFormatter':
+        """
+        Set the distance in points between tick and label.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               pad=padding)
+        return self
+
+    def set_color(self, color: Color) -> 'TicksFormatter':
+        """
+        Set the tick color.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               color=color)
+        return self
+
+    def set_colors(self, color: Color) -> 'TicksFormatter':
+        """
+        Set tick color and the label color to the same value.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               colors=color)
+        return self
+
+    def set_z_order(self, z_order: float) -> 'TicksFormatter':
+        """
+        Set the tick and label z-order.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               zorder=z_order)
+        return self
+
+    # region show ticks
+
+    def show_top(self, show: bool = True) -> 'TicksFormatter':
+        """
+        Whether to draw ticks at the top of the plot.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               top=show)
+        return self
+
+    def show_bottom(self, show: bool = True) -> 'TicksFormatter':
+        """
+        Whether to draw ticks at the bottom of the plot.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               bottom=show)
+        return self
+
+    def show_left(self, show: bool = True) -> 'TicksFormatter':
+        """
+        Whether to draw ticks at the left of the plot.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               left=show)
+        return self
+
+    def show_right(self, show: bool = True) -> 'TicksFormatter':
+        """
+        Whether to draw ticks at the right of the plot.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               right=show)
+        return self
+
+    # endregion
+
+    # region labels
+
+    def set_label_size(self, label_size: FontSize) -> 'TicksFormatter':
+        """
+        Set the tick label font size in points or as a string (e.g., 'large').
+        """
+        if isinstance(label_size, FONT_SIZE):
+            label_size = label_size.get_name()
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               labelsize=label_size)
+        return self
+
+    def set_label_color(self, color: Color) -> 'TicksFormatter':
+        """
+        Set the tick label color.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               labelcolor=color)
+        return self
+
+    def set_label_rotation(self, rotation: float) -> 'TicksFormatter':
+        """
+        Set the tick label rotation.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               rotation=rotation)
+        return self
+
+    def _iter_axis_minor(self) -> Iterator[Tuple[Axis, bool]]:
+        """
+        Iterate over the axes, and the major / minor components
+        attached to the ticks.
+        """
+        axes: List[Axis] = []
+        axis: Axis
+        if self._axis in ('x', 'both'):
+            axes.append(self._axes.xaxis)
+        if self._axis in ('y', 'both'):
+            axes.append(self._axes.yaxis)
+        minors: List[bool] = []
+        if self._which in ('minor', 'both'):
+            minors.append(True)
+        if self._which in ('major', 'both'):
+            minors.append(False)
+        for axis, minor in product(axes, minors):
+            yield axis, minor
+
+    def wrap_label_text(self, max_width: int) -> 'TicksFormatter':
+        """
+        Wrap the text for each tick label with new lines if it exceeds
+        a given width of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        for axis, minor in self._iter_axis_minor():
+            tick_labels = axis.get_ticklabels(minor=minor)
+            if all(t.get_text() == '' for t in tick_labels):
+                continue  # non categorical tick-labels e.g. line plot
+            axis.set_ticklabels(
+                ticklabels=[wrap_text(text, max_width)
+                            for text in tick_labels],
+                minor=minor
+            )
+        return self
+
+    def map_label_text(self, mapping: StringMapper) -> 'TicksFormatter':
+        """
+        Map the tick label text using a dictionary or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        plt.draw()  # make sure labels are drawn
+        for axis, minor in self._iter_axis_minor():
+            labels = [label.get_text()
+                      for label in axis.get_ticklabels(minor=minor)]
+            axis.set_ticklabels(
+                ticklabels=map_text(labels, mapping),
+                minor=minor
+            )
+        return self
+
+    def map_label_values(
+            self, mapping: Callable[[float], float]
+    ) -> 'TicksFormatter':
+        """
+        Map the values of tick label text using a dictionary or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        self.set_labels([
+            str(mapping(value)) for value in self.get_label_values()
+        ])
+        return self
+
+    # region show labels
+
+    def show_top_labels(self, show: bool = True) -> 'TicksFormatter':
+        """
+        Whether to draw tick labels at the top of the plot.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               labeltop=show)
+        return self
+
+    def show_bottom_labels(self, show: bool = True) -> 'TicksFormatter':
+        """
+        Whether to draw tick labels at the bottom of the plot.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               labelbottom=show)
+        return self
+
+    def show_left_labels(self, show: bool = True) -> 'TicksFormatter':
+        """
+        Whether to draw tick labels at the left of the plot.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               labelleft=show)
+        return self
+
+    def show_right_labels(self, show: bool = True) -> 'TicksFormatter':
+        """
+        Whether to draw tick labels at the right of the plot.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               labelright=show)
+        return self
+
+    # endregion
+
+    # endregion
+
+    # region grid
+
+    def set_grid_color(self, color: Color) -> 'TicksFormatter':
+        """
+        Set the grid line color.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               grid_color=color)
+        return self
+
+    def set_grid_alpha(self, alpha: float) -> 'TicksFormatter':
+        """
+        Set the transparency of grid lines: 0 (transparent) to 1 (opaque).
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               grid_alpha=alpha)
+        return self
+
+    def set_grid_line_width(self, line_width: float) -> 'TicksFormatter':
+        """
+        Set the width of grid lines in points.
+        """
+        self._axes.tick_params(axis=self._axis, which=self._which,
+                               grid_linewidth=line_width)
+        return self
+
+    def set_grid_line_style(self, line_style: Union[str, LINE_STYLE]):
+        """
+        Set the line style of the grid lines.
+        """
+        self._axes.tick_params(
+            axis=self._axis, which=self._which,
+            grid_linestyle=LINE_STYLE.get_line_style(line_style)
+        )
+        return self
+
+    # endregion
```

### Comparing `mpl_format-0.317/mpl_format/colors/color_maps.py` & `mpl_format-0.318/mpl_format/colors/color_maps.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from matplotlib.colors import to_rgba, ListedColormap
-from numpy import linspace, concatenate
-
-from mpl_format.compound_types import Color
-from mpl_format.utils.color_utils import cross_fade
-
-
-class ColorMapGenerator(object):
-
-    @staticmethod
-    def fade_in_to_color(to_color: Color) -> ListedColormap:
-
-        to_color = to_rgba(to_color)
-        from_color = (to_color[0], to_color[1], to_color[2], 0.0)
-        return ListedColormap(cross_fade(
-            from_color, to_color, linspace(0, 1, 256)))
-
-    @staticmethod
-    def fade_from_white(to_color:  Color) -> ListedColormap:
-        to_color = to_rgba(to_color)
-        from_color = 'white'
-        return ListedColormap(cross_fade(
-            from_color, to_color, linspace(0, 1, 256)))
-
-    @staticmethod
-    def cross_fade(from_color: Color, to_color: Color) -> ListedColormap:
-        return ListedColormap(cross_fade(
-            from_color, to_color, linspace(0, 1, 256)
-        ))
-
-    @staticmethod
-    def diverging_fade_in_to_colors(
-        low_color: Color,
-        high_color: Color
-    ):
-        low_color = to_rgba(low_color)
-        low_color_transparent = (
-            low_color[0], low_color[1], low_color[2], 0.0
-        )
-        low_half = cross_fade(
-            low_color, low_color_transparent, linspace(0, 1, 128)
-        )
-        high_color = to_rgba(high_color)
-        high_color_transparent = (
-            high_color[0], high_color[1], high_color[2], 0.0
-        )
-        high_half = cross_fade(
-            high_color_transparent, high_color, linspace(0, 1, 128)
-        )
-        return ListedColormap(concatenate([low_half, high_half]))
+from matplotlib.colors import to_rgba, ListedColormap
+from numpy import linspace, concatenate
+
+from mpl_format.compound_types import Color
+from mpl_format.utils.color_utils import cross_fade
+
+
+class ColorMapGenerator(object):
+
+    @staticmethod
+    def fade_in_to_color(to_color: Color) -> ListedColormap:
+
+        to_color = to_rgba(to_color)
+        from_color = (to_color[0], to_color[1], to_color[2], 0.0)
+        return ListedColormap(cross_fade(
+            from_color, to_color, linspace(0, 1, 256)))
+
+    @staticmethod
+    def fade_from_white(to_color:  Color) -> ListedColormap:
+        to_color = to_rgba(to_color)
+        from_color = 'white'
+        return ListedColormap(cross_fade(
+            from_color, to_color, linspace(0, 1, 256)))
+
+    @staticmethod
+    def cross_fade(from_color: Color, to_color: Color) -> ListedColormap:
+        return ListedColormap(cross_fade(
+            from_color, to_color, linspace(0, 1, 256)
+        ))
+
+    @staticmethod
+    def diverging_fade_in_to_colors(
+        low_color: Color,
+        high_color: Color
+    ):
+        low_color = to_rgba(low_color)
+        low_color_transparent = (
+            low_color[0], low_color[1], low_color[2], 0.0
+        )
+        low_half = cross_fade(
+            low_color, low_color_transparent, linspace(0, 1, 128)
+        )
+        high_color = to_rgba(high_color)
+        high_color_transparent = (
+            high_color[0], high_color[1], high_color[2], 0.0
+        )
+        high_half = cross_fade(
+            high_color_transparent, high_color, linspace(0, 1, 128)
+        )
+        return ListedColormap(concatenate([low_half, high_half]))
```

### Comparing `mpl_format-0.317/mpl_format/colors/office.py` & `mpl_format-0.318/mpl_format/colors/office.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-class OfficeColors(object):
-
-    # theme
-    WHITE_BACKGROUND_1 = '#ffffff'
-    WHITE_BACKGROUND_1_DARKER_05 = '#f2f2f2'
-    WHITE_BACKGROUND_1_DARKER_15 = '#d9d9d9'
-    WHITE_BACKGROUND_1_DARKER_25 = '#bfbfbf'
-    WHITE_BACKGROUND_1_DARKER_35 = '#a6a6a6'
-    WHITE_BACKGROUND_1_DARKER_50 = '#808080'
-
-    BLACK_TEXT_1 = '#000000'
-    BLACK_TEXT_1_LIGHTER_50 = '#808080'
-    BLACK_TEXT_1_LIGHTER_35 = '#595959'
-    BLACK_TEXT_1_LIGHTER_25 = '#404040'
-    BLACK_TEXT_1_LIGHTER_15 = '#262626'
-    BLACK_TEXT_1_LIGHTER_05 = '#0d0d0d'
-
-    LIGHT_GRAY_BACKGROUND_2 = '#e7e6e6'
-    LIGHT_GRAY_BACKGROUND_2_DARKER_10 = '#d0cece'
-    LIGHT_GRAY_BACKGROUND_2_DARKER_25 = '#adaaaa'
-    LIGHT_GRAY_BACKGROUND_2_DARKER_50 = '#747171'
-    LIGHT_GRAY_BACKGROUND_2_DARKER_75 = '#3a3838'
-    LIGHT_GRAY_BACKGROUND_2_DARKER_90 = '#161616'
-
-    BLUE_GREY_TEXT_2 = '#475468'
-    BLUE_GREY_TEXT_2_LIGHTER_80 = '#d7dce3'
-    BLUE_GREY_TEXT_2_LIGHTER_60 = '#aeb9c8'
-    BLUE_GREY_TEXT_2_LIGHTER_40 = '#8797ae'
-    BLUE_GREY_TEXT_2_DARKER_25 = '#353f4e'
-    BLUE_GREY_TEXT_2_DARKER_50 = '#242b34'
-
-    BLUE_ACCENT_1 = '#4e71be'
-    BLUE_ACCENT_1_LIGHTER_80 = '#dae1f0'
-    BLUE_ACCENT_1_LIGHTER_60 = '#b7c6e4'
-    BLUE_ACCENT_1_LIGHTER_40 = '#93a9d7'
-    BLUE_ACCENT_1_DARKER_25 = '#375491'
-    BLUE_ACCENT_1_DARKER_50 = '#253761'
-
-    ORANGE_ACCENT_2 = '#df8244'
-    ORANGE_ACCENT_2_LIGHTER_80 = '#f8e5d8'
-    ORANGE_ACCENT_2_LIGHTER_60 = '#f1ccb1'
-    ORANGE_ACCENT_2_LIGHTER_40 = '#eab38b'
-    ORANGE_ACCENT_2_DARKER_25 = '#b96029'
-    ORANGE_ACCENT_2_DARKER_50 = '#7a401a'
-
-    GRAY_ACCENT_3 = '#a5a5a5'
-    GRAY_ACCENT_3_LIGHTER_80 = '#ededed'
-    GRAY_ACCENT_3_LIGHTER_60 = '#dbdbdb'
-    GRAY_ACCENT_3_LIGHTER_40 = '#c9c9c9'
-    GRAY_ACCENT_3_DARKER_25 = '#7b7b7b'
-    GRAY_ACCENT_3_DARKER_50 = '#525252'
-
-    GOLD_ACCENT_4 = '#f6c042'
-    GOLD_ACCENT_4_LIGHTER_80 = '#fdf2d0'
-    GOLD_ACCENT_4_LIGHTER_60 = '#fbe6a3'
-    GOLD_ACCENT_4_LIGHTER_40 = '#f9db78'
-    GOLD_ACCENT_4_DARKER_25 = '#b88f2f'
-    GOLD_ACCENT_4_DARKER_50 = '#7b611d'
-
-    BLUE_ACCENT_5 = '#699bd0'
-    BLUE_ACCENT_5_LIGHTER_80 = '#dfebf6'
-    BLUE_ACCENT_5_LIGHTER_60 = '#c2d6eb'
-    BLUE_ACCENT_5_LIGHTER_40 = '#a2c1e2'
-    BLUE_ACCENT_5_DARKER_25 = '#4175b0'
-    BLUE_ACCENT_5_DARKER_50 = '#2b4e75'
-
-    GREEN_ACCENT_6 = '#7fab55'
-    GREEN_ACCENT_6_LIGHTER_80 = '#e4eedc'
-    GREEN_ACCENT_6_LIGHTER_60 = '#cbdfb8'
-    GREEN_ACCENT_6_LIGHTER_40 = '#b1ce94'
-    GREEN_ACCENT_6_DARKER_25 = '#5e803f'
-    GREEN_ACCENT_6_DARKER_50 = '#3e5529'
-
-    # light rainbow
-    SALMON = '#ef857d'
-    CANTALOUPE = '#f8d686'
-    BANANA = '#fffb8b'
-    HONEYDEW = '#dcfa8a'
-    FLORA = '#99f788'
-    SPINDRIFT = '#98fad8'
-    ICE = '#98fbfd'
-    SKY = '#8dd4fb'
-    ORCHID = '#7a82f7'
-    LAVENDER = '#cc89f8'
-    BUBBLEGUM = '#ee8df9'
-    CARNATION = '#f091d4'
-
-    # medium rainbow
-    MARASCHINO = '#eb4025'
-    TANGERINGE = '#f19737'
-    LEMON = '#fffb54'
-    LIME = '#a7f64d'
-    SPRING = '#73f54a'
-    SEA_FOAM = '#73f69c'
-    TURQUOISE = '#73f8fd'
-    AQUA = '#3f95f7'
-    BLUEBERRY = '#0838f5'
-    GRAPE = '#8843f5'
-    MAGENTA = '#ec55f7'
-    STRAWBERRY = '#eb4791'
-
-    # dark rainbow
-    CAYENNE = '#882111'
-    MOCHA = '#8b551b'
-    ASPARAGUS = '#928f2c'
-    FERN = '#5e8d28'
-    CLOVER = '#3f8c27'
-    MOSS = '#3f8d57'
-    TEAL = '#3f8f92'
-    OCEAN = '#20538e'
-    MIDNIGHT = '#021c8d'
-    EGGPLANT = '#4b228d'
-    PLUM = '#882d8e'
-    MAROON = '#882450'
-
-    # greys
-    LICORICE = '#000000'
-    LEAD = '#212121'
-    TUNGSTEN = '#424242'
-    IRON = '#5e5e5e'
-    STEEL = '#797979'
-    TIN = '#929292'
-    NICKEL = '#929292'
-    ALUMINIUM = '#aaaaaa'
-    MAGNESIUM = '#c1c1c1'
-    SILVER = '#d6d6d6'
-    MERCURY = '#ebebeb'
-    SNOW = '#ffffff'
-
-
-class OfficeSpectra(object):
-
-    light_rainbow_12 = [
-        OfficeColors.SALMON,
-        OfficeColors.CANTALOUPE,
-        OfficeColors.BANANA,
-        OfficeColors.HONEYDEW,
-        OfficeColors.FLORA,
-        OfficeColors.SPINDRIFT,
-        OfficeColors.ICE,
-        OfficeColors.SKY,
-        OfficeColors.ORCHID,
-        OfficeColors.LAVENDER,
-        OfficeColors.BUBBLEGUM,
-        OfficeColors.CARNATION
-    ]
-
-    medium_rainbow_12 = [
-        OfficeColors.MARASCHINO,
-        OfficeColors.TANGERINGE,
-        OfficeColors.LEMON,
-        OfficeColors.LIME,
-        OfficeColors.SPRING,
-        OfficeColors.SEA_FOAM,
-        OfficeColors.TURQUOISE,
-        OfficeColors.AQUA,
-        OfficeColors.BLUEBERRY,
-        OfficeColors.GRAPE,
-        OfficeColors.MAGENTA,
-        OfficeColors.STRAWBERRY
-    ]
-
-    dark_rainbow_12 = [
-        OfficeColors.CAYENNE,
-        OfficeColors.MOCHA,
-        OfficeColors.ASPARAGUS,
-        OfficeColors.FERN,
-        OfficeColors.CLOVER,
-        OfficeColors.MOSS,
-        OfficeColors.TEAL,
-        OfficeColors.OCEAN,
-        OfficeColors.MIDNIGHT,
-        OfficeColors.EGGPLANT,
-        OfficeColors.PLUM,
-        OfficeColors.MAROON
-    ]
-
-    greys_11 = [
-        OfficeColors.LICORICE,
-        OfficeColors.LEAD,
-        OfficeColors.TUNGSTEN,
-        OfficeColors.IRON,
-        OfficeColors.STEEL,
-        OfficeColors.NICKEL,
-        OfficeColors.ALUMINIUM,
-        OfficeColors.MAGNESIUM,
-        OfficeColors.SILVER,
-        OfficeColors.MERCURY,
-        OfficeColors.SNOW,
-    ]
-
-    reds_3 = [
-        OfficeColors.CAYENNE,
-        OfficeColors.MARASCHINO,
-        OfficeColors.SALMON
-    ]
-
-    oranges_3 = [
-        OfficeColors.MOCHA,
-        OfficeColors.TANGERINGE,
-        OfficeColors.CANTALOUPE
-    ]
+class OfficeColors(object):
+
+    # theme
+    WHITE_BACKGROUND_1 = '#ffffff'
+    WHITE_BACKGROUND_1_DARKER_05 = '#f2f2f2'
+    WHITE_BACKGROUND_1_DARKER_15 = '#d9d9d9'
+    WHITE_BACKGROUND_1_DARKER_25 = '#bfbfbf'
+    WHITE_BACKGROUND_1_DARKER_35 = '#a6a6a6'
+    WHITE_BACKGROUND_1_DARKER_50 = '#808080'
+
+    BLACK_TEXT_1 = '#000000'
+    BLACK_TEXT_1_LIGHTER_50 = '#808080'
+    BLACK_TEXT_1_LIGHTER_35 = '#595959'
+    BLACK_TEXT_1_LIGHTER_25 = '#404040'
+    BLACK_TEXT_1_LIGHTER_15 = '#262626'
+    BLACK_TEXT_1_LIGHTER_05 = '#0d0d0d'
+
+    LIGHT_GRAY_BACKGROUND_2 = '#e7e6e6'
+    LIGHT_GRAY_BACKGROUND_2_DARKER_10 = '#d0cece'
+    LIGHT_GRAY_BACKGROUND_2_DARKER_25 = '#adaaaa'
+    LIGHT_GRAY_BACKGROUND_2_DARKER_50 = '#747171'
+    LIGHT_GRAY_BACKGROUND_2_DARKER_75 = '#3a3838'
+    LIGHT_GRAY_BACKGROUND_2_DARKER_90 = '#161616'
+
+    BLUE_GREY_TEXT_2 = '#475468'
+    BLUE_GREY_TEXT_2_LIGHTER_80 = '#d7dce3'
+    BLUE_GREY_TEXT_2_LIGHTER_60 = '#aeb9c8'
+    BLUE_GREY_TEXT_2_LIGHTER_40 = '#8797ae'
+    BLUE_GREY_TEXT_2_DARKER_25 = '#353f4e'
+    BLUE_GREY_TEXT_2_DARKER_50 = '#242b34'
+
+    BLUE_ACCENT_1 = '#4e71be'
+    BLUE_ACCENT_1_LIGHTER_80 = '#dae1f0'
+    BLUE_ACCENT_1_LIGHTER_60 = '#b7c6e4'
+    BLUE_ACCENT_1_LIGHTER_40 = '#93a9d7'
+    BLUE_ACCENT_1_DARKER_25 = '#375491'
+    BLUE_ACCENT_1_DARKER_50 = '#253761'
+
+    ORANGE_ACCENT_2 = '#df8244'
+    ORANGE_ACCENT_2_LIGHTER_80 = '#f8e5d8'
+    ORANGE_ACCENT_2_LIGHTER_60 = '#f1ccb1'
+    ORANGE_ACCENT_2_LIGHTER_40 = '#eab38b'
+    ORANGE_ACCENT_2_DARKER_25 = '#b96029'
+    ORANGE_ACCENT_2_DARKER_50 = '#7a401a'
+
+    GRAY_ACCENT_3 = '#a5a5a5'
+    GRAY_ACCENT_3_LIGHTER_80 = '#ededed'
+    GRAY_ACCENT_3_LIGHTER_60 = '#dbdbdb'
+    GRAY_ACCENT_3_LIGHTER_40 = '#c9c9c9'
+    GRAY_ACCENT_3_DARKER_25 = '#7b7b7b'
+    GRAY_ACCENT_3_DARKER_50 = '#525252'
+
+    GOLD_ACCENT_4 = '#f6c042'
+    GOLD_ACCENT_4_LIGHTER_80 = '#fdf2d0'
+    GOLD_ACCENT_4_LIGHTER_60 = '#fbe6a3'
+    GOLD_ACCENT_4_LIGHTER_40 = '#f9db78'
+    GOLD_ACCENT_4_DARKER_25 = '#b88f2f'
+    GOLD_ACCENT_4_DARKER_50 = '#7b611d'
+
+    BLUE_ACCENT_5 = '#699bd0'
+    BLUE_ACCENT_5_LIGHTER_80 = '#dfebf6'
+    BLUE_ACCENT_5_LIGHTER_60 = '#c2d6eb'
+    BLUE_ACCENT_5_LIGHTER_40 = '#a2c1e2'
+    BLUE_ACCENT_5_DARKER_25 = '#4175b0'
+    BLUE_ACCENT_5_DARKER_50 = '#2b4e75'
+
+    GREEN_ACCENT_6 = '#7fab55'
+    GREEN_ACCENT_6_LIGHTER_80 = '#e4eedc'
+    GREEN_ACCENT_6_LIGHTER_60 = '#cbdfb8'
+    GREEN_ACCENT_6_LIGHTER_40 = '#b1ce94'
+    GREEN_ACCENT_6_DARKER_25 = '#5e803f'
+    GREEN_ACCENT_6_DARKER_50 = '#3e5529'
+
+    # light rainbow
+    SALMON = '#ef857d'
+    CANTALOUPE = '#f8d686'
+    BANANA = '#fffb8b'
+    HONEYDEW = '#dcfa8a'
+    FLORA = '#99f788'
+    SPINDRIFT = '#98fad8'
+    ICE = '#98fbfd'
+    SKY = '#8dd4fb'
+    ORCHID = '#7a82f7'
+    LAVENDER = '#cc89f8'
+    BUBBLEGUM = '#ee8df9'
+    CARNATION = '#f091d4'
+
+    # medium rainbow
+    MARASCHINO = '#eb4025'
+    TANGERINGE = '#f19737'
+    LEMON = '#fffb54'
+    LIME = '#a7f64d'
+    SPRING = '#73f54a'
+    SEA_FOAM = '#73f69c'
+    TURQUOISE = '#73f8fd'
+    AQUA = '#3f95f7'
+    BLUEBERRY = '#0838f5'
+    GRAPE = '#8843f5'
+    MAGENTA = '#ec55f7'
+    STRAWBERRY = '#eb4791'
+
+    # dark rainbow
+    CAYENNE = '#882111'
+    MOCHA = '#8b551b'
+    ASPARAGUS = '#928f2c'
+    FERN = '#5e8d28'
+    CLOVER = '#3f8c27'
+    MOSS = '#3f8d57'
+    TEAL = '#3f8f92'
+    OCEAN = '#20538e'
+    MIDNIGHT = '#021c8d'
+    EGGPLANT = '#4b228d'
+    PLUM = '#882d8e'
+    MAROON = '#882450'
+
+    # greys
+    LICORICE = '#000000'
+    LEAD = '#212121'
+    TUNGSTEN = '#424242'
+    IRON = '#5e5e5e'
+    STEEL = '#797979'
+    TIN = '#929292'
+    NICKEL = '#929292'
+    ALUMINIUM = '#aaaaaa'
+    MAGNESIUM = '#c1c1c1'
+    SILVER = '#d6d6d6'
+    MERCURY = '#ebebeb'
+    SNOW = '#ffffff'
+
+
+class OfficeSpectra(object):
+
+    light_rainbow_12 = [
+        OfficeColors.SALMON,
+        OfficeColors.CANTALOUPE,
+        OfficeColors.BANANA,
+        OfficeColors.HONEYDEW,
+        OfficeColors.FLORA,
+        OfficeColors.SPINDRIFT,
+        OfficeColors.ICE,
+        OfficeColors.SKY,
+        OfficeColors.ORCHID,
+        OfficeColors.LAVENDER,
+        OfficeColors.BUBBLEGUM,
+        OfficeColors.CARNATION
+    ]
+
+    medium_rainbow_12 = [
+        OfficeColors.MARASCHINO,
+        OfficeColors.TANGERINGE,
+        OfficeColors.LEMON,
+        OfficeColors.LIME,
+        OfficeColors.SPRING,
+        OfficeColors.SEA_FOAM,
+        OfficeColors.TURQUOISE,
+        OfficeColors.AQUA,
+        OfficeColors.BLUEBERRY,
+        OfficeColors.GRAPE,
+        OfficeColors.MAGENTA,
+        OfficeColors.STRAWBERRY
+    ]
+
+    dark_rainbow_12 = [
+        OfficeColors.CAYENNE,
+        OfficeColors.MOCHA,
+        OfficeColors.ASPARAGUS,
+        OfficeColors.FERN,
+        OfficeColors.CLOVER,
+        OfficeColors.MOSS,
+        OfficeColors.TEAL,
+        OfficeColors.OCEAN,
+        OfficeColors.MIDNIGHT,
+        OfficeColors.EGGPLANT,
+        OfficeColors.PLUM,
+        OfficeColors.MAROON
+    ]
+
+    greys_11 = [
+        OfficeColors.LICORICE,
+        OfficeColors.LEAD,
+        OfficeColors.TUNGSTEN,
+        OfficeColors.IRON,
+        OfficeColors.STEEL,
+        OfficeColors.NICKEL,
+        OfficeColors.ALUMINIUM,
+        OfficeColors.MAGNESIUM,
+        OfficeColors.SILVER,
+        OfficeColors.MERCURY,
+        OfficeColors.SNOW,
+    ]
+
+    reds_3 = [
+        OfficeColors.CAYENNE,
+        OfficeColors.MARASCHINO,
+        OfficeColors.SALMON
+    ]
+
+    oranges_3 = [
+        OfficeColors.MOCHA,
+        OfficeColors.TANGERINGE,
+        OfficeColors.CANTALOUPE
+    ]
```

### Comparing `mpl_format-0.317/mpl_format/enums/__init__.py` & `mpl_format-0.318/mpl_format/enums/__init__.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from mpl_format.enums.arrow_style import ARROW_STYLE
-from mpl_format.enums.box_style import BOX_STYLE
-from mpl_format.enums.cap_style import CAP_STYLE
-from mpl_format.enums.connection_style import CONNECTION_STYLE
-from mpl_format.enums.draw_style import DRAW_STYLE
-from mpl_format.enums.font_size import FONT_SIZE
-from mpl_format.enums.font_stretch import FONT_STRETCH
-from mpl_format.enums.font_style import FONT_STYLE
-from mpl_format.enums.font_variant import FONT_VARIANT
-from mpl_format.enums.font_weight import FONT_WEIGHT
-from mpl_format.enums.join_style import JOIN_STYLE
-from mpl_format.enums.line_style import LINE_STYLE
-from mpl_format.enums.marker_style import MARKER_STYLE
+from mpl_format.enums.arrow_style import ARROW_STYLE
+from mpl_format.enums.box_style import BOX_STYLE
+from mpl_format.enums.cap_style import CAP_STYLE
+from mpl_format.enums.connection_style import CONNECTION_STYLE
+from mpl_format.enums.draw_style import DRAW_STYLE
+from mpl_format.enums.font_size import FONT_SIZE
+from mpl_format.enums.font_stretch import FONT_STRETCH
+from mpl_format.enums.font_style import FONT_STYLE
+from mpl_format.enums.font_variant import FONT_VARIANT
+from mpl_format.enums.font_weight import FONT_WEIGHT
+from mpl_format.enums.join_style import JOIN_STYLE
+from mpl_format.enums.line_style import LINE_STYLE
+from mpl_format.enums.marker_style import MARKER_STYLE
```

### Comparing `mpl_format-0.317/mpl_format/enums/box_style.py` & `mpl_format-0.318/mpl_format/enums/box_style.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from enum import Enum
-from typing import Union
-
-from matplotlib.patches import BoxStyle
-
-
-class BOX_STYLE(Enum):
-
-    circle = 0
-    double_arrow = 1
-    left_arrow = 2
-    right_arrow = 3
-    round = 4
-    round_4 = 5
-    round_tooth = 6
-    saw_tooth = 7
-    square = 8
-
-    def get_name(self) -> str:
-
-        return {
-            'circle': 'circle',
-            'double_arrow': 'darrow',
-            'left_arrow': 'larrow',
-            'right_arrow': 'rarrow',
-            'round': 'round',
-            'round_4': 'round4',
-            'round_tooth': 'roundtooth',
-            'saw_tooth': 'sawtooth',
-            'square': 'square'
-        }[self.name]
-
-    @staticmethod
-    def get_box_style(
-            box_style: Union[str, 'BOX_STYLE']
-    ) -> str:
-        if box_style and isinstance(box_style, BOX_STYLE):
-            box_style = box_style.get_name()
-        return box_style
-
-
-BoxStyleType = Union[
-    str, BOX_STYLE,
-    BoxStyle.Circle, BoxStyle.Round, BoxStyle.Round4,
-    BoxStyle.DArrow, BoxStyle.LArrow, BoxStyle.RArrow,
-    BoxStyle.Roundtooth, BoxStyle.Sawtooth, BoxStyle.Square
-]
+from enum import Enum
+from typing import Union
+
+from matplotlib.patches import BoxStyle
+
+
+class BOX_STYLE(Enum):
+
+    circle = 0
+    double_arrow = 1
+    left_arrow = 2
+    right_arrow = 3
+    round = 4
+    round_4 = 5
+    round_tooth = 6
+    saw_tooth = 7
+    square = 8
+
+    def get_name(self) -> str:
+
+        return {
+            'circle': 'circle',
+            'double_arrow': 'darrow',
+            'left_arrow': 'larrow',
+            'right_arrow': 'rarrow',
+            'round': 'round',
+            'round_4': 'round4',
+            'round_tooth': 'roundtooth',
+            'saw_tooth': 'sawtooth',
+            'square': 'square'
+        }[self.name]
+
+    @staticmethod
+    def get_box_style(
+            box_style: Union[str, 'BOX_STYLE']
+    ) -> str:
+        if box_style and isinstance(box_style, BOX_STYLE):
+            box_style = box_style.get_name()
+        return box_style
+
+
+BoxStyleType = Union[
+    str, BOX_STYLE,
+    BoxStyle.Circle, BoxStyle.Round, BoxStyle.Round4,
+    BoxStyle.DArrow, BoxStyle.LArrow, BoxStyle.RArrow,
+    BoxStyle.Roundtooth, BoxStyle.Sawtooth, BoxStyle.Square
+]
```

### Comparing `mpl_format-0.317/mpl_format/enums/connection_style.py` & `mpl_format-0.318/mpl_format/enums/connection_style.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from enum import Enum
-from typing import Union
-
-
-class CONNECTION_STYLE(Enum):
-
-    angle = 1
-    angle_3 = 2
-    arc = 3
-    arc_3 = 4
-    bar = 5
-
-    def get_name(self) -> str:
-
-        return {
-            'angle': 'angle',
-            'angle_3': 'angle3',
-            'arc': 'arc',
-            'arc_3': 'arc3',
-            'bar': 'bar'
-        }[self.name]
-
-    @staticmethod
-    def get_connection_style(
-            connection_style: Union[str, 'CONNECTION_STYLE']
-    ) -> str:
-        if connection_style and isinstance(connection_style, CONNECTION_STYLE):
-            connection_style = connection_style.get_name()
-        return connection_style
+from enum import Enum
+from typing import Union
+
+
+class CONNECTION_STYLE(Enum):
+
+    angle = 1
+    angle_3 = 2
+    arc = 3
+    arc_3 = 4
+    bar = 5
+
+    def get_name(self) -> str:
+
+        return {
+            'angle': 'angle',
+            'angle_3': 'angle3',
+            'arc': 'arc',
+            'arc_3': 'arc3',
+            'bar': 'bar'
+        }[self.name]
+
+    @staticmethod
+    def get_connection_style(
+            connection_style: Union[str, 'CONNECTION_STYLE']
+    ) -> str:
+        if connection_style and isinstance(connection_style, CONNECTION_STYLE):
+            connection_style = connection_style.get_name()
+        return connection_style
```

### Comparing `mpl_format-0.317/mpl_format/enums/font_size.py` & `mpl_format-0.318/mpl_format/enums/font_size.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from enum import Enum
-from typing import Union
-
-
-class FONT_SIZE(Enum):
-
-    xx_small = 0
-    x_small = 1
-    small = 2
-    medium = 3
-    large = 4
-    x_large = 5
-    xx_large = 6
-
-    def get_name(self) -> str:
-
-        return {
-            'xx_small': 'xx-small',
-            'x_small': 'x-small',
-            'small': 'small',
-            'medium': 'medium',
-            'large': 'large',
-            'x_large': 'x-large',
-            'xx_large': 'xx-large'
-        }[self.name]
-
-    @staticmethod
-    def get_font_size(
-            font_size: Union[int, float, 'FONT_SIZE']
-    ) -> Union[str, int, float]:
-        if font_size and isinstance(font_size, FONT_SIZE):
-            font_size = font_size.get_name()
-        return font_size
+from enum import Enum
+from typing import Union
+
+
+class FONT_SIZE(Enum):
+
+    xx_small = 0
+    x_small = 1
+    small = 2
+    medium = 3
+    large = 4
+    x_large = 5
+    xx_large = 6
+
+    def get_name(self) -> str:
+
+        return {
+            'xx_small': 'xx-small',
+            'x_small': 'x-small',
+            'small': 'small',
+            'medium': 'medium',
+            'large': 'large',
+            'x_large': 'x-large',
+            'xx_large': 'xx-large'
+        }[self.name]
+
+    @staticmethod
+    def get_font_size(
+            font_size: Union[int, float, 'FONT_SIZE']
+    ) -> Union[str, int, float]:
+        if font_size and isinstance(font_size, FONT_SIZE):
+            font_size = font_size.get_name()
+        return font_size
```

### Comparing `mpl_format-0.317/mpl_format/enums/font_stretch.py` & `mpl_format-0.318/mpl_format/enums/font_stretch.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from enum import Enum
-from typing import Union
-
-
-class FONT_STRETCH(Enum):
-
-    ultra_condensed = 0
-    extra_condensed = 1
-    condensed = 2
-    semi_condensed = 3
-    normal = 4
-    semi_expanded = 5
-    expanded = 6
-    extra_expanded = 7
-    ultra_expanded = 8
-
-    def get_name(self) -> str:
-
-        return {
-            'ultra_condensed': 'ultra-condensed',
-            'extra_condensed': 'extra-condensed',
-            'condensed': 'condensed',
-            'semi_condensed': 'semi-condensed',
-            'normal': 'normal',
-            'semi_expanded': 'semi-expanded',
-            'expanded': 'expanded',
-            'extra_expanded': 'extra-expanded',
-            'ultra_expanded': 'ultra-expanded'
-        }[self.name]
-
-    @staticmethod
-    def get_font_stretch(
-            font_stretch: Union[int, float, 'FONT_STRETCH']
-    ) -> Union[str, int, float]:
-        if font_stretch and isinstance(font_stretch, FONT_STRETCH):
-            font_stretch = font_stretch.get_name()
-        return font_stretch
+from enum import Enum
+from typing import Union
+
+
+class FONT_STRETCH(Enum):
+
+    ultra_condensed = 0
+    extra_condensed = 1
+    condensed = 2
+    semi_condensed = 3
+    normal = 4
+    semi_expanded = 5
+    expanded = 6
+    extra_expanded = 7
+    ultra_expanded = 8
+
+    def get_name(self) -> str:
+
+        return {
+            'ultra_condensed': 'ultra-condensed',
+            'extra_condensed': 'extra-condensed',
+            'condensed': 'condensed',
+            'semi_condensed': 'semi-condensed',
+            'normal': 'normal',
+            'semi_expanded': 'semi-expanded',
+            'expanded': 'expanded',
+            'extra_expanded': 'extra-expanded',
+            'ultra_expanded': 'ultra-expanded'
+        }[self.name]
+
+    @staticmethod
+    def get_font_stretch(
+            font_stretch: Union[int, float, 'FONT_STRETCH']
+    ) -> Union[str, int, float]:
+        if font_stretch and isinstance(font_stretch, FONT_STRETCH):
+            font_stretch = font_stretch.get_name()
+        return font_stretch
```

### Comparing `mpl_format-0.317/mpl_format/enums/mappings.py` & `mpl_format-0.318/mpl_format/enums/mappings.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Dict, Callable
-
-from mpl_format.enums import \
-    FONT_SIZE, FONT_STRETCH, FONT_STYLE, FONT_VARIANT, FONT_WEIGHT, \
-    BOX_STYLE, CAP_STYLE, JOIN_STYLE, LINE_STYLE
-
-
-kwarg_mappings: Dict[str, Callable] = {
-    'boxstyle': BOX_STYLE.get_box_style,
-    'capstyle': CAP_STYLE.get_cap_style,
-    'fontsize': FONT_SIZE.get_font_size,
-    'fontstretch': FONT_STRETCH.get_font_stretch,
-    'fontstyle': FONT_STYLE.get_font_style,
-    'fontvariant': FONT_VARIANT.get_font_variant,
-    'fontweight': FONT_WEIGHT.get_font_weight,
-    'joinstyle': JOIN_STYLE.get_join_style,
-    'linestyle': LINE_STYLE.get_line_style
-}
+from typing import Dict, Callable
+
+from mpl_format.enums import \
+    FONT_SIZE, FONT_STRETCH, FONT_STYLE, FONT_VARIANT, FONT_WEIGHT, \
+    BOX_STYLE, CAP_STYLE, JOIN_STYLE, LINE_STYLE
+
+
+kwarg_mappings: Dict[str, Callable] = {
+    'boxstyle': BOX_STYLE.get_box_style,
+    'capstyle': CAP_STYLE.get_cap_style,
+    'fontsize': FONT_SIZE.get_font_size,
+    'fontstretch': FONT_STRETCH.get_font_stretch,
+    'fontstyle': FONT_STYLE.get_font_style,
+    'fontvariant': FONT_VARIANT.get_font_variant,
+    'fontweight': FONT_WEIGHT.get_font_weight,
+    'joinstyle': JOIN_STYLE.get_join_style,
+    'linestyle': LINE_STYLE.get_line_style
+}
```

### Comparing `mpl_format-0.317/mpl_format/enums/marker_style.py` & `mpl_format-0.318/mpl_format/enums/marker_style.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from enum import Enum
-from typing import Union
-
-
-class MARKER_STYLE(Enum):
-
-    nothing = 0
-    point = 1
-    pixel = 2
-    circle = 3
-    triangle_down = 4
-    triangle_up = 5
-    triangle_left = 6
-    triangle_right = 7
-    octagon = 8
-    square = 9
-    pentagon = 10
-    star = 11
-    hexagon_1 = 12
-    hexagon_2 = 13
-    plus = 14
-    cross = 15
-    diamond = 16
-    diamond_thin = 17
-    v_line = 18
-    h_line = 19
-    plus_filled = 20
-    cross_filled = 21
-    tick_left = 22
-    tick_right = 23
-    tick_up = 24
-    tick_down = 25
-    caret_left = 26
-    caret_right = 27
-    caret_up = 28
-    caret_down = 29
-    caret_left_base = 30
-    caret_right_base = 31
-    caret_up_base = 32
-    caret_down_base = 33
-
-    def get_name(self) -> str:
-
-        return {
-            'nothing': 'nothing',
-            'point': 'point',
-            'pixel': 'pixel',
-            'circle': 'circle',
-            'triangle_down': 'triangle_down',
-            'triangle_up': 'triangle_up',
-            'triangle_left': 'triangle_left',
-            'triangle_right': 'triangle_right',
-            'octagon': 'octagon',
-            'square': 'square',
-            'pentagon': 'pentagon',
-            'star': 'star',
-            'hexagon_1': 'hexagon1',
-            'hexagon_2': 'hexagon2',
-            'plus': 'plus',
-            'cross': 'x',
-            'diamond': 'diamond',
-            'diamond_thin': 'thin_diamond',
-            'v_line': 'vline',
-            'h_line': 'hline',
-            'plus_filled': 'plus_filled',
-            'cross_filled': 'x_filled',
-            'tick_left': 'tickleft',
-            'tick_right': 'tickright',
-            'tick_up': 'tickup',
-            'tick_down': 'tickdown',
-            'caret_left': 'caretleft',
-            'caret_right': 'caretright',
-            'caret_up': 'caretup',
-            'caret_down': 'caretdown',
-            'caret_left_base': 'caretleftbase',
-            'caret_right_base': 'caretrightbase',
-            'caret_up_base': 'caretupbase',
-            'caret_down_base': 'caretdownbase'
-        }[self.name]
-
-    @staticmethod
-    def get_marker_style(
-            marker_style: Union[int, float, 'MARKER_STYLE']
-    ) -> Union[str, int, float]:
-        if marker_style and isinstance(marker_style, MARKER_STYLE):
-            marker_style = marker_style.get_name()
-        return marker_style
+from enum import Enum
+from typing import Union
+
+
+class MARKER_STYLE(Enum):
+
+    nothing = 0
+    point = 1
+    pixel = 2
+    circle = 3
+    triangle_down = 4
+    triangle_up = 5
+    triangle_left = 6
+    triangle_right = 7
+    octagon = 8
+    square = 9
+    pentagon = 10
+    star = 11
+    hexagon_1 = 12
+    hexagon_2 = 13
+    plus = 14
+    cross = 15
+    diamond = 16
+    diamond_thin = 17
+    v_line = 18
+    h_line = 19
+    plus_filled = 20
+    cross_filled = 21
+    tick_left = 22
+    tick_right = 23
+    tick_up = 24
+    tick_down = 25
+    caret_left = 26
+    caret_right = 27
+    caret_up = 28
+    caret_down = 29
+    caret_left_base = 30
+    caret_right_base = 31
+    caret_up_base = 32
+    caret_down_base = 33
+
+    def get_name(self) -> str:
+
+        return {
+            'nothing': 'nothing',
+            'point': 'point',
+            'pixel': 'pixel',
+            'circle': 'circle',
+            'triangle_down': 'triangle_down',
+            'triangle_up': 'triangle_up',
+            'triangle_left': 'triangle_left',
+            'triangle_right': 'triangle_right',
+            'octagon': 'octagon',
+            'square': 'square',
+            'pentagon': 'pentagon',
+            'star': 'star',
+            'hexagon_1': 'hexagon1',
+            'hexagon_2': 'hexagon2',
+            'plus': 'plus',
+            'cross': 'x',
+            'diamond': 'diamond',
+            'diamond_thin': 'thin_diamond',
+            'v_line': 'vline',
+            'h_line': 'hline',
+            'plus_filled': 'plus_filled',
+            'cross_filled': 'x_filled',
+            'tick_left': 'tickleft',
+            'tick_right': 'tickright',
+            'tick_up': 'tickup',
+            'tick_down': 'tickdown',
+            'caret_left': 'caretleft',
+            'caret_right': 'caretright',
+            'caret_up': 'caretup',
+            'caret_down': 'caretdown',
+            'caret_left_base': 'caretleftbase',
+            'caret_right_base': 'caretrightbase',
+            'caret_up_base': 'caretupbase',
+            'caret_down_base': 'caretdownbase'
+        }[self.name]
+
+    @staticmethod
+    def get_marker_style(
+            marker_style: Union[int, float, 'MARKER_STYLE']
+    ) -> Union[str, int, float]:
+        if marker_style and isinstance(marker_style, MARKER_STYLE):
+            marker_style = marker_style.get_name()
+        return marker_style
```

### Comparing `mpl_format-0.317/mpl_format/figures/figure_formatter.py` & `mpl_format-0.318/mpl_format/figures/figure_formatter.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,896 +1,896 @@
-from pathlib import Path
-from typing import Tuple, Union, Callable, List, Optional, TypeVar
-
-import matplotlib.pyplot as plt
-from matplotlib.axes import Axes
-from matplotlib.figure import Figure
-from numpy import ndarray, reshape
-from numpy.ma import empty_like
-
-from mpl_format.compound_types import Scalar
-from mpl_format.axes import AxisFormatter
-from mpl_format.axes.axes_formatter import AxesFormatter
-from mpl_format.axes.axes_formatter_array import AxesFormatterArray
-from mpl_format.axes.axis_formatter_array import AxisFormatterArray
-from mpl_format.compound_types import StringMapper, Color
-from mpl_format.enums.line_style import LINE_STYLE
-from mpl_format.literals import ROTATION_MODE, WHICH_TICKS, SHARE_AXES, \
-    WHICH_AXIS
-from mpl_format.utils.io_utils import save_plot
-
-TextSetter = TypeVar(
-    'TextSetter',
-    str, List[str], Callable[[int, int], str], Callable[[int], str]
-)
-
-
-class FigureFormatter(object):
-
-    share_values = ('all', 'row', 'col', 'none')
-
-    def __init__(self, fig_or_axes: Union[Figure, Axes] = None,
-                 n_rows: int = 1, n_cols: int = 1,
-                 fig_size: Tuple[Scalar, Scalar] = (16, 9),
-                 share_x: SHARE_AXES = 'none',
-                 share_y: SHARE_AXES = 'none',
-                 constrained_layout: bool = True):
-
-        if fig_or_axes is not None:
-            if isinstance(fig_or_axes, Figure):
-                self._figure = fig_or_axes
-                axes_list = self._figure.axes
-                rows_cols = (
-                    axes_list[0].get_subplotspec().get_topmost_subplotspec()
-                                .get_gridspec().get_geometry()
-                )
-                self._axes = reshape(axes_list, rows_cols)
-            elif isinstance(fig_or_axes, Axes):
-                self._figure = fig_or_axes.figure
-                self._axes = fig_or_axes
-            else:
-                raise ValueError('Can only instantiate a new FigureFormatter '
-                                 'from an Axes or Figure instance.')
-        else:
-            if share_x not in self.share_values:
-                raise ValueError(f'share_x must be in {self.share_values}')
-            if share_y not in self.share_values:
-                raise ValueError(f'share_y must be in {self.share_values}')
-            self._fig_size: Tuple[int, int] = fig_size
-            figure, axes = plt.subplots(
-                nrows=n_rows, ncols=n_cols,
-                sharex=share_x, sharey=share_y,
-                figsize=fig_size,
-                constrained_layout=constrained_layout
-            )
-            self._axes: Union[Axes, ndarray] = axes
-            self._figure: Figure = figure
-        self._has_array = (
-                isinstance(self._axes, ndarray) or isinstance(self._axes, list)
-        )
-
-    @staticmethod
-    def gcf() -> 'FigureFormatter':
-
-        return FigureFormatter(fig_or_axes=plt.gcf())
-
-    # region properties
-
-    @property
-    def axes(self) -> Union[AxesFormatter, AxesFormatterArray]:
-        """
-        Return an AxesFormatter or AxesFormatterArray for the wrapped Axes or
-        array of Axes.
-        """
-        if not self._has_array:
-            return AxesFormatter(self._axes)
-        else:
-            return AxesFormatterArray(self._axes)
-
-    @property
-    def x_axes(self) -> Union[AxisFormatter, AxisFormatterArray]:
-        """
-        Return an AxisFormatter or AxisFormatterArray for the X-Axis or X-Axes
-        of the wrapped Axes.
-        """
-        if not self._has_array:
-            return AxesFormatter(self._axes).x_axis
-        else:
-            axes = empty_like(self._axes, dtype=AxisFormatter)
-            if axes.ndim == 1:
-                for i in range(self._axes.shape[0]):
-                    axes[i] = AxisFormatter(
-                        axis=self._axes[i].xaxis,
-                        direction='x',
-                        axes=self._axes[i]
-                    )
-            elif axes.ndim == 2:
-                for i in range(axes.shape[0]):
-                    for j in range(axes.shape[1]):
-                        axes[i, j] = AxisFormatter(
-                            axis=self._axes[i, j].xaxis,
-                            direction='x',
-                            axes=self._axes[i, j]
-                        )
-
-        return AxisFormatterArray(axes)
-
-    @property
-    def y_axes(self) -> Union[AxisFormatter, AxisFormatterArray]:
-        """
-        Return an AxisFormatter or AxisFormatterArray for the Y-Axis or Y-Axes
-        of the wrapped Axes.
-        """
-        if not self._has_array:
-            return AxesFormatter(self._axes).y_axis
-        else:
-            axes = empty_like(self._axes, dtype=AxisFormatter)
-            if axes.ndim == 1:
-                for i in range(self._axes.shape[0]):
-                    axes[i] = AxisFormatter(
-                        axis=self._axes[i].yaxis,
-                        direction='y',
-                        axes=self._axes[i]
-                    )
-            elif axes.ndim == 2:
-                for i in range(axes.shape[0]):
-                    for j in range(axes.shape[1]):
-                        axes[i, j] = AxisFormatter(
-                            axis=self._axes[i, j].yaxis,
-                            direction='y',
-                            axes=self._axes[i, j]
-                        )
-
-        return AxisFormatterArray(axes)
-
-    @property
-    def figure(self) -> Figure:
-        return self._figure
-
-    @property
-    def single(self) -> AxesFormatter:
-        """
-        Return an AxesFormatter for the wrapped Axes.
-        """
-        if not self._has_array:
-            return AxesFormatter(self._axes)
-        else:
-            raise TypeError('FigureFormatter holds an array of Axes.')
-
-    @property
-    def multi(self) -> AxesFormatterArray:
-        """
-        Return an AxesFormatterArray for the wrapped Axes.
-        """
-        if self._has_array:
-            return AxesFormatterArray(self._axes)
-        else:
-            raise TypeError('FigureFormatter holds a single Axes.')
-
-    # endregion
-
-    # region set text
-
-    def _set_text_property(
-            self,
-            text: TextSetter,
-            method: Callable[[AxesFormatter, str], AxesFormatter]
-    ) -> 'FigureFormatter':
-        """
-        Set a text property of each Axes using a string, list of strings,
-        or function that returns a string based on the row and column or the
-        flat index of the Axes.
-
-        :param text: Title or titles to set
-        :param method: Method to call to format the text.
-        """
-        if not self._has_array:
-            if not isinstance(text, str):
-                raise TypeError('text must be a str for a single Axes.')
-            else:
-                method(self.single, text)
-        else:
-            if isinstance(text, str):
-                for axf in self.multi.flat:
-                    method(axf, text)
-            elif isinstance(text, list):
-                if len(text) != self.multi.size:
-                    raise ValueError(f'There are {self.multi.size} Axes'
-                                     f' and {len(text)} strings.')
-                else:
-                    for axf, t in zip(self.multi.flat, text):
-                        method(axf, t)
-            elif callable(text):
-                try:
-                    for row in range(self.multi.shape[0]):
-                        for col in range(self.multi.shape[1]):
-                            method(self.multi[row, col], text(row, col))
-                except TypeError:
-                    for a, axf in enumerate(self.multi.flat):
-                        method(axf, text(a))
-            else:
-                raise TypeError(
-                    f'Wrong type passed to _set_text_property: {type(text)}'
-                )
-        return self
-
-    def set_title(self, text) -> 'FigureFormatter':
-        """
-        Set the title of the Figure.
-
-        :param text: The text for the title.
-        """
-        self._figure.suptitle(t=text)
-        return self
-
-    def set_axes_title_text(
-            self,
-            text: TextSetter
-    ) -> 'FigureFormatter':
-        """
-        Set the title text of each Axes using a string, list of strings,
-        or function that returns a string based on the row and column or the
-        flat index of the Axes.
-
-        :param text: Title or titles to set.
-        """
-        def set_text(
-                axes_formatter: AxesFormatter, string: str
-        ) -> AxesFormatter:
-            return axes_formatter.set_title_text(string)
-
-        self._set_text_property(text=text, method=set_text)
-        return self
-
-    def map_axes_title_text(
-            self, mapping: StringMapper
-    ) -> 'FigureFormatter':
-        """
-        Map the label text for the x-axis using a dictionary or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        if not self._has_array:
-            self.single.map_title_text(mapping=mapping)
-        else:
-            for axf in self.multi.flat:
-                axf.map_title_text(mapping=mapping)
-        return self
-
-    def set_axes_x_label_text(
-            self,
-            text: TextSetter
-    ) -> 'FigureFormatter':
-        """
-        Set the x-label text of each Axes using a string, list of strings,
-        or function that returns a string based on the row and column or the
-        flat index of the Axes.
-
-        :param text: Label or labels to set.
-        """
-        def set_text(
-                axes_formatter: AxesFormatter, string: str
-        ) -> AxesFormatter:
-            return axes_formatter.set_x_label_text(string)
-
-        self._set_text_property(text=text, method=set_text)
-        return self
-
-    def set_axes_y_label_text(
-            self, text: TextSetter
-    ) -> 'FigureFormatter':
-        """
-        Set the x-label text of each Axes using a string, list of strings,
-        or function that returns a string based on the row and column or the
-        flat index of the Axes.
-
-        :param text: Label or labels to set.
-        """
-        def set_text(
-                axes_formatter: AxesFormatter, string: str
-        ) -> AxesFormatter:
-            return axes_formatter.set_y_label_text(string)
-
-        self._set_text_property(text=text, method=set_text)
-        return self
-
-    def set_axes_text(
-            self,
-            title: Optional[TextSetter] = None,
-            x_label: Optional[TextSetter] = None,
-            y_label: Optional[TextSetter] = None
-    ) -> 'FigureFormatter':
-        """
-        Set the text for each Axes' title, x_label or y_label.
-
-        :param title: Axes titles.
-        :param x_label: Axes x-labels.
-        :param y_label: Axes y-labels.
-        """
-        if title is not None:
-            self.set_axes_title_text(title)
-        if x_label is not None:
-            self.set_axes_x_label_text(x_label)
-        if y_label is not None:
-            self.set_axes_y_label_text(y_label)
-        return self
-
-    # endregion
-
-    # region wrap text
-
-    def wrap_titles(self, max_width: int) -> 'FigureFormatter':
-        """
-        Wrap the text for each Axes title if it exceeds a given width
-        of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        if not self._has_array:
-            self.single.wrap_title(max_width=max_width)
-        else:
-            for axf in self.multi.flat:
-                axf.wrap_title(max_width=max_width)
-        return self
-
-    def wrap_x_labels(self, max_width: int) -> 'FigureFormatter':
-        """
-        Wrap the text for each X-Axis label if it exceeds a given width
-        of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.wrap_x_label(max_width=max_width)
-        else:
-            self.single.wrap_x_label(max_width=max_width)
-        return self
-
-    def wrap_y_labels(self, max_width: int) -> 'FigureFormatter':
-        """
-        Wrap the text for each Y-Axis label if it exceeds a given width
-        of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.wrap_y_label(max_width=max_width)
-        else:
-            self.single.wrap_y_label(max_width=max_width)
-        return self
-
-    def wrap_axes_labels(self, max_width: int) -> 'FigureFormatter':
-        """
-        Wrap the text for each Axis label if it exceeds a given width
-        of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        self.wrap_x_labels(max_width=max_width)
-        self.wrap_y_labels(max_width=max_width)
-        return self
-
-    def wrap_x_tick_labels(self, max_width: int) -> 'FigureFormatter':
-        """
-        Wrap the text for each tick label on each x-axis if it exceeds a
-        given width of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.x_ticks.wrap_label_text(max_width=max_width)
-        else:
-            self.single.x_ticks.wrap_label_text(max_width=max_width)
-        return self
-
-    def wrap_y_tick_labels(self, max_width: int) -> 'FigureFormatter':
-        """
-        Wrap the text for each tick label on each y-axis if it exceeds a
-        given width of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.y_ticks.wrap_label_text(max_width=max_width)
-        else:
-            self.single.y_ticks.wrap_label_text(max_width=max_width)
-        return self
-
-    def wrap_tick_labels(self, max_width: int) -> 'FigureFormatter':
-        """
-        Wrap the text for each tick label on each x- and y-axis if it exceeds a
-        given width of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        self.wrap_x_tick_labels(max_width=max_width)
-        self.wrap_y_tick_labels(max_width=max_width)
-        return self
-
-    # endregion
-
-    # region map labels
-
-    def map_x_axis_labels(
-            self, mapping: StringMapper
-    ) -> 'FigureFormatter':
-        """
-        Map the label text for each x-axis in the Figure using a dictionary
-        or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.map_x_axis_label(mapping=mapping)
-        else:
-            self.single.map_x_axis_label(mapping=mapping)
-        return self
-
-    def map_y_axis_labels(
-            self, mapping: StringMapper
-    ) -> 'FigureFormatter':
-        """
-        Map the label text for each y-axis in the Figure using a dictionary
-        or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.map_y_axis_label(mapping=mapping)
-        else:
-            self.single.map_y_axis_label(mapping=mapping)
-        return self
-
-    def map_axis_labels(
-            self, mapping: StringMapper
-    ) -> 'FigureFormatter':
-        """
-        Map the label text for each axis in the Figure using a dictionary
-        or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        self.map_x_axis_labels(mapping=mapping)
-        self.map_y_axis_labels(mapping=mapping)
-        return self
-
-    def map_x_tick_labels(
-            self, mapping: StringMapper
-    ) -> 'FigureFormatter':
-        """
-        Map the tick label text for each x-axis using a dictionary or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.x_ticks.map_label_text(mapping=mapping)
-        else:
-            self.single.x_ticks.map_label_text(mapping=mapping)
-        return self
-
-    def map_y_tick_labels(
-            self, mapping: StringMapper
-    ) -> 'FigureFormatter':
-        """
-        Map the tick label text for each y-axis using a dictionary or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.y_ticks.map_label_text(mapping=mapping)
-        else:
-            self.single.y_ticks.map_label_text(mapping=mapping)
-        return self
-
-    def map_tick_labels(
-            self, mapping: StringMapper
-    ) -> 'FigureFormatter':
-        """
-        Map the tick label text for each axis using a dictionary or function.
-
-        :param mapping: Dictionary or a function mapping old text to new text.
-        """
-        self.map_x_tick_labels(mapping=mapping)
-        self.map_y_tick_labels(mapping=mapping)
-        return self
-
-    # endregion
-
-    # region remove
-
-    def remove_titles(self) -> 'FigureFormatter':
-        """
-        Remove the title from each Axes.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.remove_title()
-        else:
-            self.single.remove_title()
-        return self
-
-    def remove_legends(self) -> 'FigureFormatter':
-        """
-        Remove the legend from each Axes.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.remove_legend()
-        else:
-            self.single.remove_legend()
-        return self
-
-    def remove_x_ticks(self) -> 'FigureFormatter':
-        """
-        Remove x-ticks from each Axes.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.remove_x_ticks()
-        else:
-            self.single.remove_x_ticks()
-        return self
-
-    def remove_y_ticks(self) -> 'FigureFormatter':
-        """
-        Remove y-ticks from each Axes.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.remove_y_ticks()
-        else:
-            self.single.remove_y_ticks()
-        return self
-
-    def remove_axes_ticks(self) -> 'FigureFormatter':
-        """
-        Remove ticks from each Axes.
-        """
-        self.remove_x_ticks()
-        self.remove_y_ticks()
-        return self
-
-    def remove_x_labels(self) -> 'FigureFormatter':
-        """
-        Remove the x-axis label from each Axes in the Figure.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.remove_x_label()
-        else:
-            self.single.remove_x_label()
-        return self
-
-    def remove_y_labels(self) -> 'FigureFormatter':
-        """
-        Remove the y-axis label from each Axes in the Figure.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.remove_y_label()
-        else:
-            self.single.remove_y_label()
-        return self
-
-    def remove_axes_labels(self) -> 'FigureFormatter':
-        """
-        Remove the x-axis label for each Axes in the Figure.
-        """
-        self.remove_x_labels()
-        self.remove_y_labels()
-        return self
-
-    # endregion
-
-    # region rotation
-
-    def rotate_x_labels(self,
-                        rotation: int,
-                        how: ROTATION_MODE = 'absolute') -> 'FigureFormatter':
-        """
-        Set the rotation of each x-axis label.
-
-        :param rotation: The rotation value to set in degrees.
-        :param how: 'absolute' or 'relative'
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.rotate_x_label(rotation=rotation, how=how)
-        else:
-            self.single.rotate_x_label(rotation=rotation, how=how)
-        return self
-
-    def rotate_y_labels(self,
-                        rotation: int,
-                        how: ROTATION_MODE = 'absolute') -> 'FigureFormatter':
-        """
-        Set the rotation of each x-axis label.
-
-        :param rotation: The rotation value to set in degrees.
-        :param how: 'absolute' or 'relative'
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.rotate_y_label(rotation=rotation, how=how)
-        else:
-            self.single.rotate_y_label(rotation=rotation, how=how)
-        return self
-
-    def rotate_x_tick_labels(self,
-                             rotation: int) -> 'FigureFormatter':
-        """
-        Set the rotation of each x-axis' tick-labels.
-
-        :param rotation: The rotation value to set in degrees.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.x_ticks.set_label_rotation(rotation=rotation)
-        else:
-            self.single.x_ticks.set_label_rotation(rotation=rotation)
-        return self
-
-    def rotate_y_tick_labels(self,
-                             rotation: int) -> 'FigureFormatter':
-        """
-        Set the rotation of each y-axis' tick-labels.
-
-        :param rotation: The rotation value to set in degrees.
-        """
-        if self._has_array:
-            for axf in self.multi.flat:
-                axf.y_ticks.set_label_rotation(rotation=rotation)
-        else:
-            self.single.y_ticks.set_label_rotation(rotation=rotation)
-        return self
-
-    # endregion
-
-    # region margins
-
-    def subplots_adjust(
-            self,
-            left: Optional[float] = None, right: Optional[float] = None,
-            top: Optional[float] = None, bottom: Optional[float] = None,
-            w_space: Optional[float] = None, h_space: Optional[float] = None
-    ) -> 'FigureFormatter':
-        """
-        Adjust the padding of the Figure.
-
-        :param left: The position of the left edge of the subplots,
-                     as a fraction of the figure width. Use 0 for no margin.
-        :param right: The position of the right edge of the subplots,
-                      as a fraction of the figure width. Use 1 for no margin.
-        :param top: The position of the top edge of the subplots,
-                    as a fraction of the figure height. Use 1 for no margin.
-        :param bottom: The position of the bottom edge of the subplots,
-                       as a fraction of the figure height. Use 0 for no margin.
-        :param w_space: The width of the padding between subplots,
-                        as a fraction of the average axes width.
-        :param h_space: The height of the padding between subplots,
-                        as a fraction of the average axes height.
-        """
-        self.figure.subplots_adjust(
-            left=left, right=right,
-            bottom=bottom, top=top,
-            wspace=w_space, hspace=h_space
-        )
-        return self
-
-    def set_left_margin(self, margin_size: float) -> 'FigureFormatter':
-        """
-        Set the margin size at the left of the plot.
-
-        :param margin_size: Value between 0 and 1. 0 for no margin
-        """
-        self.subplots_adjust(left=margin_size)
-        return self
-
-    def set_right_margin(self, margin_size: float) -> 'FigureFormatter':
-        """
-        Set the margin size at the right of the plot.
-
-        :param margin_size: Value between 0 and 1. 0 for no margin
-        """
-        self.subplots_adjust(right=1 - margin_size)
-        return self
-
-    def set_top_margin(self, margin_size: float) -> 'FigureFormatter':
-        """
-        Set the margin size at the top of the plot.
-
-        :param margin_size: Value between 0 and 1. 0 for no margin
-        """
-        self.subplots_adjust(top=1 - margin_size)
-        return self
-
-    def set_bottom_margin(self, margin_size: float) -> 'FigureFormatter':
-        """
-        Set the margin size at the bottom of the plot.
-
-        :param margin_size: Value between 0 and 1. 0 for no margin
-        """
-        self.subplots_adjust(bottom=margin_size)
-        return self
-
-    def set_horizontal_margin(self, margin_size: float) -> 'FigureFormatter':
-        """
-        Set the margin size at the left and right of the plot.
-
-        :param margin_size: Value between 0 and 1. 0 for no margin
-        """
-        self.subplots_adjust(left=margin_size, right=1 - margin_size)
-        return self
-
-    def set_vertical_margin(self, margin_size: float) -> 'FigureFormatter':
-        """
-        Set the margin size at the top and bottom of the plot.
-
-        :param margin_size: Value between 0 and 1. 0 for no margin
-        """
-        self.subplots_adjust(bottom=margin_size, top=1 - margin_size)
-        return self
-
-    def set_margin(self, margin_size: float) -> 'FigureFormatter':
-        """
-        Set the margin size at the top of the plot.
-
-        :param margin_size: Value between 0 and 1. 0 for no margin
-        """
-        self.subplots_adjust(bottom=margin_size, top=1 - margin_size,
-                             left=margin_size, right=1 - margin_size)
-        return self
-
-    def set_horizontal_spacing(self, spacing: float) -> 'FigureFormatter':
-        """
-        Set the horizontal spacing between each subplot.
-
-        :param spacing: The width of the padding between subplots,
-                        as a fraction of the average axes width.
-        """
-        self.subplots_adjust(w_space=spacing)
-        return self
-
-    def set_vertical_spacing(self, spacing: float) -> 'FigureFormatter':
-        """
-        Set the vertical spacing between each subplot.
-
-        :param spacing: The height of the padding between subplots,
-                        as a fraction of the average axes height.
-        """
-        self.subplots_adjust(h_space=spacing)
-        return self
-
-    # endregion
-
-    def grids(
-            self, value: bool = True,
-            which: WHICH_TICKS = 'major',
-            axis: WHICH_AXIS = 'both',
-            color: Optional[Color] = None,
-            line_width: Optional[float] = None,
-            line_style: Optional[Union[str, LINE_STYLE]] = None
-    ) -> 'FigureFormatter':
-        """
-        Turn the grid on or off.
-
-        :param value: True or False. Defaults to True.
-        :param which: 'major', 'minor' or 'both'
-        :param axis: 'x', 'y' or 'both.
-        :param color: Color of the lines.
-        :param line_width: Line width.
-        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
-                           (offset, on-off-seq), ...}
-        """
-        for axes in self.axes.flat:
-            axes.grid(value=value, which=which, axis=axis,
-                      color=color, line_width=line_width,
-                      line_style=line_style)
-        return self
-
-    def set_axes_below(self, value: bool = True) -> 'FigureFormatter':
-        """
-        Set whether axis ticks and gridlines are above or below most artists.
-
-        :param value: True or False
-        """
-        for axes in self.axes.flat:
-            axes.set_axis_below(value=value)
-        return self
-
-    def tight_layout(self) -> 'FigureFormatter':
-        """
-        Call the tight_layout method on the wrapped Figure.
-        """
-        self.figure.tight_layout()
-        return self
-
-    # region limits
-
-    def set_x_lims(self, left: Optional[float] = None,
-                   right: Optional[float] = None) -> 'FigureFormatter':
-        """
-        Set the limits of the x-axes.
-
-        :param left: Lower limit.
-        :param right: Upper limit.
-        """
-        for axf in self.multi.flat:
-            axf.set_x_lim(left=left, right=right)
-        return self
-
-    def set_y_lims(self, bottom: Optional[float] = None,
-                   top: Optional[float] = None) -> 'FigureFormatter':
-        """
-        Set the limits of the y-axes.
-
-        :param bottom: Lower limit.
-        :param top: Upper limit.
-        """
-        for axf in self.multi.flat:
-            axf.set_y_lim(bottom=bottom, top=top)
-        return self
-
-    def set_x_mins(self, left: float = None) -> 'FigureFormatter':
-        """
-        Set the x-axes lower view limit.
-        """
-        self.set_x_lims(left, None)
-        return self
-
-    def set_x_maxes(self, right: float = None) -> 'FigureFormatter':
-        """
-        Set the x-axes upper view limit.
-        """
-        self.set_x_lims(None, right)
-        return self
-
-    def set_y_mins(self, bottom: float = None) -> 'FigureFormatter':
-        """
-        Set the y-axes lower view limit.
-        """
-        self.set_y_lims(bottom, None)
-        return self
-
-    def set_y_maxes(self, top: float = None) -> 'FigureFormatter':
-        """
-        Set the y-axes upper view limit.
-        """
-        self.set_y_lims(None, top)
-        return self
-
-    # endregion
-
-    def save(
-            self,
-            file_path: Union[str, Path],
-            file_type: Optional[str] = None
-    ) -> 'FigureFormatter':
-        """
-        Save the plot to disk.
-
-        :param file_path: The file path to save the plot object to.
-        :param file_type: The type of file to save.
-                          Defaults to png if can't be auto-detected from name.
-        """
-        save_plot(plot_object=self._figure,
-                  file_path=file_path, file_type=file_type)
-        return self
-
-    def show(self) -> 'FigureFormatter':
-        """
-        Show the figure.
-        """
-        plt.show()
-        return self
-
-    def __getitem__(self, *args, **kwargs) -> AxesFormatter:
-
-        return self.multi.__getitem__(*args, **kwargs)
+from pathlib import Path
+from typing import Tuple, Union, Callable, List, Optional, TypeVar
+
+import matplotlib.pyplot as plt
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
+from numpy import ndarray, reshape
+from numpy.ma import empty_like
+
+from mpl_format.compound_types import Scalar
+from mpl_format.axes import AxisFormatter
+from mpl_format.axes.axes_formatter import AxesFormatter
+from mpl_format.axes.axes_formatter_array import AxesFormatterArray
+from mpl_format.axes.axis_formatter_array import AxisFormatterArray
+from mpl_format.compound_types import StringMapper, Color
+from mpl_format.enums.line_style import LINE_STYLE
+from mpl_format.literals import ROTATION_MODE, WHICH_TICKS, SHARE_AXES, \
+    WHICH_AXIS
+from mpl_format.utils.io_utils import save_plot
+
+TextSetter = TypeVar(
+    'TextSetter',
+    str, List[str], Callable[[int, int], str], Callable[[int], str]
+)
+
+
+class FigureFormatter(object):
+
+    share_values = ('all', 'row', 'col', 'none')
+
+    def __init__(self, fig_or_axes: Union[Figure, Axes] = None,
+                 n_rows: int = 1, n_cols: int = 1,
+                 fig_size: Tuple[Scalar, Scalar] = (16, 9),
+                 share_x: SHARE_AXES = 'none',
+                 share_y: SHARE_AXES = 'none',
+                 constrained_layout: bool = True):
+
+        if fig_or_axes is not None:
+            if isinstance(fig_or_axes, Figure):
+                self._figure = fig_or_axes
+                axes_list = self._figure.axes
+                rows_cols = (
+                    axes_list[0].get_subplotspec().get_topmost_subplotspec()
+                                .get_gridspec().get_geometry()
+                )
+                self._axes = reshape(axes_list, rows_cols)
+            elif isinstance(fig_or_axes, Axes):
+                self._figure = fig_or_axes.figure
+                self._axes = fig_or_axes
+            else:
+                raise ValueError('Can only instantiate a new FigureFormatter '
+                                 'from an Axes or Figure instance.')
+        else:
+            if share_x not in self.share_values:
+                raise ValueError(f'share_x must be in {self.share_values}')
+            if share_y not in self.share_values:
+                raise ValueError(f'share_y must be in {self.share_values}')
+            self._fig_size: Tuple[int, int] = fig_size
+            figure, axes = plt.subplots(
+                nrows=n_rows, ncols=n_cols,
+                sharex=share_x, sharey=share_y,
+                figsize=fig_size,
+                constrained_layout=constrained_layout
+            )
+            self._axes: Union[Axes, ndarray] = axes
+            self._figure: Figure = figure
+        self._has_array = (
+                isinstance(self._axes, ndarray) or isinstance(self._axes, list)
+        )
+
+    @staticmethod
+    def gcf() -> 'FigureFormatter':
+
+        return FigureFormatter(fig_or_axes=plt.gcf())
+
+    # region properties
+
+    @property
+    def axes(self) -> Union[AxesFormatter, AxesFormatterArray]:
+        """
+        Return an AxesFormatter or AxesFormatterArray for the wrapped Axes or
+        array of Axes.
+        """
+        if not self._has_array:
+            return AxesFormatter(self._axes)
+        else:
+            return AxesFormatterArray(self._axes)
+
+    @property
+    def x_axes(self) -> Union[AxisFormatter, AxisFormatterArray]:
+        """
+        Return an AxisFormatter or AxisFormatterArray for the X-Axis or X-Axes
+        of the wrapped Axes.
+        """
+        if not self._has_array:
+            return AxesFormatter(self._axes).x_axis
+        else:
+            axes = empty_like(self._axes, dtype=AxisFormatter)
+            if axes.ndim == 1:
+                for i in range(self._axes.shape[0]):
+                    axes[i] = AxisFormatter(
+                        axis=self._axes[i].xaxis,
+                        direction='x',
+                        axes=self._axes[i]
+                    )
+            elif axes.ndim == 2:
+                for i in range(axes.shape[0]):
+                    for j in range(axes.shape[1]):
+                        axes[i, j] = AxisFormatter(
+                            axis=self._axes[i, j].xaxis,
+                            direction='x',
+                            axes=self._axes[i, j]
+                        )
+
+        return AxisFormatterArray(axes)
+
+    @property
+    def y_axes(self) -> Union[AxisFormatter, AxisFormatterArray]:
+        """
+        Return an AxisFormatter or AxisFormatterArray for the Y-Axis or Y-Axes
+        of the wrapped Axes.
+        """
+        if not self._has_array:
+            return AxesFormatter(self._axes).y_axis
+        else:
+            axes = empty_like(self._axes, dtype=AxisFormatter)
+            if axes.ndim == 1:
+                for i in range(self._axes.shape[0]):
+                    axes[i] = AxisFormatter(
+                        axis=self._axes[i].yaxis,
+                        direction='y',
+                        axes=self._axes[i]
+                    )
+            elif axes.ndim == 2:
+                for i in range(axes.shape[0]):
+                    for j in range(axes.shape[1]):
+                        axes[i, j] = AxisFormatter(
+                            axis=self._axes[i, j].yaxis,
+                            direction='y',
+                            axes=self._axes[i, j]
+                        )
+
+        return AxisFormatterArray(axes)
+
+    @property
+    def figure(self) -> Figure:
+        return self._figure
+
+    @property
+    def single(self) -> AxesFormatter:
+        """
+        Return an AxesFormatter for the wrapped Axes.
+        """
+        if not self._has_array:
+            return AxesFormatter(self._axes)
+        else:
+            raise TypeError('FigureFormatter holds an array of Axes.')
+
+    @property
+    def multi(self) -> AxesFormatterArray:
+        """
+        Return an AxesFormatterArray for the wrapped Axes.
+        """
+        if self._has_array:
+            return AxesFormatterArray(self._axes)
+        else:
+            raise TypeError('FigureFormatter holds a single Axes.')
+
+    # endregion
+
+    # region set text
+
+    def _set_text_property(
+            self,
+            text: TextSetter,
+            method: Callable[[AxesFormatter, str], AxesFormatter]
+    ) -> 'FigureFormatter':
+        """
+        Set a text property of each Axes using a string, list of strings,
+        or function that returns a string based on the row and column or the
+        flat index of the Axes.
+
+        :param text: Title or titles to set
+        :param method: Method to call to format the text.
+        """
+        if not self._has_array:
+            if not isinstance(text, str):
+                raise TypeError('text must be a str for a single Axes.')
+            else:
+                method(self.single, text)
+        else:
+            if isinstance(text, str):
+                for axf in self.multi.flat:
+                    method(axf, text)
+            elif isinstance(text, list):
+                if len(text) != self.multi.size:
+                    raise ValueError(f'There are {self.multi.size} Axes'
+                                     f' and {len(text)} strings.')
+                else:
+                    for axf, t in zip(self.multi.flat, text):
+                        method(axf, t)
+            elif callable(text):
+                try:
+                    for row in range(self.multi.shape[0]):
+                        for col in range(self.multi.shape[1]):
+                            method(self.multi[row, col], text(row, col))
+                except TypeError:
+                    for a, axf in enumerate(self.multi.flat):
+                        method(axf, text(a))
+            else:
+                raise TypeError(
+                    f'Wrong type passed to _set_text_property: {type(text)}'
+                )
+        return self
+
+    def set_title(self, text) -> 'FigureFormatter':
+        """
+        Set the title of the Figure.
+
+        :param text: The text for the title.
+        """
+        self._figure.suptitle(t=text)
+        return self
+
+    def set_axes_title_text(
+            self,
+            text: TextSetter
+    ) -> 'FigureFormatter':
+        """
+        Set the title text of each Axes using a string, list of strings,
+        or function that returns a string based on the row and column or the
+        flat index of the Axes.
+
+        :param text: Title or titles to set.
+        """
+        def set_text(
+                axes_formatter: AxesFormatter, string: str
+        ) -> AxesFormatter:
+            return axes_formatter.set_title_text(string)
+
+        self._set_text_property(text=text, method=set_text)
+        return self
+
+    def map_axes_title_text(
+            self, mapping: StringMapper
+    ) -> 'FigureFormatter':
+        """
+        Map the label text for the x-axis using a dictionary or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        if not self._has_array:
+            self.single.map_title_text(mapping=mapping)
+        else:
+            for axf in self.multi.flat:
+                axf.map_title_text(mapping=mapping)
+        return self
+
+    def set_axes_x_label_text(
+            self,
+            text: TextSetter
+    ) -> 'FigureFormatter':
+        """
+        Set the x-label text of each Axes using a string, list of strings,
+        or function that returns a string based on the row and column or the
+        flat index of the Axes.
+
+        :param text: Label or labels to set.
+        """
+        def set_text(
+                axes_formatter: AxesFormatter, string: str
+        ) -> AxesFormatter:
+            return axes_formatter.set_x_label_text(string)
+
+        self._set_text_property(text=text, method=set_text)
+        return self
+
+    def set_axes_y_label_text(
+            self, text: TextSetter
+    ) -> 'FigureFormatter':
+        """
+        Set the x-label text of each Axes using a string, list of strings,
+        or function that returns a string based on the row and column or the
+        flat index of the Axes.
+
+        :param text: Label or labels to set.
+        """
+        def set_text(
+                axes_formatter: AxesFormatter, string: str
+        ) -> AxesFormatter:
+            return axes_formatter.set_y_label_text(string)
+
+        self._set_text_property(text=text, method=set_text)
+        return self
+
+    def set_axes_text(
+            self,
+            title: Optional[TextSetter] = None,
+            x_label: Optional[TextSetter] = None,
+            y_label: Optional[TextSetter] = None
+    ) -> 'FigureFormatter':
+        """
+        Set the text for each Axes' title, x_label or y_label.
+
+        :param title: Axes titles.
+        :param x_label: Axes x-labels.
+        :param y_label: Axes y-labels.
+        """
+        if title is not None:
+            self.set_axes_title_text(title)
+        if x_label is not None:
+            self.set_axes_x_label_text(x_label)
+        if y_label is not None:
+            self.set_axes_y_label_text(y_label)
+        return self
+
+    # endregion
+
+    # region wrap text
+
+    def wrap_titles(self, max_width: int) -> 'FigureFormatter':
+        """
+        Wrap the text for each Axes title if it exceeds a given width
+        of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        if not self._has_array:
+            self.single.wrap_title(max_width=max_width)
+        else:
+            for axf in self.multi.flat:
+                axf.wrap_title(max_width=max_width)
+        return self
+
+    def wrap_x_labels(self, max_width: int) -> 'FigureFormatter':
+        """
+        Wrap the text for each X-Axis label if it exceeds a given width
+        of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.wrap_x_label(max_width=max_width)
+        else:
+            self.single.wrap_x_label(max_width=max_width)
+        return self
+
+    def wrap_y_labels(self, max_width: int) -> 'FigureFormatter':
+        """
+        Wrap the text for each Y-Axis label if it exceeds a given width
+        of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.wrap_y_label(max_width=max_width)
+        else:
+            self.single.wrap_y_label(max_width=max_width)
+        return self
+
+    def wrap_axes_labels(self, max_width: int) -> 'FigureFormatter':
+        """
+        Wrap the text for each Axis label if it exceeds a given width
+        of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        self.wrap_x_labels(max_width=max_width)
+        self.wrap_y_labels(max_width=max_width)
+        return self
+
+    def wrap_x_tick_labels(self, max_width: int) -> 'FigureFormatter':
+        """
+        Wrap the text for each tick label on each x-axis if it exceeds a
+        given width of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.x_ticks.wrap_label_text(max_width=max_width)
+        else:
+            self.single.x_ticks.wrap_label_text(max_width=max_width)
+        return self
+
+    def wrap_y_tick_labels(self, max_width: int) -> 'FigureFormatter':
+        """
+        Wrap the text for each tick label on each y-axis if it exceeds a
+        given width of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.y_ticks.wrap_label_text(max_width=max_width)
+        else:
+            self.single.y_ticks.wrap_label_text(max_width=max_width)
+        return self
+
+    def wrap_tick_labels(self, max_width: int) -> 'FigureFormatter':
+        """
+        Wrap the text for each tick label on each x- and y-axis if it exceeds a
+        given width of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        self.wrap_x_tick_labels(max_width=max_width)
+        self.wrap_y_tick_labels(max_width=max_width)
+        return self
+
+    # endregion
+
+    # region map labels
+
+    def map_x_axis_labels(
+            self, mapping: StringMapper
+    ) -> 'FigureFormatter':
+        """
+        Map the label text for each x-axis in the Figure using a dictionary
+        or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.map_x_axis_label(mapping=mapping)
+        else:
+            self.single.map_x_axis_label(mapping=mapping)
+        return self
+
+    def map_y_axis_labels(
+            self, mapping: StringMapper
+    ) -> 'FigureFormatter':
+        """
+        Map the label text for each y-axis in the Figure using a dictionary
+        or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.map_y_axis_label(mapping=mapping)
+        else:
+            self.single.map_y_axis_label(mapping=mapping)
+        return self
+
+    def map_axis_labels(
+            self, mapping: StringMapper
+    ) -> 'FigureFormatter':
+        """
+        Map the label text for each axis in the Figure using a dictionary
+        or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        self.map_x_axis_labels(mapping=mapping)
+        self.map_y_axis_labels(mapping=mapping)
+        return self
+
+    def map_x_tick_labels(
+            self, mapping: StringMapper
+    ) -> 'FigureFormatter':
+        """
+        Map the tick label text for each x-axis using a dictionary or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.x_ticks.map_label_text(mapping=mapping)
+        else:
+            self.single.x_ticks.map_label_text(mapping=mapping)
+        return self
+
+    def map_y_tick_labels(
+            self, mapping: StringMapper
+    ) -> 'FigureFormatter':
+        """
+        Map the tick label text for each y-axis using a dictionary or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.y_ticks.map_label_text(mapping=mapping)
+        else:
+            self.single.y_ticks.map_label_text(mapping=mapping)
+        return self
+
+    def map_tick_labels(
+            self, mapping: StringMapper
+    ) -> 'FigureFormatter':
+        """
+        Map the tick label text for each axis using a dictionary or function.
+
+        :param mapping: Dictionary or a function mapping old text to new text.
+        """
+        self.map_x_tick_labels(mapping=mapping)
+        self.map_y_tick_labels(mapping=mapping)
+        return self
+
+    # endregion
+
+    # region remove
+
+    def remove_titles(self) -> 'FigureFormatter':
+        """
+        Remove the title from each Axes.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.remove_title()
+        else:
+            self.single.remove_title()
+        return self
+
+    def remove_legends(self) -> 'FigureFormatter':
+        """
+        Remove the legend from each Axes.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.remove_legend()
+        else:
+            self.single.remove_legend()
+        return self
+
+    def remove_x_ticks(self) -> 'FigureFormatter':
+        """
+        Remove x-ticks from each Axes.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.remove_x_ticks()
+        else:
+            self.single.remove_x_ticks()
+        return self
+
+    def remove_y_ticks(self) -> 'FigureFormatter':
+        """
+        Remove y-ticks from each Axes.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.remove_y_ticks()
+        else:
+            self.single.remove_y_ticks()
+        return self
+
+    def remove_axes_ticks(self) -> 'FigureFormatter':
+        """
+        Remove ticks from each Axes.
+        """
+        self.remove_x_ticks()
+        self.remove_y_ticks()
+        return self
+
+    def remove_x_labels(self) -> 'FigureFormatter':
+        """
+        Remove the x-axis label from each Axes in the Figure.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.remove_x_label()
+        else:
+            self.single.remove_x_label()
+        return self
+
+    def remove_y_labels(self) -> 'FigureFormatter':
+        """
+        Remove the y-axis label from each Axes in the Figure.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.remove_y_label()
+        else:
+            self.single.remove_y_label()
+        return self
+
+    def remove_axes_labels(self) -> 'FigureFormatter':
+        """
+        Remove the x-axis label for each Axes in the Figure.
+        """
+        self.remove_x_labels()
+        self.remove_y_labels()
+        return self
+
+    # endregion
+
+    # region rotation
+
+    def rotate_x_labels(self,
+                        rotation: int,
+                        how: ROTATION_MODE = 'absolute') -> 'FigureFormatter':
+        """
+        Set the rotation of each x-axis label.
+
+        :param rotation: The rotation value to set in degrees.
+        :param how: 'absolute' or 'relative'
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.rotate_x_label(rotation=rotation, how=how)
+        else:
+            self.single.rotate_x_label(rotation=rotation, how=how)
+        return self
+
+    def rotate_y_labels(self,
+                        rotation: int,
+                        how: ROTATION_MODE = 'absolute') -> 'FigureFormatter':
+        """
+        Set the rotation of each x-axis label.
+
+        :param rotation: The rotation value to set in degrees.
+        :param how: 'absolute' or 'relative'
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.rotate_y_label(rotation=rotation, how=how)
+        else:
+            self.single.rotate_y_label(rotation=rotation, how=how)
+        return self
+
+    def rotate_x_tick_labels(self,
+                             rotation: int) -> 'FigureFormatter':
+        """
+        Set the rotation of each x-axis' tick-labels.
+
+        :param rotation: The rotation value to set in degrees.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.x_ticks.set_label_rotation(rotation=rotation)
+        else:
+            self.single.x_ticks.set_label_rotation(rotation=rotation)
+        return self
+
+    def rotate_y_tick_labels(self,
+                             rotation: int) -> 'FigureFormatter':
+        """
+        Set the rotation of each y-axis' tick-labels.
+
+        :param rotation: The rotation value to set in degrees.
+        """
+        if self._has_array:
+            for axf in self.multi.flat:
+                axf.y_ticks.set_label_rotation(rotation=rotation)
+        else:
+            self.single.y_ticks.set_label_rotation(rotation=rotation)
+        return self
+
+    # endregion
+
+    # region margins
+
+    def subplots_adjust(
+            self,
+            left: Optional[float] = None, right: Optional[float] = None,
+            top: Optional[float] = None, bottom: Optional[float] = None,
+            w_space: Optional[float] = None, h_space: Optional[float] = None
+    ) -> 'FigureFormatter':
+        """
+        Adjust the padding of the Figure.
+
+        :param left: The position of the left edge of the subplots,
+                     as a fraction of the figure width. Use 0 for no margin.
+        :param right: The position of the right edge of the subplots,
+                      as a fraction of the figure width. Use 1 for no margin.
+        :param top: The position of the top edge of the subplots,
+                    as a fraction of the figure height. Use 1 for no margin.
+        :param bottom: The position of the bottom edge of the subplots,
+                       as a fraction of the figure height. Use 0 for no margin.
+        :param w_space: The width of the padding between subplots,
+                        as a fraction of the average axes width.
+        :param h_space: The height of the padding between subplots,
+                        as a fraction of the average axes height.
+        """
+        self.figure.subplots_adjust(
+            left=left, right=right,
+            bottom=bottom, top=top,
+            wspace=w_space, hspace=h_space
+        )
+        return self
+
+    def set_left_margin(self, margin_size: float) -> 'FigureFormatter':
+        """
+        Set the margin size at the left of the plot.
+
+        :param margin_size: Value between 0 and 1. 0 for no margin
+        """
+        self.subplots_adjust(left=margin_size)
+        return self
+
+    def set_right_margin(self, margin_size: float) -> 'FigureFormatter':
+        """
+        Set the margin size at the right of the plot.
+
+        :param margin_size: Value between 0 and 1. 0 for no margin
+        """
+        self.subplots_adjust(right=1 - margin_size)
+        return self
+
+    def set_top_margin(self, margin_size: float) -> 'FigureFormatter':
+        """
+        Set the margin size at the top of the plot.
+
+        :param margin_size: Value between 0 and 1. 0 for no margin
+        """
+        self.subplots_adjust(top=1 - margin_size)
+        return self
+
+    def set_bottom_margin(self, margin_size: float) -> 'FigureFormatter':
+        """
+        Set the margin size at the bottom of the plot.
+
+        :param margin_size: Value between 0 and 1. 0 for no margin
+        """
+        self.subplots_adjust(bottom=margin_size)
+        return self
+
+    def set_horizontal_margin(self, margin_size: float) -> 'FigureFormatter':
+        """
+        Set the margin size at the left and right of the plot.
+
+        :param margin_size: Value between 0 and 1. 0 for no margin
+        """
+        self.subplots_adjust(left=margin_size, right=1 - margin_size)
+        return self
+
+    def set_vertical_margin(self, margin_size: float) -> 'FigureFormatter':
+        """
+        Set the margin size at the top and bottom of the plot.
+
+        :param margin_size: Value between 0 and 1. 0 for no margin
+        """
+        self.subplots_adjust(bottom=margin_size, top=1 - margin_size)
+        return self
+
+    def set_margin(self, margin_size: float) -> 'FigureFormatter':
+        """
+        Set the margin size at the top of the plot.
+
+        :param margin_size: Value between 0 and 1. 0 for no margin
+        """
+        self.subplots_adjust(bottom=margin_size, top=1 - margin_size,
+                             left=margin_size, right=1 - margin_size)
+        return self
+
+    def set_horizontal_spacing(self, spacing: float) -> 'FigureFormatter':
+        """
+        Set the horizontal spacing between each subplot.
+
+        :param spacing: The width of the padding between subplots,
+                        as a fraction of the average axes width.
+        """
+        self.subplots_adjust(w_space=spacing)
+        return self
+
+    def set_vertical_spacing(self, spacing: float) -> 'FigureFormatter':
+        """
+        Set the vertical spacing between each subplot.
+
+        :param spacing: The height of the padding between subplots,
+                        as a fraction of the average axes height.
+        """
+        self.subplots_adjust(h_space=spacing)
+        return self
+
+    # endregion
+
+    def grids(
+            self, value: bool = True,
+            which: WHICH_TICKS = 'major',
+            axis: WHICH_AXIS = 'both',
+            color: Optional[Color] = None,
+            line_width: Optional[float] = None,
+            line_style: Optional[Union[str, LINE_STYLE]] = None
+    ) -> 'FigureFormatter':
+        """
+        Turn the grid on or off.
+
+        :param value: True or False. Defaults to True.
+        :param which: 'major', 'minor' or 'both'
+        :param axis: 'x', 'y' or 'both.
+        :param color: Color of the lines.
+        :param line_width: Line width.
+        :param line_style: Line Style. One of {'-', '--', '-.', ':', '',
+                           (offset, on-off-seq), ...}
+        """
+        for axes in self.axes.flat:
+            axes.grid(value=value, which=which, axis=axis,
+                      color=color, line_width=line_width,
+                      line_style=line_style)
+        return self
+
+    def set_axes_below(self, value: bool = True) -> 'FigureFormatter':
+        """
+        Set whether axis ticks and gridlines are above or below most artists.
+
+        :param value: True or False
+        """
+        for axes in self.axes.flat:
+            axes.set_axis_below(value=value)
+        return self
+
+    def tight_layout(self) -> 'FigureFormatter':
+        """
+        Call the tight_layout method on the wrapped Figure.
+        """
+        self.figure.tight_layout()
+        return self
+
+    # region limits
+
+    def set_x_lims(self, left: Optional[float] = None,
+                   right: Optional[float] = None) -> 'FigureFormatter':
+        """
+        Set the limits of the x-axes.
+
+        :param left: Lower limit.
+        :param right: Upper limit.
+        """
+        for axf in self.multi.flat:
+            axf.set_x_lim(left=left, right=right)
+        return self
+
+    def set_y_lims(self, bottom: Optional[float] = None,
+                   top: Optional[float] = None) -> 'FigureFormatter':
+        """
+        Set the limits of the y-axes.
+
+        :param bottom: Lower limit.
+        :param top: Upper limit.
+        """
+        for axf in self.multi.flat:
+            axf.set_y_lim(bottom=bottom, top=top)
+        return self
+
+    def set_x_mins(self, left: float = None) -> 'FigureFormatter':
+        """
+        Set the x-axes lower view limit.
+        """
+        self.set_x_lims(left, None)
+        return self
+
+    def set_x_maxes(self, right: float = None) -> 'FigureFormatter':
+        """
+        Set the x-axes upper view limit.
+        """
+        self.set_x_lims(None, right)
+        return self
+
+    def set_y_mins(self, bottom: float = None) -> 'FigureFormatter':
+        """
+        Set the y-axes lower view limit.
+        """
+        self.set_y_lims(bottom, None)
+        return self
+
+    def set_y_maxes(self, top: float = None) -> 'FigureFormatter':
+        """
+        Set the y-axes upper view limit.
+        """
+        self.set_y_lims(None, top)
+        return self
+
+    # endregion
+
+    def save(
+            self,
+            file_path: Union[str, Path],
+            file_type: Optional[str] = None
+    ) -> 'FigureFormatter':
+        """
+        Save the plot to disk.
+
+        :param file_path: The file path to save the plot object to.
+        :param file_type: The type of file to save.
+                          Defaults to png if can't be auto-detected from name.
+        """
+        save_plot(plot_object=self._figure,
+                  file_path=file_path, file_type=file_type)
+        return self
+
+    def show(self) -> 'FigureFormatter':
+        """
+        Show the figure.
+        """
+        plt.show()
+        return self
+
+    def __getitem__(self, *args, **kwargs) -> AxesFormatter:
+
+        return self.multi.__getitem__(*args, **kwargs)
```

### Comparing `mpl_format-0.317/mpl_format/legend/legend_formatter.py` & `mpl_format-0.318/mpl_format/legend/legend_formatter.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,414 +1,414 @@
-from typing import Union, List, Optional
-
-from matplotlib.collections import PathCollection
-from matplotlib.font_manager import FontProperties
-from matplotlib.legend import Legend
-
-from mpl_format.compound_types import ArrayLike
-from mpl_format.compound_types import Color, FontSize, LegendLocation, \
-    StringMapper
-from mpl_format.text.text_formatter import TextFormatter
-from mpl_format.text.text_utils import map_text
-
-
-class LegendFormatter(object):
-
-    def __init__(self, legend: Legend):
-        """
-        Create a new legend formatter.
-        """
-        self._legend: Legend = legend
-
-    @property
-    def legend(self) -> Legend:
-        return self._legend
-
-    @property
-    def title(self) -> TextFormatter:
-        """
-        Return a TextFormatter around the legend's title.
-        """
-        return TextFormatter(self._legend.get_title())
-
-    # region set location
-
-    def set_location(self, location: Union[int, str]) -> 'LegendFormatter':
-        """
-        Set the legend location.
-        """
-        self.recreate_legend(location=location)
-        return self
-
-    def set_location_best(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'best'.
-        """
-        self.set_location('best')
-        return self
-
-    def set_location_upper_left(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'upper left'.
-        """
-        self.set_location('upper left')
-        return self
-
-    def set_location_upper_center(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'upper center'.
-        """
-        self.set_location('upper center')
-        return self
-
-    def set_location_upper_right(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'upper right'.
-        """
-        self.set_location('upper right')
-        return self
-
-    def set_location_center_left(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'center left'.
-        """
-        self.set_location('center left')
-        return self
-
-    def set_location_center(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'center'.
-        """
-        self.set_location('center')
-        return self
-
-    def set_location_center_right(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'center right'.
-        """
-        self.set_location('center right')
-        return self
-
-    def set_location_lower_left(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'lower left'.
-        """
-        self.set_location('lower left')
-        return self
-
-    def set_location_lower_center(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'lower center'.
-        """
-        self.set_location('lower center')
-        return self
-
-    def set_location_lower_right(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'lower right'.
-        """
-        self.set_location('lower right')
-        return self
-
-    def set_location_left(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'center left'.
-        """
-        self.set_location('center left')
-        return self
-
-    def set_location_right(self) -> 'LegendFormatter':
-        """
-        Set the legend location to 'center right'.
-        """
-        self.set_location('center right')
-        return self
-
-    # endregion
-
-    def recreate_legend(
-            self, handles: Optional[List[PathCollection]] = None,
-            labels: Optional[List[str]] = None,
-            location: Optional[LegendLocation] = None,
-            n_cols: Optional[int] = None,
-            font_size: Optional[str] = None,
-            font_properties: Optional[Union[FontProperties, dict]] = None,
-            line_points: Optional[int] = None,
-            scatter_points: Optional[int] = None,
-            scatter_y_offsets: Optional[ArrayLike] = None,
-            marker_scale: Optional[float] = None,
-            frame_on: Optional[bool] = None,
-            shadow: Optional[bool] = None,
-            frame_alpha: Optional[float] = None,
-            face_color: Optional[Color] = None,
-            edge_color: Optional[Color] = None,
-            mode: Optional[str] = None,
-            title: Optional[str] = None,
-            title_font_size: Optional[FontSize] = None,
-            label_spacing: Optional[float] = None,
-            handle_length: Optional[float] = None,
-            handle_text_pad: Optional[float] = None,
-            border_axes_pad: Optional[float] = None,
-            column_spacing: Optional[float] = None) -> 'LegendFormatter':
-        """
-
-        :param handles: A list of Artists (lines, patches) to be added to the
-                        legend.
-        :param labels: A list of labels to show next to the artists. The length
-                       of handles and labels should be the same. If they are
-                       not, they are truncated to the smaller of both lengths.
-        :param location: The location of the legend.
-        :param n_cols: The number of columns that the legend has. Default is 1.
-        :param font_size: The font size of the legend. If the value is numeric
-                          the size will be the absolute font size in points.
-                          String values are relative to the current default font
-                          size. This argument is only used if font_properties is
-                          not specified.
-        :param font_properties: The font properties of the legend. If None
-                                (default), the current matplotlib.rcParams
-                                will be used.
-        :param line_points: The number of marker points in the legend when
-                            creating a legend entry for a Line2D (line).
-                            Default is None, which means using
-                            rcParams["legend.numpoints"] (default: 1).
-        :param scatter_points: The number of marker points in the legend when
-                               creating a legend entry for a PathCollection
-                               (scatter plot). Default is None, which means
-                               using rcParams["legend.scatterpoints"]
-                               (default: 1).
-        :param scatter_y_offsets: The vertical offset (relative to the font
-                                  size) for the markers created for a scatter
-                                  plot legend entry. 0.0 is at the base the
-                                  legend text, and 1.0 is at the top. To draw
-                                  all markers at the same height, set to [0.5].
-                                  Default is [0.375, 0.5, 0.3125].
-        :param marker_scale: The relative size of legend markers compared with
-                             the originally drawn ones. Default is None, which
-                             means using rcParams["legend.markerscale"]
-                             (default: 1.0).
-        :param frame_on: Whether the legend should be drawn on a patch (frame).
-                         Default is None, which means using
-                         rcParams["legend.frameon"] (default: True).
-        :param shadow: Whether to draw a shadow behind the legend. Default is
-                       None, which means using rcParams["legend.shadow"]
-                       (default: False).
-        :param frame_alpha: The alpha transparency of the legend's background.
-                            Default is None, which means using
-                            rcParams["legend.framealpha"] (default: 0.8). If
-                            shadow is activated and framealpha is None, the
-                            default value is ignored.
-        :param face_color: The legend's background color. Default is None,
-                           which means using rcParams["legend.facecolor"]
-                           (default: 'inherit'). If "inherit", use
-                           rcParams["axes.facecolor"] (default: 'white').
-        :param edge_color: The legend's background patch edge color. Default is
-                           None, which means using rcParams["legend.edgecolor"]
-                           (default: '0.8'). If "inherit", use take
-                           rcParams["axes.edgecolor"] (default: 'black').
-        :param mode: If mode is set to "expand" the legend will be horizontally
-                     expanded to fill the axes area (or bbox_to_anchor if
-                     defines the legend's size).
-        :param title: The legend's title. Default is no title (None).
-        :param title_font_size: The fontsize of the legend's title. Default is
-                                the default fontsize.
-        :param label_spacing: The fractional whitespace inside the legend
-                              border, in font-size units. Default is None,
-                              which means using rcParams["legend.borderpad"]
-                              (default: 0.4).
-        :param handle_length: The length of the legend handles, in font-size
-                              units. Default is None, which means using
-                              rcParams["legend.handlelength"] (default: 2.0).
-        :param handle_text_pad: The pad between the legend handle and text, in
-                                font-size units. Default is None, which means
-                                using rcParams["legend.handletextpad"]
-                                (default: 0.8).
-        :param border_axes_pad: The pad between the axes and legend border, in
-                                font-size units. Default is None, which means
-                                using rcParams["legend.borderaxespad"]
-                                (default: 0.5).
-        :param column_spacing: The spacing between columns, in font-size units.
-                               Default is None, which means using
-                               rcParams["legend.columnspacing"] (default: 2.0).
-        """
-        kwargs = {}
-        for kwarg, mpl_arg in zip(
-                [handles, labels, n_cols, font_properties, font_size,
-                 line_points, scatter_points, scatter_y_offsets,
-                 marker_scale, frame_on, shadow, frame_alpha, face_color,
-                 edge_color, mode, title,
-                 title_font_size, label_spacing, handle_length, handle_text_pad,
-                 border_axes_pad, column_spacing,
-                 location],
-                ['handles', 'labels', 'ncol', 'prop', 'fontsize', 'numpoints',
-                 'scatterpoints', 'scatteryoffsets',
-                 'markerscale', 'frameon', 'shadow', 'framealpha', 'facecolor',
-                 'edgecolor', 'mode', 'title',
-                 'title_fontsize', 'labelspacing', 'handlelength',
-                 'handletextpad', 'borderaxespad', 'columnspacing',
-                 'loc']
-        ):
-            if kwarg is not None:
-                kwargs[mpl_arg] = kwarg
-
-        if 'handles' not in kwargs.keys():
-            kwargs['handles'] = self._legend.legendHandles
-        if 'labels' not in kwargs.keys():
-            kwargs['labels'] = [text.get_text() for text in self._legend.texts]
-
-        self._legend = self._legend.axes.legend(**kwargs)
-        return self
-
-    def remove_entries(self, indices: List[int]) -> 'LegendFormatter':
-        """
-        Remove legend handles and labels from the legend at the given indices.
-        N.B. this creates a new legend. May need to set the following properties
-        manually afterwards as they cannot be automatically determined from the
-        old legend:
-        ['loc', 'markerfirst', 'fancybox', 'bbox_to_anchor' 'bbox_transform',
-        'handler_map']
-
-        :param indices: The indices of the legend entries to remove.
-        """
-        handles = self._legend.legendHandles
-        labels = [text.get_text() for text in self._legend.texts]
-        for entry_index in sorted(indices, reverse=True):
-            handles.pop(entry_index)
-            labels.pop(entry_index)
-        legend = self._legend
-        self.recreate_legend(
-            handles=handles, labels=labels,
-            n_cols=legend._ncol,
-            font_properties=legend.prop,
-            line_points=legend.numpoints,
-            scatter_points=legend.scatterpoints,
-            scatter_y_offsets=legend._scatteryoffsets,
-            marker_scale=legend.markerscale,
-            frame_on=legend.get_frame_on(),
-            shadow=legend.shadow,
-            frame_alpha=legend.get_frame().get_alpha(),
-            face_color=legend.get_frame().get_facecolor(),
-            edge_color=legend.get_frame().get_edgecolor(),
-            mode=legend._mode,
-            title=legend.get_title().get_text(),
-            title_font_size=legend.get_title().get_fontsize(),
-            label_spacing=legend.labelspacing,
-            handle_length=legend.handlelength,
-            handle_text_pad=legend.handletextpad,
-            border_axes_pad=legend.borderaxespad,
-            column_spacing=legend.columnspacing
-        )
-        return self
-
-    def map_labels(
-            self, mapping: StringMapper
-    ) -> 'LegendFormatter':
-        """
-        Replace label text using a dictionary or function.
-
-        :param mapping: Mappings to replace text.
-        """
-        handles, labels = self._legend.axes.get_legend_handles_labels()
-        labels = [map_text(text=label, mapping=mapping) for label in labels]
-        self.recreate_legend(labels=labels)
-        return self
-
-    def set_alpha(self, alpha: float) -> 'LegendFormatter':
-        """
-        Set the opacity of the legend frame.
-        """
-        self._legend.set_alpha(alpha=alpha)
-        return self
-
-    def set_face_color(self, color: Color) -> 'LegendFormatter':
-        """
-        Set the face color of the legend frame.
-        """
-        self._legend.get_frame().set_facecolor(color)
-        return self
-
-    def set_edge_color(self, color: Color) -> 'LegendFormatter':
-        """
-        Set the edge color of the legend frame.
-        """
-        self._legend.get_frame().set_edgecolor(color)
-        return self
-
-    def set_frame_on(self, on: bool = True) -> 'LegendFormatter':
-        """
-        Turn the frame on or off.
-        """
-        self._legend.set_frame_on(b=on)
-        return self
-
-    def set_z_order(self, level: int) -> 'LegendFormatter':
-        """
-        Set the z-order of the legend.
-        """
-        self._legend.set_zorder(level=level)
-        return self
-
-    def set_title_text(self, text: str) -> 'LegendFormatter':
-        """
-        Set the text of the legend title.
-        """
-        self.title.set_text(text)
-        return self
-
-    def set_title_font_family(self, font_name: str) -> 'LegendFormatter':
-        """
-        Set the font family of the legend title.
-        """
-        self.title.set_font_family(font_name)
-        return self
-
-    def set_title_font_size(self, font_size: FontSize) -> 'LegendFormatter':
-        """
-        Set the font size of the legend title.
-        """
-        self.title.set_size(font_size=font_size)
-        return self
-
-    def set_n_cols(self, n_cols: int) -> 'LegendFormatter':
-        """
-        Set the number of columns the legend has.
-
-        N.B. this creates a new legend. May need to set the following properties
-        manually afterwards as they cannot be automatically determined from the
-        old legend:
-        ['loc', 'markerfirst', 'fancybox', 'bbox_to_anchor' 'bbox_transform',
-        'handler_map']
-        """
-        self.recreate_legend(n_cols=n_cols)
-        return self
-
-    def set_line_points(self, num_points: int) -> 'LegendFormatter':
-        """
-        Set the number of points for a line legend entry.
-
-        N.B. this creates a new legend. May need to set the following properties
-        manually afterwards as they cannot be automatically determined from the
-        old legend:
-        ['loc', 'markerfirst', 'fancybox', 'bbox_to_anchor' 'bbox_transform',
-        'handler_map']
-        """
-        self.recreate_legend(line_points=num_points)
-        return self
-
-    def set_scatter_points(self, num_points: int) -> 'LegendFormatter':
-        """
-        Set the number of points for a scatter legend entry.
-
-        N.B. this creates a new legend. May need to set the following properties
-        manually afterwards as they cannot be automatically determined from the
-        old legend:
-        ['loc', 'markerfirst', 'fancybox', 'bbox_to_anchor' 'bbox_transform',
-        'handler_map']
-        """
-        self.recreate_legend(scatter_points=num_points)
-        return self
-
-    def set_shadow(self, on: bool = True) -> 'LegendFormatter':
-        """
-        Turn the shadow on or off for the legend frame.
-        """
-        self._legend.shadow = on
-        return self
+from typing import Union, List, Optional
+
+from matplotlib.collections import PathCollection
+from matplotlib.font_manager import FontProperties
+from matplotlib.legend import Legend
+
+from mpl_format.compound_types import ArrayLike
+from mpl_format.compound_types import Color, FontSize, LegendLocation, \
+    StringMapper
+from mpl_format.text.text_formatter import TextFormatter
+from mpl_format.text.text_utils import map_text
+
+
+class LegendFormatter(object):
+
+    def __init__(self, legend: Legend):
+        """
+        Create a new legend formatter.
+        """
+        self._legend: Legend = legend
+
+    @property
+    def legend(self) -> Legend:
+        return self._legend
+
+    @property
+    def title(self) -> TextFormatter:
+        """
+        Return a TextFormatter around the legend's title.
+        """
+        return TextFormatter(self._legend.get_title())
+
+    # region set location
+
+    def set_location(self, location: Union[int, str]) -> 'LegendFormatter':
+        """
+        Set the legend location.
+        """
+        self.recreate_legend(location=location)
+        return self
+
+    def set_location_best(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'best'.
+        """
+        self.set_location('best')
+        return self
+
+    def set_location_upper_left(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'upper left'.
+        """
+        self.set_location('upper left')
+        return self
+
+    def set_location_upper_center(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'upper center'.
+        """
+        self.set_location('upper center')
+        return self
+
+    def set_location_upper_right(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'upper right'.
+        """
+        self.set_location('upper right')
+        return self
+
+    def set_location_center_left(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'center left'.
+        """
+        self.set_location('center left')
+        return self
+
+    def set_location_center(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'center'.
+        """
+        self.set_location('center')
+        return self
+
+    def set_location_center_right(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'center right'.
+        """
+        self.set_location('center right')
+        return self
+
+    def set_location_lower_left(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'lower left'.
+        """
+        self.set_location('lower left')
+        return self
+
+    def set_location_lower_center(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'lower center'.
+        """
+        self.set_location('lower center')
+        return self
+
+    def set_location_lower_right(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'lower right'.
+        """
+        self.set_location('lower right')
+        return self
+
+    def set_location_left(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'center left'.
+        """
+        self.set_location('center left')
+        return self
+
+    def set_location_right(self) -> 'LegendFormatter':
+        """
+        Set the legend location to 'center right'.
+        """
+        self.set_location('center right')
+        return self
+
+    # endregion
+
+    def recreate_legend(
+            self, handles: Optional[List[PathCollection]] = None,
+            labels: Optional[List[str]] = None,
+            location: Optional[LegendLocation] = None,
+            n_cols: Optional[int] = None,
+            font_size: Optional[str] = None,
+            font_properties: Optional[Union[FontProperties, dict]] = None,
+            line_points: Optional[int] = None,
+            scatter_points: Optional[int] = None,
+            scatter_y_offsets: Optional[ArrayLike] = None,
+            marker_scale: Optional[float] = None,
+            frame_on: Optional[bool] = None,
+            shadow: Optional[bool] = None,
+            frame_alpha: Optional[float] = None,
+            face_color: Optional[Color] = None,
+            edge_color: Optional[Color] = None,
+            mode: Optional[str] = None,
+            title: Optional[str] = None,
+            title_font_size: Optional[FontSize] = None,
+            label_spacing: Optional[float] = None,
+            handle_length: Optional[float] = None,
+            handle_text_pad: Optional[float] = None,
+            border_axes_pad: Optional[float] = None,
+            column_spacing: Optional[float] = None) -> 'LegendFormatter':
+        """
+
+        :param handles: A list of Artists (lines, patches) to be added to the
+                        legend.
+        :param labels: A list of labels to show next to the artists. The length
+                       of handles and labels should be the same. If they are
+                       not, they are truncated to the smaller of both lengths.
+        :param location: The location of the legend.
+        :param n_cols: The number of columns that the legend has. Default is 1.
+        :param font_size: The font size of the legend. If the value is numeric
+                          the size will be the absolute font size in points.
+                          String values are relative to the current default font
+                          size. This argument is only used if font_properties is
+                          not specified.
+        :param font_properties: The font properties of the legend. If None
+                                (default), the current matplotlib.rcParams
+                                will be used.
+        :param line_points: The number of marker points in the legend when
+                            creating a legend entry for a Line2D (line).
+                            Default is None, which means using
+                            rcParams["legend.numpoints"] (default: 1).
+        :param scatter_points: The number of marker points in the legend when
+                               creating a legend entry for a PathCollection
+                               (scatter plot). Default is None, which means
+                               using rcParams["legend.scatterpoints"]
+                               (default: 1).
+        :param scatter_y_offsets: The vertical offset (relative to the font
+                                  size) for the markers created for a scatter
+                                  plot legend entry. 0.0 is at the base the
+                                  legend text, and 1.0 is at the top. To draw
+                                  all markers at the same height, set to [0.5].
+                                  Default is [0.375, 0.5, 0.3125].
+        :param marker_scale: The relative size of legend markers compared with
+                             the originally drawn ones. Default is None, which
+                             means using rcParams["legend.markerscale"]
+                             (default: 1.0).
+        :param frame_on: Whether the legend should be drawn on a patch (frame).
+                         Default is None, which means using
+                         rcParams["legend.frameon"] (default: True).
+        :param shadow: Whether to draw a shadow behind the legend. Default is
+                       None, which means using rcParams["legend.shadow"]
+                       (default: False).
+        :param frame_alpha: The alpha transparency of the legend's background.
+                            Default is None, which means using
+                            rcParams["legend.framealpha"] (default: 0.8). If
+                            shadow is activated and framealpha is None, the
+                            default value is ignored.
+        :param face_color: The legend's background color. Default is None,
+                           which means using rcParams["legend.facecolor"]
+                           (default: 'inherit'). If "inherit", use
+                           rcParams["axes.facecolor"] (default: 'white').
+        :param edge_color: The legend's background patch edge color. Default is
+                           None, which means using rcParams["legend.edgecolor"]
+                           (default: '0.8'). If "inherit", use take
+                           rcParams["axes.edgecolor"] (default: 'black').
+        :param mode: If mode is set to "expand" the legend will be horizontally
+                     expanded to fill the axes area (or bbox_to_anchor if
+                     defines the legend's size).
+        :param title: The legend's title. Default is no title (None).
+        :param title_font_size: The fontsize of the legend's title. Default is
+                                the default fontsize.
+        :param label_spacing: The fractional whitespace inside the legend
+                              border, in font-size units. Default is None,
+                              which means using rcParams["legend.borderpad"]
+                              (default: 0.4).
+        :param handle_length: The length of the legend handles, in font-size
+                              units. Default is None, which means using
+                              rcParams["legend.handlelength"] (default: 2.0).
+        :param handle_text_pad: The pad between the legend handle and text, in
+                                font-size units. Default is None, which means
+                                using rcParams["legend.handletextpad"]
+                                (default: 0.8).
+        :param border_axes_pad: The pad between the axes and legend border, in
+                                font-size units. Default is None, which means
+                                using rcParams["legend.borderaxespad"]
+                                (default: 0.5).
+        :param column_spacing: The spacing between columns, in font-size units.
+                               Default is None, which means using
+                               rcParams["legend.columnspacing"] (default: 2.0).
+        """
+        kwargs = {}
+        for kwarg, mpl_arg in zip(
+                [handles, labels, n_cols, font_properties, font_size,
+                 line_points, scatter_points, scatter_y_offsets,
+                 marker_scale, frame_on, shadow, frame_alpha, face_color,
+                 edge_color, mode, title,
+                 title_font_size, label_spacing, handle_length, handle_text_pad,
+                 border_axes_pad, column_spacing,
+                 location],
+                ['handles', 'labels', 'ncol', 'prop', 'fontsize', 'numpoints',
+                 'scatterpoints', 'scatteryoffsets',
+                 'markerscale', 'frameon', 'shadow', 'framealpha', 'facecolor',
+                 'edgecolor', 'mode', 'title',
+                 'title_fontsize', 'labelspacing', 'handlelength',
+                 'handletextpad', 'borderaxespad', 'columnspacing',
+                 'loc']
+        ):
+            if kwarg is not None:
+                kwargs[mpl_arg] = kwarg
+
+        if 'handles' not in kwargs.keys():
+            kwargs['handles'] = self._legend.legendHandles
+        if 'labels' not in kwargs.keys():
+            kwargs['labels'] = [text.get_text() for text in self._legend.texts]
+
+        self._legend = self._legend.axes.legend(**kwargs)
+        return self
+
+    def remove_entries(self, indices: List[int]) -> 'LegendFormatter':
+        """
+        Remove legend handles and labels from the legend at the given indices.
+        N.B. this creates a new legend. May need to set the following properties
+        manually afterwards as they cannot be automatically determined from the
+        old legend:
+        ['loc', 'markerfirst', 'fancybox', 'bbox_to_anchor' 'bbox_transform',
+        'handler_map']
+
+        :param indices: The indices of the legend entries to remove.
+        """
+        handles = self._legend.legendHandles
+        labels = [text.get_text() for text in self._legend.texts]
+        for entry_index in sorted(indices, reverse=True):
+            handles.pop(entry_index)
+            labels.pop(entry_index)
+        legend = self._legend
+        self.recreate_legend(
+            handles=handles, labels=labels,
+            n_cols=legend._ncol,
+            font_properties=legend.prop,
+            line_points=legend.numpoints,
+            scatter_points=legend.scatterpoints,
+            scatter_y_offsets=legend._scatteryoffsets,
+            marker_scale=legend.markerscale,
+            frame_on=legend.get_frame_on(),
+            shadow=legend.shadow,
+            frame_alpha=legend.get_frame().get_alpha(),
+            face_color=legend.get_frame().get_facecolor(),
+            edge_color=legend.get_frame().get_edgecolor(),
+            mode=legend._mode,
+            title=legend.get_title().get_text(),
+            title_font_size=legend.get_title().get_fontsize(),
+            label_spacing=legend.labelspacing,
+            handle_length=legend.handlelength,
+            handle_text_pad=legend.handletextpad,
+            border_axes_pad=legend.borderaxespad,
+            column_spacing=legend.columnspacing
+        )
+        return self
+
+    def map_labels(
+            self, mapping: StringMapper
+    ) -> 'LegendFormatter':
+        """
+        Replace label text using a dictionary or function.
+
+        :param mapping: Mappings to replace text.
+        """
+        handles, labels = self._legend.axes.get_legend_handles_labels()
+        labels = [map_text(text=label, mapping=mapping) for label in labels]
+        self.recreate_legend(labels=labels)
+        return self
+
+    def set_alpha(self, alpha: float) -> 'LegendFormatter':
+        """
+        Set the opacity of the legend frame.
+        """
+        self._legend.set_alpha(alpha=alpha)
+        return self
+
+    def set_face_color(self, color: Color) -> 'LegendFormatter':
+        """
+        Set the face color of the legend frame.
+        """
+        self._legend.get_frame().set_facecolor(color)
+        return self
+
+    def set_edge_color(self, color: Color) -> 'LegendFormatter':
+        """
+        Set the edge color of the legend frame.
+        """
+        self._legend.get_frame().set_edgecolor(color)
+        return self
+
+    def set_frame_on(self, on: bool = True) -> 'LegendFormatter':
+        """
+        Turn the frame on or off.
+        """
+        self._legend.set_frame_on(b=on)
+        return self
+
+    def set_z_order(self, level: int) -> 'LegendFormatter':
+        """
+        Set the z-order of the legend.
+        """
+        self._legend.set_zorder(level=level)
+        return self
+
+    def set_title_text(self, text: str) -> 'LegendFormatter':
+        """
+        Set the text of the legend title.
+        """
+        self.title.set_text(text)
+        return self
+
+    def set_title_font_family(self, font_name: str) -> 'LegendFormatter':
+        """
+        Set the font family of the legend title.
+        """
+        self.title.set_font_family(font_name)
+        return self
+
+    def set_title_font_size(self, font_size: FontSize) -> 'LegendFormatter':
+        """
+        Set the font size of the legend title.
+        """
+        self.title.set_size(font_size=font_size)
+        return self
+
+    def set_n_cols(self, n_cols: int) -> 'LegendFormatter':
+        """
+        Set the number of columns the legend has.
+
+        N.B. this creates a new legend. May need to set the following properties
+        manually afterwards as they cannot be automatically determined from the
+        old legend:
+        ['loc', 'markerfirst', 'fancybox', 'bbox_to_anchor' 'bbox_transform',
+        'handler_map']
+        """
+        self.recreate_legend(n_cols=n_cols)
+        return self
+
+    def set_line_points(self, num_points: int) -> 'LegendFormatter':
+        """
+        Set the number of points for a line legend entry.
+
+        N.B. this creates a new legend. May need to set the following properties
+        manually afterwards as they cannot be automatically determined from the
+        old legend:
+        ['loc', 'markerfirst', 'fancybox', 'bbox_to_anchor' 'bbox_transform',
+        'handler_map']
+        """
+        self.recreate_legend(line_points=num_points)
+        return self
+
+    def set_scatter_points(self, num_points: int) -> 'LegendFormatter':
+        """
+        Set the number of points for a scatter legend entry.
+
+        N.B. this creates a new legend. May need to set the following properties
+        manually afterwards as they cannot be automatically determined from the
+        old legend:
+        ['loc', 'markerfirst', 'fancybox', 'bbox_to_anchor' 'bbox_transform',
+        'handler_map']
+        """
+        self.recreate_legend(scatter_points=num_points)
+        return self
+
+    def set_shadow(self, on: bool = True) -> 'LegendFormatter':
+        """
+        Turn the shadow on or off for the legend frame.
+        """
+        self._legend.shadow = on
+        return self
```

### Comparing `mpl_format-0.317/mpl_format/literals.py` & `mpl_format-0.318/mpl_format/literals.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing_extensions import Literal   # can't use typing.Literal for Python < 3.8
-
-H_ALIGN = Literal['left', 'center', 'right']
-V_ALIGN = Literal['top', 'center', 'bottom']
-TEXT_V_ALIGN = Literal['top', 'center', 'bottom', 'baseline', 'center_baseline']
-ROTATION_MODE = Literal['absolute', 'relative']
-WHICH_TICKS = Literal['major', 'minor', 'both']
-WHICH_AXIS = Literal['x', 'y', 'both']
-SHARE_AXES = Literal['none', 'all', 'row', 'col']
-FIGURE_UNITS = Literal['inches', 'pixels']
-AXIS_SCALE = Literal['log', 'linear', 'symlog', 'logit']
-LINE_STYLE_STR = ['solid', 'dashed', 'dashdot', 'dotted']
-ASPECT = Literal['auto', 'equal']
-ANCHOR = ['NW', 'N', 'NE', 'W', 'C', 'E', 'SW', 'S', 'SE']
+from typing_extensions import Literal   # can't use typing.Literal for Python < 3.8
+
+H_ALIGN = Literal['left', 'center', 'right']
+V_ALIGN = Literal['top', 'center', 'bottom']
+TEXT_V_ALIGN = Literal['top', 'center', 'bottom', 'baseline', 'center_baseline']
+ROTATION_MODE = Literal['absolute', 'relative']
+WHICH_TICKS = Literal['major', 'minor', 'both']
+WHICH_AXIS = Literal['x', 'y', 'both']
+SHARE_AXES = Literal['none', 'all', 'row', 'col']
+FIGURE_UNITS = Literal['inches', 'pixels']
+AXIS_SCALE = Literal['log', 'linear', 'symlog', 'logit']
+LINE_STYLE_STR = ['solid', 'dashed', 'dashdot', 'dotted']
+ASPECT = Literal['auto', 'equal']
+ANCHOR = ['NW', 'N', 'NE', 'W', 'C', 'E', 'SW', 'S', 'SE']
```

### Comparing `mpl_format-0.317/mpl_format/patches/arc_list_formatter.py` & `mpl_format-0.318/mpl_format/patches/arc_list_formatter.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from typing import List
-
-from matplotlib.patches import Arc
-
-from mpl_format.patches import PatchListFormatter
-
-
-class ArcListFormatter(PatchListFormatter):
-
-    _patches: List[Arc]
-
-    def __init__(self, patches: List[Arc]):
-
-        super().__init__(patches)
-
-    def x_centers(self) -> List[float]:
-
-        return [arc.get_center()[0] for arc in self._patches]
-
-    def y_centers(self) -> List[float]:
-
-        return [arc.get_center()[1] for arc in self._patches]
-
-    def widths(self) -> List[float]:
-
-        return [arc.width for arc in self._patches]
-
-    def heights(self) -> List[float]:
-
-        return [arc.height for arc in self._patches]
-
-    def angles(self) -> List[float]:
-
-        return [arc.angle for arc in self._patches]
-
-    def theta_starts(self) -> List[float]:
-
-        return [arc.theta1 for arc in self._patches]
-
-    def theta_ends(self) -> List[float]:
-
-        return [arc.theta2 for arc in self._patches]
+from typing import List
+
+from matplotlib.patches import Arc
+
+from mpl_format.patches import PatchListFormatter
+
+
+class ArcListFormatter(PatchListFormatter):
+
+    _patches: List[Arc]
+
+    def __init__(self, patches: List[Arc]):
+
+        super().__init__(patches)
+
+    def x_centers(self) -> List[float]:
+
+        return [arc.get_center()[0] for arc in self._patches]
+
+    def y_centers(self) -> List[float]:
+
+        return [arc.get_center()[1] for arc in self._patches]
+
+    def widths(self) -> List[float]:
+
+        return [arc.width for arc in self._patches]
+
+    def heights(self) -> List[float]:
+
+        return [arc.height for arc in self._patches]
+
+    def angles(self) -> List[float]:
+
+        return [arc.angle for arc in self._patches]
+
+    def theta_starts(self) -> List[float]:
+
+        return [arc.theta1 for arc in self._patches]
+
+    def theta_ends(self) -> List[float]:
+
+        return [arc.theta2 for arc in self._patches]
```

### Comparing `mpl_format-0.317/mpl_format/plots/density.py` & `mpl_format-0.318/mpl_format/plots/density.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,288 +1,288 @@
-import matplotlib.pyplot as plt
-from numpy import log10, inf
-from typing import Optional, List, Union, Tuple
-
-from matplotlib.axes import Axes
-from numpy import concatenate
-from pandas import DataFrame, cut
-
-from mpl_format.axes import AxesFormatter
-from mpl_format.axes.axis_utils import new_axes
-from mpl_format.compound_types import Color
-
-
-def categorical_discrete_values_histogram(
-        data: DataFrame,
-        x: str, y: str,
-        categories: Optional[List[str]] = None,
-        colors: Union[Color, List[Color]] = 'k',
-        norm: str = 'single',
-        mean: Optional[Color] = None,
-        median: Optional[Color] = None,
-        ax: Optional[Axes] = None
-):
-    """
-    Plot a histogram of several categories together.
-
-    :param data: DataFrame with columns x and y
-    :param x: Name of the category column. Categories will be found from the
-              unique values of this column.
-    :param y: Name of the value column. Each value is assumed to be a count,
-              and the number of each count value will be counted.
-    :param categories: Optional override for categories of x. Use to select a
-                       subset of x, or to reorder x.
-    :param colors: Single color or list of colors to override default color of
-                   each histogram.
-    :param norm: Whether to normalize the density to the max of each category
-                 ('single'), or the max of all categories ('all').
-    :param mean: Color for lines showing the mean of each distribution.
-    :param median: Color for lines showing the median of each distribution.
-    :param ax: Optional matplotlib Axes instance to plot on.
-    """
-    ax: Axes = ax or new_axes()
-    axf = AxesFormatter(ax)
-    # get categories
-    if categories is None:
-        categories = data[x].unique()
-    num_cats = len(categories)
-    # colors
-    if not isinstance(colors, list):
-        colors = [colors] * num_cats
-    # filter to category data
-    data = data.loc[data[x].isin(categories)]
-    # find max and min values for scaling
-    y_min = data[y].min()
-    y_max = data[y].max()
-    # get counts for histogram
-    z = data.groupby([x, y]).size()
-    z_max = z.max()
-    # plot densities
-    for c, category, color in zip(
-        range(1, num_cats + 1),
-        categories,
-        colors
-    ):
-        cat_hist = z.loc[category, :]
-        if norm == 'all':
-            z_max_cat = z_max
-        elif norm == 'single':
-            z_max_cat = cat_hist.max()
-        else:
-            raise ValueError('norm must be in {"all", "single"}')
-        for (_, y_i), z_i in cat_hist.items():
-            axf.add_rectangle(
-                width=0.8, height=1,
-                x_center=c, y_center=y_i,
-                alpha=z_i / z_max_cat,
-                color=color
-            )
-        if mean is not None:
-            cat_mean = data.loc[data[x] == category, y].mean()
-            axf.add_line(x=[c - 0.4, c + 0.4],
-                         y=[cat_mean, cat_mean],
-                         color=mean)
-        if median is not None:
-            cat_median = data.loc[data[x] == category, y].median()
-            axf.add_line(x=[c - 0.4, c + 0.4],
-                         y=[cat_median, cat_median],
-                         color=median)
-    # format axes
-    axf.set_x_min(0.5)
-    axf.set_x_max(len(categories) + 0.5)
-    axf.set_y_min(y_min - 1)
-    axf.set_y_max(y_max + 1)
-    axf.x_ticks.set_locations(list(range(1, 1 + len(categories))))
-    axf.x_ticks.set_labels(categories)
-    axf.set_text(x_label=x, y_label=y)
-
-    return ax
-
-
-def categorical_continuous_values_histogram(
-        data: DataFrame,
-        x: str, y: str,
-        log_y: bool = False,
-        bins: int = 100,
-        q_lim: Optional[Tuple[float, float]] = None,
-        categories: Optional[List[str]] = None,
-        colors: Union[Color, List[Color]] = 'k',
-        norm: str = 'single',
-        mean: Optional[Color] = None,
-        median: Optional[Color] = None,
-        ax: Optional[Axes] = None
-):
-    """
-    Plot a histogram of several categories together.
-
-    :param data: DataFrame with columns x and y
-    :param x: Name of the category column. Categories will be found from the
-              unique values of this column.
-    :param y: Name of the value column. Each value is assumed to be a count,
-              and the number of each count value will be counted.
-    :param log_y: Whether to take log10 of the data.
-    :param bins: Number of equally-spaced bins to cut the data into.
-    :param q_lim: Optional percentile range to filter to e.g. (0, 0.99).
-    :param categories: Optional override for categories of x. Use to select a
-                       subset of x, or to reorder x.
-    :param colors: Single color or list of colors to override default color of
-                   each histogram.
-    :param norm: Whether to normalize the density to the max of each category
-                 ('single'), or the max of all categories ('all').
-    :param mean: Color for lines showing the mean of each distribution.
-    :param median: Color for lines showing the median of each distribution.
-    :param ax: Optional matplotlib Axes instance to plot on.
-    """
-    ax: Axes = ax or new_axes()
-    axf = AxesFormatter(ax)
-    # get categories
-    if categories is None:
-        categories = data[x].unique()
-    num_cats = len(categories)
-    # colors
-    if not isinstance(colors, list):
-        colors = [colors] * num_cats
-    # filter to category data
-    data = data.loc[data[x].isin(categories)]
-    # filter non-positive values for log-transform
-    if log_y:
-        data = data.loc[data['y'] > 0]
-    # find max and min values for scaling
-    if log_y:
-        y_log = data[y].map(log10)
-        y_min = y_log.min()
-        y_max = y_log.max()
-    else:
-        y_min = data[y].min()
-        y_max = data[y].max()
-    # get counts for histogram
-    z = {}
-    z_max_cats = {}
-    # calculate counts and maxes
-    for category in categories:
-        cat_data = data.loc[data[x] == category, y]
-        if log_y:
-            cat_data = cat_data.map(log10)
-        if q_lim is not None:
-            q_low, q_high = cat_data.quantile([q_lim[0], q_lim[1]])
-            cat_data = cat_data.loc[
-                (cat_data >= q_low) & (cat_data <= q_high)
-            ]
-        z[category] = cut(cat_data, bins).value_counts().sort_index()
-        z_max_cats[category] = z[category].max()
-    z_max = max(z_max_cats.values())
-    # plot densities
-    for c, category, color in zip(
-            range(1, num_cats + 1),
-            categories,
-            colors
-    ):
-        if norm == 'all':
-            z_max_cat = z_max
-        elif norm == 'single':
-            z_max_cat = z_max_cats[category]
-        else:
-            raise ValueError('norm must be in {"all", "single"}')
-        for rng, z_i in z[category].items():
-            axf.add_rectangle(
-                width=0.8, height=rng.length,
-                x_center=c, y_center=rng.mid,
-                alpha=z_i / z_max_cat,
-                color=color
-            )
-        if mean is not None:
-            cat_mean = data.loc[data[x] == category, y].mean()
-            if log_y:
-                cat_mean = log10(cat_mean)
-            axf.add_line(x=[c - 0.4, c + 0.4],
-                         y=[cat_mean, cat_mean],
-                         color=mean)
-        if median is not None:
-            cat_median = data.loc[data[x] == category, y].median()
-            if log_y:
-                cat_median = log10(cat_median)
-            axf.add_line(x=[c - 0.4, c + 0.4],
-                         y=[cat_median, cat_median],
-                         color=median)
-    # format axes
-    axf.set_x_min(0.5)
-    axf.set_x_max(len(categories) + 0.5)
-    axf.set_y_min(y_min - 1)
-    axf.set_y_max(y_max + 1)
-    axf.x_ticks.set_locations(list(range(1, 1 + len(categories))))
-    axf.x_ticks.set_labels(categories)
-    axf.set_text(x_label=x, y_label=y)
-
-    return ax
-
-
-def do_test_discrete_plot():
-
-    from scipy.stats import poisson
-    p = concatenate([
-        poisson(3).rvs(1_000),
-        poisson(7).rvs(1_000),
-        poisson(10).rvs(1_000)
-    ])
-    d = DataFrame({
-        'y': p,
-        'x': ['a'] * 1000 + ['b'] * 1_000 + ['c'] * 1_000
-    })
-    ax = categorical_discrete_values_histogram(
-        data=d, x='x', y='y'
-    )
-    plt.show()
-    ax = categorical_discrete_values_histogram(
-        data=d, x='x', y='y', categories=['c', 'a']
-    )
-    plt.show()
-    ax = categorical_discrete_values_histogram(
-        data=d, x='x', y='y', categories=['c', 'a'], colors=['r', 'g']
-    )
-    AxesFormatter(ax).set_axis_below().grid()
-    ax = categorical_discrete_values_histogram(
-        data=d, x='x', y='y', categories=['c', 'a'], colors=['r', 'g'],
-        norm='all', mean='b', median='purple'
-    )
-    AxesFormatter(ax).set_axis_below().grid()
-    plt.show()
-
-
-def do_test_continuous_plot():
-
-    from scipy.stats import norm
-    n = concatenate([
-        norm(5, 1).rvs(10_000),
-        norm(7, 2).rvs(10_000),
-        norm(10, 1).rvs(10_000)
-    ])
-    d = DataFrame({
-        'y': n,
-        'x': ['a'] * 10_000 + ['b'] * 10_000 + ['c'] * 10_000
-    })
-    ax = categorical_continuous_values_histogram(
-        data=d, x='x', y='y',
-        categories=['c', 'a', 'b'], colors=['b', 'r', 'g'],
-        norm='all', mean='b', median='purple',
-        log_y=False
-    )
-    plt.show()
-    ax = categorical_continuous_values_histogram(
-        data=d, x='x', y='y',
-        categories=['c', 'a', 'b'], colors=['b', 'r', 'g'],
-        norm='all', mean='b', median='purple',
-        log_y=True
-    )
-    plt.show()
-    ax = categorical_continuous_values_histogram(
-        data=d, x='x', y='y',
-        categories=['c', 'a', 'b'], colors=['b', 'r', 'g'],
-        norm='all', mean='b', median='purple',
-        log_y=False, q_lim=(0.1, 0.9)
-    )
-    plt.show()
-
-
-if __name__ == '__main__':
-
-    # do_test_discrete_plot()
-    do_test_continuous_plot()
+import matplotlib.pyplot as plt
+from numpy import log10, inf
+from typing import Optional, List, Union, Tuple
+
+from matplotlib.axes import Axes
+from numpy import concatenate
+from pandas import DataFrame, cut
+
+from mpl_format.axes import AxesFormatter
+from mpl_format.axes.axis_utils import new_axes
+from mpl_format.compound_types import Color
+
+
+def categorical_discrete_values_histogram(
+        data: DataFrame,
+        x: str, y: str,
+        categories: Optional[List[str]] = None,
+        colors: Union[Color, List[Color]] = 'k',
+        norm: str = 'single',
+        mean: Optional[Color] = None,
+        median: Optional[Color] = None,
+        ax: Optional[Axes] = None
+):
+    """
+    Plot a histogram of several categories together.
+
+    :param data: DataFrame with columns x and y
+    :param x: Name of the category column. Categories will be found from the
+              unique values of this column.
+    :param y: Name of the value column. Each value is assumed to be a count,
+              and the number of each count value will be counted.
+    :param categories: Optional override for categories of x. Use to select a
+                       subset of x, or to reorder x.
+    :param colors: Single color or list of colors to override default color of
+                   each histogram.
+    :param norm: Whether to normalize the density to the max of each category
+                 ('single'), or the max of all categories ('all').
+    :param mean: Color for lines showing the mean of each distribution.
+    :param median: Color for lines showing the median of each distribution.
+    :param ax: Optional matplotlib Axes instance to plot on.
+    """
+    ax: Axes = ax or new_axes()
+    axf = AxesFormatter(ax)
+    # get categories
+    if categories is None:
+        categories = data[x].unique()
+    num_cats = len(categories)
+    # colors
+    if not isinstance(colors, list):
+        colors = [colors] * num_cats
+    # filter to category data
+    data = data.loc[data[x].isin(categories)]
+    # find max and min values for scaling
+    y_min = data[y].min()
+    y_max = data[y].max()
+    # get counts for histogram
+    z = data.groupby([x, y]).size()
+    z_max = z.max()
+    # plot densities
+    for c, category, color in zip(
+        range(1, num_cats + 1),
+        categories,
+        colors
+    ):
+        cat_hist = z.loc[category, :]
+        if norm == 'all':
+            z_max_cat = z_max
+        elif norm == 'single':
+            z_max_cat = cat_hist.max()
+        else:
+            raise ValueError('norm must be in {"all", "single"}')
+        for (_, y_i), z_i in cat_hist.items():
+            axf.add_rectangle(
+                width=0.8, height=1,
+                x_center=c, y_center=y_i,
+                alpha=z_i / z_max_cat,
+                color=color
+            )
+        if mean is not None:
+            cat_mean = data.loc[data[x] == category, y].mean()
+            axf.add_line(x=[c - 0.4, c + 0.4],
+                         y=[cat_mean, cat_mean],
+                         color=mean)
+        if median is not None:
+            cat_median = data.loc[data[x] == category, y].median()
+            axf.add_line(x=[c - 0.4, c + 0.4],
+                         y=[cat_median, cat_median],
+                         color=median)
+    # format axes
+    axf.set_x_min(0.5)
+    axf.set_x_max(len(categories) + 0.5)
+    axf.set_y_min(y_min - 1)
+    axf.set_y_max(y_max + 1)
+    axf.x_ticks.set_locations(list(range(1, 1 + len(categories))))
+    axf.x_ticks.set_labels(categories)
+    axf.set_text(x_label=x, y_label=y)
+
+    return ax
+
+
+def categorical_continuous_values_histogram(
+        data: DataFrame,
+        x: str, y: str,
+        log_y: bool = False,
+        bins: int = 100,
+        q_lim: Optional[Tuple[float, float]] = None,
+        categories: Optional[List[str]] = None,
+        colors: Union[Color, List[Color]] = 'k',
+        norm: str = 'single',
+        mean: Optional[Color] = None,
+        median: Optional[Color] = None,
+        ax: Optional[Axes] = None
+):
+    """
+    Plot a histogram of several categories together.
+
+    :param data: DataFrame with columns x and y
+    :param x: Name of the category column. Categories will be found from the
+              unique values of this column.
+    :param y: Name of the value column. Each value is assumed to be a count,
+              and the number of each count value will be counted.
+    :param log_y: Whether to take log10 of the data.
+    :param bins: Number of equally-spaced bins to cut the data into.
+    :param q_lim: Optional percentile range to filter to e.g. (0, 0.99).
+    :param categories: Optional override for categories of x. Use to select a
+                       subset of x, or to reorder x.
+    :param colors: Single color or list of colors to override default color of
+                   each histogram.
+    :param norm: Whether to normalize the density to the max of each category
+                 ('single'), or the max of all categories ('all').
+    :param mean: Color for lines showing the mean of each distribution.
+    :param median: Color for lines showing the median of each distribution.
+    :param ax: Optional matplotlib Axes instance to plot on.
+    """
+    ax: Axes = ax or new_axes()
+    axf = AxesFormatter(ax)
+    # get categories
+    if categories is None:
+        categories = data[x].unique()
+    num_cats = len(categories)
+    # colors
+    if not isinstance(colors, list):
+        colors = [colors] * num_cats
+    # filter to category data
+    data = data.loc[data[x].isin(categories)]
+    # filter non-positive values for log-transform
+    if log_y:
+        data = data.loc[data['y'] > 0]
+    # find max and min values for scaling
+    if log_y:
+        y_log = data[y].map(log10)
+        y_min = y_log.min()
+        y_max = y_log.max()
+    else:
+        y_min = data[y].min()
+        y_max = data[y].max()
+    # get counts for histogram
+    z = {}
+    z_max_cats = {}
+    # calculate counts and maxes
+    for category in categories:
+        cat_data = data.loc[data[x] == category, y]
+        if log_y:
+            cat_data = cat_data.map(log10)
+        if q_lim is not None:
+            q_low, q_high = cat_data.quantile([q_lim[0], q_lim[1]])
+            cat_data = cat_data.loc[
+                (cat_data >= q_low) & (cat_data <= q_high)
+            ]
+        z[category] = cut(cat_data, bins).value_counts().sort_index()
+        z_max_cats[category] = z[category].max()
+    z_max = max(z_max_cats.values())
+    # plot densities
+    for c, category, color in zip(
+            range(1, num_cats + 1),
+            categories,
+            colors
+    ):
+        if norm == 'all':
+            z_max_cat = z_max
+        elif norm == 'single':
+            z_max_cat = z_max_cats[category]
+        else:
+            raise ValueError('norm must be in {"all", "single"}')
+        for rng, z_i in z[category].items():
+            axf.add_rectangle(
+                width=0.8, height=rng.length,
+                x_center=c, y_center=rng.mid,
+                alpha=z_i / z_max_cat,
+                color=color
+            )
+        if mean is not None:
+            cat_mean = data.loc[data[x] == category, y].mean()
+            if log_y:
+                cat_mean = log10(cat_mean)
+            axf.add_line(x=[c - 0.4, c + 0.4],
+                         y=[cat_mean, cat_mean],
+                         color=mean)
+        if median is not None:
+            cat_median = data.loc[data[x] == category, y].median()
+            if log_y:
+                cat_median = log10(cat_median)
+            axf.add_line(x=[c - 0.4, c + 0.4],
+                         y=[cat_median, cat_median],
+                         color=median)
+    # format axes
+    axf.set_x_min(0.5)
+    axf.set_x_max(len(categories) + 0.5)
+    axf.set_y_min(y_min - 1)
+    axf.set_y_max(y_max + 1)
+    axf.x_ticks.set_locations(list(range(1, 1 + len(categories))))
+    axf.x_ticks.set_labels(categories)
+    axf.set_text(x_label=x, y_label=y)
+
+    return ax
+
+
+def do_test_discrete_plot():
+
+    from scipy.stats import poisson
+    p = concatenate([
+        poisson(3).rvs(1_000),
+        poisson(7).rvs(1_000),
+        poisson(10).rvs(1_000)
+    ])
+    d = DataFrame({
+        'y': p,
+        'x': ['a'] * 1000 + ['b'] * 1_000 + ['c'] * 1_000
+    })
+    ax = categorical_discrete_values_histogram(
+        data=d, x='x', y='y'
+    )
+    plt.show()
+    ax = categorical_discrete_values_histogram(
+        data=d, x='x', y='y', categories=['c', 'a']
+    )
+    plt.show()
+    ax = categorical_discrete_values_histogram(
+        data=d, x='x', y='y', categories=['c', 'a'], colors=['r', 'g']
+    )
+    AxesFormatter(ax).set_axis_below().grid()
+    ax = categorical_discrete_values_histogram(
+        data=d, x='x', y='y', categories=['c', 'a'], colors=['r', 'g'],
+        norm='all', mean='b', median='purple'
+    )
+    AxesFormatter(ax).set_axis_below().grid()
+    plt.show()
+
+
+def do_test_continuous_plot():
+
+    from scipy.stats import norm
+    n = concatenate([
+        norm(5, 1).rvs(10_000),
+        norm(7, 2).rvs(10_000),
+        norm(10, 1).rvs(10_000)
+    ])
+    d = DataFrame({
+        'y': n,
+        'x': ['a'] * 10_000 + ['b'] * 10_000 + ['c'] * 10_000
+    })
+    ax = categorical_continuous_values_histogram(
+        data=d, x='x', y='y',
+        categories=['c', 'a', 'b'], colors=['b', 'r', 'g'],
+        norm='all', mean='b', median='purple',
+        log_y=False
+    )
+    plt.show()
+    ax = categorical_continuous_values_histogram(
+        data=d, x='x', y='y',
+        categories=['c', 'a', 'b'], colors=['b', 'r', 'g'],
+        norm='all', mean='b', median='purple',
+        log_y=True
+    )
+    plt.show()
+    ax = categorical_continuous_values_histogram(
+        data=d, x='x', y='y',
+        categories=['c', 'a', 'b'], colors=['b', 'r', 'g'],
+        norm='all', mean='b', median='purple',
+        log_y=False, q_lim=(0.1, 0.9)
+    )
+    plt.show()
+
+
+if __name__ == '__main__':
+
+    # do_test_discrete_plot()
+    do_test_continuous_plot()
```

### Comparing `mpl_format-0.317/mpl_format/text/text_formatter.py` & `mpl_format-0.318/mpl_format/text/text_formatter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,283 +1,283 @@
-from matplotlib.text import Text
-from typing import Dict, Union, Callable
-
-from mpl_format.compound_types import FontSize
-from mpl_format.enums import FONT_SIZE
-from mpl_format.literals import ROTATION_MODE, H_ALIGN, TEXT_V_ALIGN
-from mpl_format.text.text_utils import wrap_text, remove_parenthesized_text, \
-    HORIZONTAL_ALIGNMENTS, VERTICAL_ALIGNMENTS
-
-
-class TextFormatter(object):
-
-    def __init__(self, text: Text):
-        """
-        Create a new TextFormatter for a matplotlib Text instance.
-
-        :param text: The matplotlib Text instance to wrap.
-        """
-        self._text: Text = text
-
-    @property
-    def text(self) -> Text:
-        """
-        Return the wrapped matplotlib Text instance.
-        """
-        return self._text
-
-    def to_string(self) -> str:
-        """
-        Return the text of the wrapped matplotlib Text instance.
-        """
-        return self._text.get_text()
-
-    def wrap(self, max_width: int) -> 'TextFormatter':
-        """
-        Wrap the text with new lines if it exceeds a given width of characters.
-
-        :param max_width: The maximum character width per line.
-        """
-        wrapped = wrap_text(self.to_string(), max_width=max_width)
-        self._text.set_text(wrapped)
-        return self
-
-    def rotate(
-            self, rotation: Union[str, int],
-            how: ROTATION_MODE = 'absolute'
-    ) -> 'TextFormatter':
-        """
-        Set the rotation of the text.
-
-        :param rotation: The rotation value to set in degrees, 'horizontal'
-                         or 'vertical'.
-        :param how: 'absolute' or 'relative'
-        """
-        if how == 'relative' and not isinstance(rotation, str):
-            self._text.set_rotation(self._text.get_rotation() + rotation)
-        elif how == 'absolute':
-            self._text.set_rotation(rotation)
-        else:
-            raise ValueError("`how` must be 'absolute' or 'relative'")
-        return self
-
-    def map(
-            self, mapping: Union[Dict[str, str], Callable[[str], str]]
-    ) -> 'TextFormatter':
-        """
-        Replace text using a dictionary or function.
-
-        :param mapping: Mappings to replace text.
-        """
-        if isinstance(mapping, dict):
-            if self.to_string() in mapping.keys():
-                self._text.set_text(mapping[self.to_string()])
-        elif callable(mapping):
-            self._text.set_text(mapping(self.to_string()))
-        else:
-            raise TypeError('mapping must be a dict or callable')
-        return self
-
-    def remove_parenthesized_text(self) -> 'TextFormatter':
-        """
-        Remove any text inside parentheses, along with the parentheses.
-        """
-        self._text.set_text(remove_parenthesized_text(self.to_string()))
-        return self
-
-    def replace(self, old: str, new: str) -> 'TextFormatter':
-        """
-        Replace old text with new text.
-
-        :param old: The text to remove.
-        :param new: The text to insert.
-        """
-        self._text.set_text(
-            self.to_string().replace(old, new)
-        )
-        return self
-
-    def set_text(self, text: str) -> 'TextFormatter':
-        """
-        Set the text string.
-        """
-        self._text.set_text(text)
-        return self
-
-    def clear(self) -> 'TextFormatter':
-        """
-        Clear the text string.
-        """
-        self.set_text('')
-        return self
-
-    # region set size
-
-    def set_size(self, font_size: FontSize) -> 'TextFormatter':
-        """
-        Set the font size for the Text.
-        """
-        if isinstance(font_size, FONT_SIZE):
-            font_size = font_size.get_name()
-        self._text.set_fontsize(font_size)
-        return self
-    
-    def set_size_xx_small(self) -> 'TextFormatter':
-        self.set_size('xx-small')
-        return self
-
-    def set_size_x_small(self) -> 'TextFormatter':
-        self.set_size('x-small')
-        return self
-
-    def set_size_small(self) -> 'TextFormatter':
-        self.set_size('small')
-        return self
-
-    def set_size_medium(self) -> 'TextFormatter':
-        self.set_size('medium')
-        return self
-
-    def set_size_large(self) -> 'TextFormatter':
-        self.set_size('large')
-        return self
-
-    def set_size_x_large(self) -> 'TextFormatter':
-        self.set_size('x-large')
-        return self
-
-    def set_size_xx_large(self) -> 'TextFormatter':
-        self.set_size('xx-large')
-        return self
-
-    def set_size_larger(self) -> 'TextFormatter':
-        self.set_size('larger')
-        return self
-
-    def set_size_smaller(self) -> 'TextFormatter':
-        self.set_size('smaller')
-        return self
-
-    # endregion
-
-    # region set font family
-
-    def set_font_family(self, font_name: str) -> 'TextFormatter':
-        """
-        Set the font family to the given font name.
-
-        :param font_name: Name of the font to set.
-        """
-        self._text.set_fontfamily(fontname=font_name)
-        return self
-
-    def set_font_family_serif(self) -> 'TextFormatter':
-        """
-        Set the font family to 'serif'
-        """
-        self.set_font_family('serif')
-        return self
-
-    def set_font_family_sans_serif(self) -> 'TextFormatter':
-        """
-        Set the font family to 'sans-serif'
-        """
-        self.set_font_family('sans-serif')
-        return self
-
-    def set_font_family_cursive(self) -> 'TextFormatter':
-        """
-        Set the font family to 'cursive'
-        """
-        self.set_font_family('cursive')
-        return self
-
-    def set_font_family_fantasy(self) -> 'TextFormatter':
-        """
-        Set the font family to 'fantasy'
-        """
-        self.set_font_family('fantasy')
-        return self
-
-    def set_font_family_monospace(self) -> 'TextFormatter':
-        """
-        Set the font family to 'monospace'
-        """
-        self.set_font_family('monospace')
-        return self
-
-    def set_font_family_benton_sans_f(self) -> 'TextFormatter':
-        """
-        Set the font family to 'BentonSansF'
-        """
-        self.set_font_family('BentonSansF')
-        return self
-
-    def set_font_family_quarto(self) -> 'TextFormatter':
-        """
-        Set the font family to 'Quarto'
-        """
-        self.set_font_family('Quarto')
-        return self
-
-    def set_font_family_calibri(self) -> 'TextFormatter':
-        """
-        Set the font family to 'Calibri'
-        """
-        self.set_font_family('Calibri')
-        return self
-
-    # endregion
-
-    # region set alignment
-
-    def set_ha(self, alignment: H_ALIGN) -> 'TextFormatter':
-
-        if alignment not in HORIZONTAL_ALIGNMENTS:
-            raise ValueError(
-                f'alignment must be one of {HORIZONTAL_ALIGNMENTS}'
-            )
-        self._text.set_horizontalalignment(align=alignment)
-        return self
-
-    def set_ha_left(self) -> 'TextFormatter':
-
-        return self.set_ha('left')
-
-    def set_ha_center(self) -> 'TextFormatter':
-
-        return self.set_ha('center')
-
-    def set_ha_right(self) -> 'TextFormatter':
-
-        return self.set_ha('right')
-
-    def set_va(self, alignment: TEXT_V_ALIGN) -> 'TextFormatter':
-
-        if alignment not in VERTICAL_ALIGNMENTS:
-            raise ValueError(
-                f'alignment must be one of {VERTICAL_ALIGNMENTS}'
-            )
-        self._text.set_verticalalignment(align=alignment)
-        return self
-
-    def set_va_top(self) -> 'TextFormatter':
-
-        return self.set_va('top')
-
-    def set_va_center(self) -> 'TextFormatter':
-
-        return self.set_va('center')
-
-    def set_va_bottom(self) -> 'TextFormatter':
-
-        return self.set_va('bottom')
-
-    def set_va_baseline(self) -> 'TextFormatter':
-
-        return self.set_va('baseline')
-
-    def set_va_center_baseline(self) -> 'TextFormatter':
-
-        return self.set_va('center_baseline')
-
-    # endregion
+from matplotlib.text import Text
+from typing import Dict, Union, Callable
+
+from mpl_format.compound_types import FontSize
+from mpl_format.enums import FONT_SIZE
+from mpl_format.literals import ROTATION_MODE, H_ALIGN, TEXT_V_ALIGN
+from mpl_format.text.text_utils import wrap_text, remove_parenthesized_text, \
+    HORIZONTAL_ALIGNMENTS, VERTICAL_ALIGNMENTS
+
+
+class TextFormatter(object):
+
+    def __init__(self, text: Text):
+        """
+        Create a new TextFormatter for a matplotlib Text instance.
+
+        :param text: The matplotlib Text instance to wrap.
+        """
+        self._text: Text = text
+
+    @property
+    def text(self) -> Text:
+        """
+        Return the wrapped matplotlib Text instance.
+        """
+        return self._text
+
+    def to_string(self) -> str:
+        """
+        Return the text of the wrapped matplotlib Text instance.
+        """
+        return self._text.get_text()
+
+    def wrap(self, max_width: int) -> 'TextFormatter':
+        """
+        Wrap the text with new lines if it exceeds a given width of characters.
+
+        :param max_width: The maximum character width per line.
+        """
+        wrapped = wrap_text(self.to_string(), max_width=max_width)
+        self._text.set_text(wrapped)
+        return self
+
+    def rotate(
+            self, rotation: Union[str, int],
+            how: ROTATION_MODE = 'absolute'
+    ) -> 'TextFormatter':
+        """
+        Set the rotation of the text.
+
+        :param rotation: The rotation value to set in degrees, 'horizontal'
+                         or 'vertical'.
+        :param how: 'absolute' or 'relative'
+        """
+        if how == 'relative' and not isinstance(rotation, str):
+            self._text.set_rotation(self._text.get_rotation() + rotation)
+        elif how == 'absolute':
+            self._text.set_rotation(rotation)
+        else:
+            raise ValueError("`how` must be 'absolute' or 'relative'")
+        return self
+
+    def map(
+            self, mapping: Union[Dict[str, str], Callable[[str], str]]
+    ) -> 'TextFormatter':
+        """
+        Replace text using a dictionary or function.
+
+        :param mapping: Mappings to replace text.
+        """
+        if isinstance(mapping, dict):
+            if self.to_string() in mapping.keys():
+                self._text.set_text(mapping[self.to_string()])
+        elif callable(mapping):
+            self._text.set_text(mapping(self.to_string()))
+        else:
+            raise TypeError('mapping must be a dict or callable')
+        return self
+
+    def remove_parenthesized_text(self) -> 'TextFormatter':
+        """
+        Remove any text inside parentheses, along with the parentheses.
+        """
+        self._text.set_text(remove_parenthesized_text(self.to_string()))
+        return self
+
+    def replace(self, old: str, new: str) -> 'TextFormatter':
+        """
+        Replace old text with new text.
+
+        :param old: The text to remove.
+        :param new: The text to insert.
+        """
+        self._text.set_text(
+            self.to_string().replace(old, new)
+        )
+        return self
+
+    def set_text(self, text: str) -> 'TextFormatter':
+        """
+        Set the text string.
+        """
+        self._text.set_text(text)
+        return self
+
+    def clear(self) -> 'TextFormatter':
+        """
+        Clear the text string.
+        """
+        self.set_text('')
+        return self
+
+    # region set size
+
+    def set_size(self, font_size: FontSize) -> 'TextFormatter':
+        """
+        Set the font size for the Text.
+        """
+        if isinstance(font_size, FONT_SIZE):
+            font_size = font_size.get_name()
+        self._text.set_fontsize(font_size)
+        return self
+    
+    def set_size_xx_small(self) -> 'TextFormatter':
+        self.set_size('xx-small')
+        return self
+
+    def set_size_x_small(self) -> 'TextFormatter':
+        self.set_size('x-small')
+        return self
+
+    def set_size_small(self) -> 'TextFormatter':
+        self.set_size('small')
+        return self
+
+    def set_size_medium(self) -> 'TextFormatter':
+        self.set_size('medium')
+        return self
+
+    def set_size_large(self) -> 'TextFormatter':
+        self.set_size('large')
+        return self
+
+    def set_size_x_large(self) -> 'TextFormatter':
+        self.set_size('x-large')
+        return self
+
+    def set_size_xx_large(self) -> 'TextFormatter':
+        self.set_size('xx-large')
+        return self
+
+    def set_size_larger(self) -> 'TextFormatter':
+        self.set_size('larger')
+        return self
+
+    def set_size_smaller(self) -> 'TextFormatter':
+        self.set_size('smaller')
+        return self
+
+    # endregion
+
+    # region set font family
+
+    def set_font_family(self, font_name: str) -> 'TextFormatter':
+        """
+        Set the font family to the given font name.
+
+        :param font_name: Name of the font to set.
+        """
+        self._text.set_fontfamily(fontname=font_name)
+        return self
+
+    def set_font_family_serif(self) -> 'TextFormatter':
+        """
+        Set the font family to 'serif'
+        """
+        self.set_font_family('serif')
+        return self
+
+    def set_font_family_sans_serif(self) -> 'TextFormatter':
+        """
+        Set the font family to 'sans-serif'
+        """
+        self.set_font_family('sans-serif')
+        return self
+
+    def set_font_family_cursive(self) -> 'TextFormatter':
+        """
+        Set the font family to 'cursive'
+        """
+        self.set_font_family('cursive')
+        return self
+
+    def set_font_family_fantasy(self) -> 'TextFormatter':
+        """
+        Set the font family to 'fantasy'
+        """
+        self.set_font_family('fantasy')
+        return self
+
+    def set_font_family_monospace(self) -> 'TextFormatter':
+        """
+        Set the font family to 'monospace'
+        """
+        self.set_font_family('monospace')
+        return self
+
+    def set_font_family_benton_sans_f(self) -> 'TextFormatter':
+        """
+        Set the font family to 'BentonSansF'
+        """
+        self.set_font_family('BentonSansF')
+        return self
+
+    def set_font_family_quarto(self) -> 'TextFormatter':
+        """
+        Set the font family to 'Quarto'
+        """
+        self.set_font_family('Quarto')
+        return self
+
+    def set_font_family_calibri(self) -> 'TextFormatter':
+        """
+        Set the font family to 'Calibri'
+        """
+        self.set_font_family('Calibri')
+        return self
+
+    # endregion
+
+    # region set alignment
+
+    def set_ha(self, alignment: H_ALIGN) -> 'TextFormatter':
+
+        if alignment not in HORIZONTAL_ALIGNMENTS:
+            raise ValueError(
+                f'alignment must be one of {HORIZONTAL_ALIGNMENTS}'
+            )
+        self._text.set_horizontalalignment(align=alignment)
+        return self
+
+    def set_ha_left(self) -> 'TextFormatter':
+
+        return self.set_ha('left')
+
+    def set_ha_center(self) -> 'TextFormatter':
+
+        return self.set_ha('center')
+
+    def set_ha_right(self) -> 'TextFormatter':
+
+        return self.set_ha('right')
+
+    def set_va(self, alignment: TEXT_V_ALIGN) -> 'TextFormatter':
+
+        if alignment not in VERTICAL_ALIGNMENTS:
+            raise ValueError(
+                f'alignment must be one of {VERTICAL_ALIGNMENTS}'
+            )
+        self._text.set_verticalalignment(align=alignment)
+        return self
+
+    def set_va_top(self) -> 'TextFormatter':
+
+        return self.set_va('top')
+
+    def set_va_center(self) -> 'TextFormatter':
+
+        return self.set_va('center')
+
+    def set_va_bottom(self) -> 'TextFormatter':
+
+        return self.set_va('bottom')
+
+    def set_va_baseline(self) -> 'TextFormatter':
+
+        return self.set_va('baseline')
+
+    def set_va_center_baseline(self) -> 'TextFormatter':
+
+        return self.set_va('center_baseline')
+
+    # endregion
```

### Comparing `mpl_format-0.317/mpl_format/text/text_list_formatter.py` & `mpl_format-0.318/mpl_format/text/text_list_formatter.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-from typing import List
-
-from mpl_format.compound_types import FontSize
-from mpl_format.literals import TEXT_V_ALIGN, H_ALIGN
-from mpl_format.text.text_formatter import TextFormatter
-from mpl_format.text.text_utils import \
-    HORIZONTAL_ALIGNMENTS, VERTICAL_ALIGNMENTS
-
-
-class TextListFormatter(object):
-
-    def __init__(self, text_list: List[TextFormatter]):
-
-        self._text_list: List[TextFormatter] = text_list
-
-    # region set size
-
-    def set_size(self, font_size: FontSize) -> 'TextListFormatter':
-        """
-        Set the font size for each Text element.
-        """
-        for text in self._text_list:
-            text.set_size(font_size)
-        return self
-
-    def set_size_xx_small(self) -> 'TextListFormatter':
-        self.set_size('xx-small')
-        return self
-
-    def set_size_x_small(self) -> 'TextListFormatter':
-        self.set_size('x-small')
-        return self
-
-    def set_size_small(self) -> 'TextListFormatter':
-        self.set_size('small')
-        return self
-
-    def set_size_medium(self) -> 'TextListFormatter':
-        self.set_size('medium')
-        return self
-
-    def set_size_large(self) -> 'TextListFormatter':
-        self.set_size('large')
-        return self
-
-    def set_size_x_large(self) -> 'TextListFormatter':
-        self.set_size('x-large')
-        return self
-
-    def set_size_xx_large(self) -> 'TextListFormatter':
-        self.set_size('xx-large')
-        return self
-
-    def set_size_larger(self) -> 'TextListFormatter':
-        self.set_size('larger')
-        return self
-
-    def set_size_smaller(self) -> 'TextListFormatter':
-        self.set_size('smaller')
-        return self
-
-    # endregion
-
-    # region set font family
-
-    def set_font_family(self, font_name: str) -> 'TextListFormatter':
-        """
-        Set the font family to the given font name.
-
-        :param font_name: Name of the font to set.
-        """
-        for text in self._text_list:
-            text.set_font_family(font_name)
-        return self
-
-    def set_font_family_serif(self) -> 'TextListFormatter':
-        """
-        Set the font family to 'serif'
-        """
-        self.set_font_family('serif')
-        return self
-
-    def set_font_family_sans_serif(self) -> 'TextListFormatter':
-        """
-        Set the font family to 'sans-serif'
-        """
-        self.set_font_family('sans-serif')
-        return self
-
-    def set_font_family_cursive(self) -> 'TextListFormatter':
-        """
-        Set the font family to 'cursive'
-        """
-        self.set_font_family('cursive')
-        return self
-
-    def set_font_family_fantasy(self) -> 'TextListFormatter':
-        """
-        Set the font family to 'fantasy'
-        """
-        self.set_font_family('fantasy')
-        return self
-
-    def set_font_family_monospace(self) -> 'TextListFormatter':
-        """
-        Set the font family to 'monospace'
-        """
-        self.set_font_family('monospace')
-        return self
-
-    def set_font_family_benton_sans_f(self) -> 'TextListFormatter':
-        """
-        Set the font family to 'BentonSansF'
-        """
-        self.set_font_family('BentonSansF')
-        return self
-
-    def set_font_family_quarto(self) -> 'TextListFormatter':
-        """
-        Set the font family to 'Quarto'
-        """
-        self.set_font_family('Quarto')
-        return self
-
-    def set_font_family_calibri(self) -> 'TextListFormatter':
-        """
-        Set the font family to 'Calibri'
-        """
-        self.set_font_family('Calibri')
-        return self
-
-    # endregion
-
-    # region set alignment
-
-    def set_ha(self, alignment: H_ALIGN) -> 'TextListFormatter':
-
-        if alignment not in HORIZONTAL_ALIGNMENTS:
-            raise ValueError(
-                f'alignment must be one of {HORIZONTAL_ALIGNMENTS}'
-            )
-        for text in self._text_list:
-            text.set_ha(alignment=alignment)
-        return self
-
-    def set_ha_left(self) -> 'TextListFormatter':
-
-        return self.set_ha('left')
-
-    def set_ha_center(self) -> 'TextListFormatter':
-
-        return self.set_ha('center')
-
-    def set_ha_right(self) -> 'TextListFormatter':
-
-        return self.set_ha('right')
-
-    def set_va(self, alignment: TEXT_V_ALIGN) -> 'TextListFormatter':
-
-        if alignment not in VERTICAL_ALIGNMENTS:
-            raise ValueError(
-                f'alignment must be one of {VERTICAL_ALIGNMENTS}'
-            )
-        for text in self._text_list:
-            text.set_va(alignment=alignment)
-        return self
-
-    def set_va_top(self) -> 'TextListFormatter':
-
-        return self.set_va('top')
-
-    def set_va_center(self) -> 'TextListFormatter':
-
-        return self.set_va('center')
-
-    def set_va_bottom(self) -> 'TextListFormatter':
-
-        return self.set_va('bottom')
-
-    def set_va_baseline(self) -> 'TextListFormatter':
-
-        return self.set_va('baseline')
-
-    def set_va_center_baseline(self) -> 'TextListFormatter':
-
-        return self.set_va('center_baseline')
-
-    # endregion
-
-    @property
-    def texts(self) -> List[str]:
-
-        return[t.to_string() for t in self._text_list]
+from typing import List
+
+from mpl_format.compound_types import FontSize
+from mpl_format.literals import TEXT_V_ALIGN, H_ALIGN
+from mpl_format.text.text_formatter import TextFormatter
+from mpl_format.text.text_utils import \
+    HORIZONTAL_ALIGNMENTS, VERTICAL_ALIGNMENTS
+
+
+class TextListFormatter(object):
+
+    def __init__(self, text_list: List[TextFormatter]):
+
+        self._text_list: List[TextFormatter] = text_list
+
+    # region set size
+
+    def set_size(self, font_size: FontSize) -> 'TextListFormatter':
+        """
+        Set the font size for each Text element.
+        """
+        for text in self._text_list:
+            text.set_size(font_size)
+        return self
+
+    def set_size_xx_small(self) -> 'TextListFormatter':
+        self.set_size('xx-small')
+        return self
+
+    def set_size_x_small(self) -> 'TextListFormatter':
+        self.set_size('x-small')
+        return self
+
+    def set_size_small(self) -> 'TextListFormatter':
+        self.set_size('small')
+        return self
+
+    def set_size_medium(self) -> 'TextListFormatter':
+        self.set_size('medium')
+        return self
+
+    def set_size_large(self) -> 'TextListFormatter':
+        self.set_size('large')
+        return self
+
+    def set_size_x_large(self) -> 'TextListFormatter':
+        self.set_size('x-large')
+        return self
+
+    def set_size_xx_large(self) -> 'TextListFormatter':
+        self.set_size('xx-large')
+        return self
+
+    def set_size_larger(self) -> 'TextListFormatter':
+        self.set_size('larger')
+        return self
+
+    def set_size_smaller(self) -> 'TextListFormatter':
+        self.set_size('smaller')
+        return self
+
+    # endregion
+
+    # region set font family
+
+    def set_font_family(self, font_name: str) -> 'TextListFormatter':
+        """
+        Set the font family to the given font name.
+
+        :param font_name: Name of the font to set.
+        """
+        for text in self._text_list:
+            text.set_font_family(font_name)
+        return self
+
+    def set_font_family_serif(self) -> 'TextListFormatter':
+        """
+        Set the font family to 'serif'
+        """
+        self.set_font_family('serif')
+        return self
+
+    def set_font_family_sans_serif(self) -> 'TextListFormatter':
+        """
+        Set the font family to 'sans-serif'
+        """
+        self.set_font_family('sans-serif')
+        return self
+
+    def set_font_family_cursive(self) -> 'TextListFormatter':
+        """
+        Set the font family to 'cursive'
+        """
+        self.set_font_family('cursive')
+        return self
+
+    def set_font_family_fantasy(self) -> 'TextListFormatter':
+        """
+        Set the font family to 'fantasy'
+        """
+        self.set_font_family('fantasy')
+        return self
+
+    def set_font_family_monospace(self) -> 'TextListFormatter':
+        """
+        Set the font family to 'monospace'
+        """
+        self.set_font_family('monospace')
+        return self
+
+    def set_font_family_benton_sans_f(self) -> 'TextListFormatter':
+        """
+        Set the font family to 'BentonSansF'
+        """
+        self.set_font_family('BentonSansF')
+        return self
+
+    def set_font_family_quarto(self) -> 'TextListFormatter':
+        """
+        Set the font family to 'Quarto'
+        """
+        self.set_font_family('Quarto')
+        return self
+
+    def set_font_family_calibri(self) -> 'TextListFormatter':
+        """
+        Set the font family to 'Calibri'
+        """
+        self.set_font_family('Calibri')
+        return self
+
+    # endregion
+
+    # region set alignment
+
+    def set_ha(self, alignment: H_ALIGN) -> 'TextListFormatter':
+
+        if alignment not in HORIZONTAL_ALIGNMENTS:
+            raise ValueError(
+                f'alignment must be one of {HORIZONTAL_ALIGNMENTS}'
+            )
+        for text in self._text_list:
+            text.set_ha(alignment=alignment)
+        return self
+
+    def set_ha_left(self) -> 'TextListFormatter':
+
+        return self.set_ha('left')
+
+    def set_ha_center(self) -> 'TextListFormatter':
+
+        return self.set_ha('center')
+
+    def set_ha_right(self) -> 'TextListFormatter':
+
+        return self.set_ha('right')
+
+    def set_va(self, alignment: TEXT_V_ALIGN) -> 'TextListFormatter':
+
+        if alignment not in VERTICAL_ALIGNMENTS:
+            raise ValueError(
+                f'alignment must be one of {VERTICAL_ALIGNMENTS}'
+            )
+        for text in self._text_list:
+            text.set_va(alignment=alignment)
+        return self
+
+    def set_va_top(self) -> 'TextListFormatter':
+
+        return self.set_va('top')
+
+    def set_va_center(self) -> 'TextListFormatter':
+
+        return self.set_va('center')
+
+    def set_va_bottom(self) -> 'TextListFormatter':
+
+        return self.set_va('bottom')
+
+    def set_va_baseline(self) -> 'TextListFormatter':
+
+        return self.set_va('baseline')
+
+    def set_va_center_baseline(self) -> 'TextListFormatter':
+
+        return self.set_va('center_baseline')
+
+    # endregion
+
+    @property
+    def texts(self) -> List[str]:
+
+        return[t.to_string() for t in self._text_list]
```

### Comparing `mpl_format-0.317/mpl_format/utils/arg_transforms.py` & `mpl_format-0.318/mpl_format/utils/arg_transforms.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from typing import Sized, Dict, Any, Callable
-
-
-def smart_zip(*args):
-    """
-    Method to convert arguments into a zipped list.
-    Similar to Python's built-in zip method but converts each non-Sized into
-    a list so that it can be iterated over by the user without explicitly
-    checking its type.
-
-    :param args: Each arg should be a single value or a Sized of values. Sized
-                 args which are shorter than the longest Sized will be repeated
-                 len(Sized) times like any non-Sized arg. dicts, strs and tuples
-                 are treated as non-Sizeds as there are contexts in matplotlib
-                 where they are treated as single arguments.
-    """
-    max_arg_length = 1
-    values = []
-    # find longest sized arg
-    for arg in args:
-        if (
-                isinstance(arg, Sized) and
-                not isinstance(arg, dict) and
-                not isinstance(arg, str) and
-                not isinstance(arg, tuple)
-        ):
-            arg_length = len(arg)
-            if arg_length > max_arg_length:
-                max_arg_length = arg_length
-    # create values
-    for arg in args:
-        if (
-                isinstance(arg, Sized) and
-                not isinstance(arg, dict) and
-                not isinstance(arg, str) and
-                not isinstance(arg, tuple) and
-                len(arg) == max_arg_length
-        ):
-            values.append(arg)
-        else:
-            values.append([arg] * max_arg_length)
-    for value_set in zip(*values):
-        yield value_set
-
-
-def smart_zip_kwargs(**kwargs):
-    """
-    Takes kwargs, passes the args into smart_zip and yields dicts mapping kws to
-    zipped arg values.
-
-    :param kwargs: Keys and values. Values passed into smart_zip.
-    :return:
-    """
-    keys = list(kwargs.keys())
-    values = list(kwargs.values())
-    for value_set in smart_zip(*values):
-        out_dict = {
-            key: value for key, value in zip(keys, value_set)
-        }
-        yield out_dict
-
-
-def drop_none_values(items: dict) -> dict:
-    """
-    Return a copy of the dictionary without any keys or values where the value
-    is None.
-    """
-    return {
-        key: value for key, value in items.items()
-        if value is not None
-    }
-
-
-def apply_mappings(items: Dict[str, Any],
-                   mappings: Dict[str, Callable]) -> Dict[str, Any]:
-    """
-    Return a copy of the dictionary with any items with a key in mappings
-    transformed by the callable value associated with that key.
-
-    :param items: dict of items to transform
-    :param mappings: dict of mappings.
-    """
-    return {
-        key: mappings[key](value) if key in mappings.keys() else value
-        for key, value in items.items()
-    }
+from typing import Sized, Dict, Any, Callable
+
+
+def smart_zip(*args):
+    """
+    Method to convert arguments into a zipped list.
+    Similar to Python's built-in zip method but converts each non-Sized into
+    a list so that it can be iterated over by the user without explicitly
+    checking its type.
+
+    :param args: Each arg should be a single value or a Sized of values. Sized
+                 args which are shorter than the longest Sized will be repeated
+                 len(Sized) times like any non-Sized arg. dicts, strs and tuples
+                 are treated as non-Sizeds as there are contexts in matplotlib
+                 where they are treated as single arguments.
+    """
+    max_arg_length = 1
+    values = []
+    # find longest sized arg
+    for arg in args:
+        if (
+                isinstance(arg, Sized) and
+                not isinstance(arg, dict) and
+                not isinstance(arg, str) and
+                not isinstance(arg, tuple)
+        ):
+            arg_length = len(arg)
+            if arg_length > max_arg_length:
+                max_arg_length = arg_length
+    # create values
+    for arg in args:
+        if (
+                isinstance(arg, Sized) and
+                not isinstance(arg, dict) and
+                not isinstance(arg, str) and
+                not isinstance(arg, tuple) and
+                len(arg) == max_arg_length
+        ):
+            values.append(arg)
+        else:
+            values.append([arg] * max_arg_length)
+    for value_set in zip(*values):
+        yield value_set
+
+
+def smart_zip_kwargs(**kwargs):
+    """
+    Takes kwargs, passes the args into smart_zip and yields dicts mapping kws to
+    zipped arg values.
+
+    :param kwargs: Keys and values. Values passed into smart_zip.
+    :return:
+    """
+    keys = list(kwargs.keys())
+    values = list(kwargs.values())
+    for value_set in smart_zip(*values):
+        out_dict = {
+            key: value for key, value in zip(keys, value_set)
+        }
+        yield out_dict
+
+
+def drop_none_values(items: dict) -> dict:
+    """
+    Return a copy of the dictionary without any keys or values where the value
+    is None.
+    """
+    return {
+        key: value for key, value in items.items()
+        if value is not None
+    }
+
+
+def apply_mappings(items: Dict[str, Any],
+                   mappings: Dict[str, Callable]) -> Dict[str, Any]:
+    """
+    Return a copy of the dictionary with any items with a key in mappings
+    transformed by the callable value associated with that key.
+
+    :param items: dict of items to transform
+    :param mappings: dict of mappings.
+    """
+    return {
+        key: mappings[key](value) if key in mappings.keys() else value
+        for key, value in items.items()
+    }
```

### Comparing `mpl_format-0.317/mpl_format/utils/color_utils.py` & `mpl_format-0.318/mpl_format/utils/color_utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from typing import Iterable, Union, List
-
-from mpl_format.compound_types import FloatOrFloatIterable
-from matplotlib.colors import to_rgba
-
-from mpl_format.compound_types import Color
-
-
-def cross_fade(
-        from_color: Color, to_color: Color,
-        amount: FloatOrFloatIterable,
-) -> Union[Color, List[Color]]:
-    """
-    Return a new color which fades amount proportion of the way between the 2
-    colors.
-
-    :param from_color: The color to fade from.
-    :param to_color: The color to fade to.
-    :param amount: The amount to fade by, from 0.0 to 1.0
-    """
-    if isinstance(amount, Iterable):
-        return [
-            cross_fade(from_color, to_color, amt)
-            for amt in amount
-        ]
-    if isinstance(from_color, str):
-        from_color = to_rgba(from_color)
-    if isinstance(to_color, str):
-        to_color = to_rgba(to_color)
-
-    return tuple([from_value + amount * (to_value - from_value)
-                  for from_value, to_value in zip(from_color, to_color)])
-
-
-def blacken(
-        color: Color, amount: FloatOrFloatIterable
-) -> Union[Color, List[Color]]:
-    """
-    Return a color or colors amount fraction or fractions of the way from
-    `color` to `black`.
-
-    :param color: The existing color.
-    :param amount: The proportion to blacken by.
-    """
-    return cross_fade(from_color=color, to_color='black',
-                      amount=amount)
-
-
-def whiten(
-        color: Color, amount: FloatOrFloatIterable
-) -> Union[Color, List[Color]]:
-    """
-    Return a color or colors amount fraction or fractions of the way from
-    `color` to `white`.
-
-    :param color: The existing color.
-    :param amount: The proportion to blacken by.
-    """
-    return cross_fade(from_color=color, to_color='white',
-                      amount=amount)
-
-
-def set_alpha(color: Color, alpha: float) -> Color:
-    """
-    Set the alpha level of a color to a given value.
-
-    :param color: The existing color.
-    :param alpha: The new alpha level
-    """
-    color = to_rgba(color)
-    color = (color[0], color[1], color[2], alpha)
-    return color
+from typing import Iterable, Union, List
+
+from mpl_format.compound_types import FloatOrFloatIterable
+from matplotlib.colors import to_rgba
+
+from mpl_format.compound_types import Color
+
+
+def cross_fade(
+        from_color: Color, to_color: Color,
+        amount: FloatOrFloatIterable,
+) -> Union[Color, List[Color]]:
+    """
+    Return a new color which fades amount proportion of the way between the 2
+    colors.
+
+    :param from_color: The color to fade from.
+    :param to_color: The color to fade to.
+    :param amount: The amount to fade by, from 0.0 to 1.0
+    """
+    if isinstance(amount, Iterable):
+        return [
+            cross_fade(from_color, to_color, amt)
+            for amt in amount
+        ]
+    if isinstance(from_color, str):
+        from_color = to_rgba(from_color)
+    if isinstance(to_color, str):
+        to_color = to_rgba(to_color)
+
+    return tuple([from_value + amount * (to_value - from_value)
+                  for from_value, to_value in zip(from_color, to_color)])
+
+
+def blacken(
+        color: Color, amount: FloatOrFloatIterable
+) -> Union[Color, List[Color]]:
+    """
+    Return a color or colors amount fraction or fractions of the way from
+    `color` to `black`.
+
+    :param color: The existing color.
+    :param amount: The proportion to blacken by.
+    """
+    return cross_fade(from_color=color, to_color='black',
+                      amount=amount)
+
+
+def whiten(
+        color: Color, amount: FloatOrFloatIterable
+) -> Union[Color, List[Color]]:
+    """
+    Return a color or colors amount fraction or fractions of the way from
+    `color` to `white`.
+
+    :param color: The existing color.
+    :param amount: The proportion to blacken by.
+    """
+    return cross_fade(from_color=color, to_color='white',
+                      amount=amount)
+
+
+def set_alpha(color: Color, alpha: float) -> Color:
+    """
+    Set the alpha level of a color to a given value.
+
+    :param color: The existing color.
+    :param alpha: The new alpha level
+    """
+    color = to_rgba(color)
+    color = (color[0], color[1], color[2], alpha)
+    return color
```

### Comparing `mpl_format-0.317/mpl_format/utils/type_checks.py` & `mpl_format-0.318/mpl_format/utils/type_checks.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-def all_are_none(*args) -> bool:
-    """
-    Return True if all args are None.
-    """
-    return all([arg is None for arg in args])
-
-
-def none_are_none(*args) -> bool:
-    """
-    Return True if no args are None.
-    """
-    return not any([arg is None for arg in args])
-
-
-def any_are_not_none(*args) -> bool:
-    """
-    Return True if any arg is not None.
-    """
-    return any([arg is not None for arg in args])
-
-
-def any_are_none(*args) -> bool:
-    """
-    Return True if any arg is None.
-    """
-    return any([arg is None for arg in args])
-
-
-def one_is_none(*args) -> bool:
-    """
-    Return True if exactly one arg is None.
-    """
-    return sum([arg is None for arg in args]) == 1
-
-
-def one_is_not_none(*args) -> bool:
-    """
-    Return True if exactly one arg is not None.
-    """
+def all_are_none(*args) -> bool:
+    """
+    Return True if all args are None.
+    """
+    return all([arg is None for arg in args])
+
+
+def none_are_none(*args) -> bool:
+    """
+    Return True if no args are None.
+    """
+    return not any([arg is None for arg in args])
+
+
+def any_are_not_none(*args) -> bool:
+    """
+    Return True if any arg is not None.
+    """
+    return any([arg is not None for arg in args])
+
+
+def any_are_none(*args) -> bool:
+    """
+    Return True if any arg is None.
+    """
+    return any([arg is None for arg in args])
+
+
+def one_is_none(*args) -> bool:
+    """
+    Return True if exactly one arg is None.
+    """
+    return sum([arg is None for arg in args]) == 1
+
+
+def one_is_not_none(*args) -> bool:
+    """
+    Return True if exactly one arg is not None.
+    """
     return sum([arg is not None for arg in args]) == 1
```

### Comparing `mpl_format-0.317/mpl_format.egg-info/SOURCES.txt` & `mpl_format-0.318/mpl_format.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE.txt
 README.md
 setup.cfg
 setup.py
 mpl_format/__init__.py
 mpl_format/compound_types.py
 mpl_format/literals.py
 mpl_format/settings.py
```

### Comparing `mpl_format-0.317/setup.py` & `mpl_format-0.318/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from distutils.core import setup
-from setuptools import find_packages
-
-setup(
-    name='mpl_format',
-    packages=find_packages(),
-    version='0.317',
-    license='MIT',
-    description='Library for easier formatting of matplotlib plots written in '
-                'a functional style.',
-    author='Vahndi Minah',
-    url='https://github.com/vahndi/mpl-format',
-    keywords=['matplotlib'],
-    install_requires=[
-        'celluloid',
-        'matplotlib',
-        'numpy',
-        'pandas',
-        'seaborn',
-    ],
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3'
-    ],
-)
+from distutils.core import setup
+from setuptools import find_packages
+
+setup(
+    name='mpl_format',
+    packages=find_packages(),
+    version='0.318',
+    license='MIT',
+    description='Library for easier formatting of matplotlib plots written in '
+                'a functional style.',
+    author='Vahndi Minah',
+    url='https://github.com/vahndi/mpl-format',
+    keywords=['matplotlib'],
+    install_requires=[
+        'celluloid',
+        'matplotlib',
+        'numpy',
+        'pandas',
+        'seaborn',
+    ],
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3'
+    ],
+)
```

### Comparing `mpl_format-0.317/tests/test_axis_formatter.py` & `mpl_format-0.318/tests/test_axis_formatter.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-from unittest.case import TestCase
-
-from pandas import Series
-
-from mpl_format.axes import AxesFormatter
-
-
-class TestAxisFormatter(TestCase):
-
-    def setUp(self) -> None:
-
-        self.data = Series({
-            1_000: 3, 2_000: 5, 3_000: 4, 4_000: 6, 5_000: 5
-        })
-        self.data_pct = Series({
-            0.1: 3, 0.2: 5, 0.3: 4, 0.4: 6, 0.5: 5
-        })
-
-    def test_set_format_integer_bar(self):
-
-        axf = AxesFormatter()
-        self.data.plot.bar(ax=axf.axes)
-        axf.x_axis.set_format_integer(categorical=True)
-        axf.show()
-        actual = axf.x_axis.tick_labels.texts
-        expected = ['1,000', '2,000', '3,000', '4,000', '5,000']
-        self.assertListEqual(expected, actual)
-
-    def test_set_format_integer_k_bar(self):
-
-        axf = AxesFormatter()
-        self.data.plot.bar(ax=axf.axes)
-        axf.x_axis.set_format_integer(categorical=True, kmbt=True)
-        axf.show()
-        actual = axf.x_axis.tick_labels.texts
-        expected = ['1K', '2K', '3K', '4K', '5K']
-        self.assertListEqual(expected, actual)
-
-    def test_set_format_integer_line(self):
-
-        axf = AxesFormatter()
-        self.data.plot.line(ax=axf.axes)
-        axf.x_axis.set_format_integer()
-        axf.show()
-        actual = axf.x_axis.tick_labels.texts
-        expected = ['500', '1,000', '1,500', '2,000', '2,500',
-                    '3,000', '3,500', '4,000', '4,500', '5,000', '5,500']
-        self.assertListEqual(expected, actual)
-
-    def test_set_format_integer_k_line(self):
-
-        axf = AxesFormatter()
-        self.data.plot.line(ax=axf.axes)
-        axf.x_axis.set_format_integer(kmbt=True)
-        axf.show()
-        actual = axf.x_axis.tick_labels.texts
-        expected = ['500', '1K', '1.5K', '2K', '2.5K',
-                    '3K', '3.5K', '4K', '4.5K', '5K', '5.5K']
-        self.assertListEqual(expected, actual)
-
-    def test_set_format_currency_bar(self):
-
-        axf = AxesFormatter()
-        self.data.plot.bar(ax=axf.axes)
-        axf.x_axis.set_format_currency(categorical=True)
-        axf.show()
-        actual = axf.x_axis.tick_labels.texts
-        expected = ['$1,000', '$2,000', '$3,000', '$4,000', '$5,000']
-        self.assertListEqual(expected, actual)
-
-    def test_set_format_currency_k_bar(self):
-
-        axf = AxesFormatter()
-        self.data.plot.bar(ax=axf.axes)
-        axf.x_axis.set_format_currency(categorical=True, kmbt=True)
-        axf.show()
-        actual = axf.x_axis.tick_labels.texts
-        expected = ['$1K', '$2K', '$3K', '$4K', '$5K']
-        self.assertListEqual(expected, actual)
-
-    def test_set_format_currency_line(self):
-
-        axf = AxesFormatter()
-        self.data.plot.line(ax=axf.axes)
-        axf.x_axis.set_format_currency()
-        axf.show()
-        actual = axf.x_axis.tick_labels.texts
-        expected = ['$500', '$1,000', '$1,500', '$2,000', '$2,500',
-                    '$3,000', '$3,500', '$4,000', '$4,500', '$5,000', '$5,500']
-        self.assertListEqual(expected, actual)
-
-    def test_set_format_currency_k_line(self):
-
-        axf = AxesFormatter()
-        self.data.plot.line(ax=axf.axes)
-        axf.x_axis.set_format_currency(kmbt=True)
-        axf.show()
-        actual = axf.x_axis.tick_labels.texts
-        expected = ['$500', '$1K', '$1.5K', '$2K', '$2.5K',
-                    '$3K', '$3.5K', '$4K', '$4.5K', '$5K', '$5.5K']
-        self.assertListEqual(expected, actual)
-
-    def test_set_format_percent_bar(self):
-
-        axf = AxesFormatter()
-        self.data_pct.plot.bar(ax=axf.axes)
-        axf.x_axis.set_format_percent(categorical=True)
-        axf.show()
-        actual = axf.x_axis.tick_labels.texts
-        expected = ['10%', '20%', '30%', '40%', '50%']
-        self.assertListEqual(expected, actual)
-
-    def test_set_format_percent_line(self):
-
-        axf = AxesFormatter()
-        self.data_pct.plot.line(ax=axf.axes)
-        axf.x_axis.set_format_percent()
-        axf.show()
-        actual = axf.x_axis.tick_labels.texts
-        expected = ['5%', '10%', '15%', '20%', '25%',
-                    '30%', '35%', '40%', '45%', '50%', '55%']
-        self.assertListEqual(expected, actual)
+from unittest.case import TestCase
+
+from pandas import Series
+
+from mpl_format.axes import AxesFormatter
+
+
+class TestAxisFormatter(TestCase):
+
+    def setUp(self) -> None:
+
+        self.data = Series({
+            1_000: 3, 2_000: 5, 3_000: 4, 4_000: 6, 5_000: 5
+        })
+        self.data_pct = Series({
+            0.1: 3, 0.2: 5, 0.3: 4, 0.4: 6, 0.5: 5
+        })
+
+    def test_set_format_integer_bar(self):
+
+        axf = AxesFormatter()
+        self.data.plot.bar(ax=axf.axes)
+        axf.x_axis.set_format_integer(categorical=True)
+        axf.show()
+        actual = axf.x_axis.tick_labels.texts
+        expected = ['1,000', '2,000', '3,000', '4,000', '5,000']
+        self.assertListEqual(expected, actual)
+
+    def test_set_format_integer_k_bar(self):
+
+        axf = AxesFormatter()
+        self.data.plot.bar(ax=axf.axes)
+        axf.x_axis.set_format_integer(categorical=True, kmbt=True)
+        axf.show()
+        actual = axf.x_axis.tick_labels.texts
+        expected = ['1K', '2K', '3K', '4K', '5K']
+        self.assertListEqual(expected, actual)
+
+    def test_set_format_integer_line(self):
+
+        axf = AxesFormatter()
+        self.data.plot.line(ax=axf.axes)
+        axf.x_axis.set_format_integer()
+        axf.show()
+        actual = axf.x_axis.tick_labels.texts
+        expected = ['500', '1,000', '1,500', '2,000', '2,500',
+                    '3,000', '3,500', '4,000', '4,500', '5,000', '5,500']
+        self.assertListEqual(expected, actual)
+
+    def test_set_format_integer_k_line(self):
+
+        axf = AxesFormatter()
+        self.data.plot.line(ax=axf.axes)
+        axf.x_axis.set_format_integer(kmbt=True)
+        axf.show()
+        actual = axf.x_axis.tick_labels.texts
+        expected = ['500', '1K', '1.5K', '2K', '2.5K',
+                    '3K', '3.5K', '4K', '4.5K', '5K', '5.5K']
+        self.assertListEqual(expected, actual)
+
+    def test_set_format_currency_bar(self):
+
+        axf = AxesFormatter()
+        self.data.plot.bar(ax=axf.axes)
+        axf.x_axis.set_format_currency(categorical=True)
+        axf.show()
+        actual = axf.x_axis.tick_labels.texts
+        expected = ['$1,000', '$2,000', '$3,000', '$4,000', '$5,000']
+        self.assertListEqual(expected, actual)
+
+    def test_set_format_currency_k_bar(self):
+
+        axf = AxesFormatter()
+        self.data.plot.bar(ax=axf.axes)
+        axf.x_axis.set_format_currency(categorical=True, kmbt=True)
+        axf.show()
+        actual = axf.x_axis.tick_labels.texts
+        expected = ['$1K', '$2K', '$3K', '$4K', '$5K']
+        self.assertListEqual(expected, actual)
+
+    def test_set_format_currency_line(self):
+
+        axf = AxesFormatter()
+        self.data.plot.line(ax=axf.axes)
+        axf.x_axis.set_format_currency()
+        axf.show()
+        actual = axf.x_axis.tick_labels.texts
+        expected = ['$500', '$1,000', '$1,500', '$2,000', '$2,500',
+                    '$3,000', '$3,500', '$4,000', '$4,500', '$5,000', '$5,500']
+        self.assertListEqual(expected, actual)
+
+    def test_set_format_currency_k_line(self):
+
+        axf = AxesFormatter()
+        self.data.plot.line(ax=axf.axes)
+        axf.x_axis.set_format_currency(kmbt=True)
+        axf.show()
+        actual = axf.x_axis.tick_labels.texts
+        expected = ['$500', '$1K', '$1.5K', '$2K', '$2.5K',
+                    '$3K', '$3.5K', '$4K', '$4.5K', '$5K', '$5.5K']
+        self.assertListEqual(expected, actual)
+
+    def test_set_format_percent_bar(self):
+
+        axf = AxesFormatter()
+        self.data_pct.plot.bar(ax=axf.axes)
+        axf.x_axis.set_format_percent(categorical=True)
+        axf.show()
+        actual = axf.x_axis.tick_labels.texts
+        expected = ['10%', '20%', '30%', '40%', '50%']
+        self.assertListEqual(expected, actual)
+
+    def test_set_format_percent_line(self):
+
+        axf = AxesFormatter()
+        self.data_pct.plot.line(ax=axf.axes)
+        axf.x_axis.set_format_percent()
+        axf.show()
+        actual = axf.x_axis.tick_labels.texts
+        expected = ['5%', '10%', '15%', '20%', '25%',
+                    '30%', '35%', '40%', '45%', '50%', '55%']
+        self.assertListEqual(expected, actual)
```

### Comparing `mpl_format-0.317/tests/test_text/test_text_utils.py` & `mpl_format-0.318/tests/test_text/test_text_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from matplotlib.text import Text
-from unittest.case import TestCase
-
-from mpl_format.text.text_utils import wrap_text, map_text
-
-
-class TestTextUtils(TestCase):
-
-    def setUp(self) -> None:
-
-        self.a_to_z = 'abcdefghijklmnopqrstuvwxyz'
-        self.digits = '0123456789'
-        self.a_to_z__wrapped_10 = 'abcdefghij\nklmnopqrst\nuvwxyz'
-        self.a_to_z__wrapped_5 = 'abcde\nfghij\nklmno\npqrst\nuvwxy\nz'
-        self.digits__wrapped_5 = '01234\n56789'
-
-    def test_wrap_text__str(self):
-
-        wrapped = wrap_text(text=self.a_to_z, max_width=10)
-        self.assertEqual(self.a_to_z__wrapped_10, wrapped)
-
-    def test_wrap_text__text(self):
-
-        text__a_to_z = Text(text=self.a_to_z)
-        wrapped = wrap_text(text=text__a_to_z, max_width=10)
-        self.assertEqual(self.a_to_z__wrapped_10, wrapped)
-
-    def test_wrap_text__list_str(self):
-
-        expected = [self.a_to_z__wrapped_5, self.digits__wrapped_5]
-        wrapped = wrap_text(text=[self.a_to_z, self.digits], max_width=5)
-        self.assertEqual(expected, wrapped)
-
-    def test_map_text(self):
-
-        mapping = {'a': 'A', 'b': 'B'}
-        self.assertEqual('A', map_text(text='a', mapping=mapping))
-        self.assertEqual('B', map_text(text='b', mapping=mapping))
-        self.assertEqual('c', map_text(text='c', mapping=mapping))
+from matplotlib.text import Text
+from unittest.case import TestCase
+
+from mpl_format.text.text_utils import wrap_text, map_text
+
+
+class TestTextUtils(TestCase):
+
+    def setUp(self) -> None:
+
+        self.a_to_z = 'abcdefghijklmnopqrstuvwxyz'
+        self.digits = '0123456789'
+        self.a_to_z__wrapped_10 = 'abcdefghij\nklmnopqrst\nuvwxyz'
+        self.a_to_z__wrapped_5 = 'abcde\nfghij\nklmno\npqrst\nuvwxy\nz'
+        self.digits__wrapped_5 = '01234\n56789'
+
+    def test_wrap_text__str(self):
+
+        wrapped = wrap_text(text=self.a_to_z, max_width=10)
+        self.assertEqual(self.a_to_z__wrapped_10, wrapped)
+
+    def test_wrap_text__text(self):
+
+        text__a_to_z = Text(text=self.a_to_z)
+        wrapped = wrap_text(text=text__a_to_z, max_width=10)
+        self.assertEqual(self.a_to_z__wrapped_10, wrapped)
+
+    def test_wrap_text__list_str(self):
+
+        expected = [self.a_to_z__wrapped_5, self.digits__wrapped_5]
+        wrapped = wrap_text(text=[self.a_to_z, self.digits], max_width=5)
+        self.assertEqual(expected, wrapped)
+
+    def test_map_text(self):
+
+        mapping = {'a': 'A', 'b': 'B'}
+        self.assertEqual('A', map_text(text='a', mapping=mapping))
+        self.assertEqual('B', map_text(text='b', mapping=mapping))
+        self.assertEqual('c', map_text(text='c', mapping=mapping))
```

