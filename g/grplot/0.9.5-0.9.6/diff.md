# Comparing `tmp/grplot-0.9.5.tar.gz` & `tmp/grplot-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Kuliah\Mandiri\grplot\pypi\grplot\dist\tmp7y0t5vlj\grplot-0.9.5.tar", last modified: Mon Jul  4 13:43:44 2022, max compression
+gzip compressed data, was "C:\Kuliah\Mandiri\grplot\pypi\grplot\dist\tmp0rg9auqg\grplot-0.9.6.tar", last modified: Tue Jul  5 10:55:17 2022, max compression
```

## Comparing `grplot-0.9.5.tar` & `grplot-0.9.6.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:44.098563 grplot-0.9.5/
--rw-rw-rw-   0        0        0     1555 2022-05-13 10:51:24.000000 grplot-0.9.5/LICENSE
--rw-rw-rw-   0        0        0     2532 2022-07-04 13:43:44.087563 grplot-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     1506 2022-05-15 05:16:52.000000 grplot-0.9.5/README.md
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.477089 grplot-0.9.5/grplot/
--rw-rw-rw-   0        0        0    50388 2022-07-04 13:32:09.000000 grplot-0.9.5/grplot/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.594094 grplot-0.9.5/grplot/features/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.286073 grplot-0.9.5/grplot/features/add/
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.650100 grplot-0.9.5/grplot/features/add/label_add/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/label_add/__init__.py
--rw-rw-rw-   0        0        0      717 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/label_add/check_label_add.py
--rw-rw-rw-   0        0        0     1015 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/label_add/label_add_def.py
--rw-rw-rw-   0        0        0      450 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/label_add/label_add_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.720112 grplot-0.9.5/grplot/features/add/log_label_add/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/log_label_add/__init__.py
--rw-rw-rw-   0        0        0      749 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/log_label_add/check_log_label_add.py
--rw-rw-rw-   0        0        0      279 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/log_label_add/log_label_add_def.py
--rw-rw-rw-   0        0        0      474 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/log_label_add/log_label_add_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.767110 grplot-0.9.5/grplot/features/add/statdesc_add/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/statdesc_add/__init__.py
--rw-rw-rw-   0        0        0     1394 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/statdesc_add/statdesc_add_def.py
--rw-rw-rw-   0        0        0      461 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/statdesc_add/statdesc_add_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.812512 grplot-0.9.5/grplot/features/add/text_add/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/text_add/__init__.py
--rw-rw-rw-   0        0        0     1386 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/text_add/text_add_def.py
--rw-rw-rw-   0        0        0      621 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/text_add/text_add_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.871518 grplot-0.9.5/grplot/features/add/tick_add/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/tick_add/__init__.py
--rw-rw-rw-   0        0        0      709 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/tick_add/check_tick_add.py
--rw-rw-rw-   0        0        0     3618 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/tick_add/tick_add_def.py
--rw-rw-rw-   0        0        0      444 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/add/tick_add/tick_add_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.924519 grplot-0.9.5/grplot/features/dt/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/dt/__init__.py
--rw-rw-rw-   0        0        0      644 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/dt/check_dt.py
--rw-rw-rw-   0        0        0      484 2022-06-06 03:30:17.000000 grplot-0.9.5/grplot/features/dt/dt_def.py
--rw-rw-rw-   0        0        0      397 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/dt/dt_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.958529 grplot-0.9.5/grplot/features/font/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/font/__init__.py
--rw-rw-rw-   0        0        0     1061 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/font/check_fontsize.py
--rw-rw-rw-   0        0        0     3408 2022-06-07 05:45:38.000000 grplot-0.9.5/grplot/features/font/font_def.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.984527 grplot-0.9.5/grplot/features/legend/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/legend/__init__.py
--rw-rw-rw-   0        0        0     2174 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/legend/check_legend.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.039760 grplot-0.9.5/grplot/features/lim/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/lim/__init__.py
--rw-rw-rw-   0        0        0      665 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/lim/check_lim.py
--rw-rw-rw-   0        0        0      373 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/lim/lim_def.py
--rw-rw-rw-   0        0        0      411 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/lim/lim_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.102764 grplot-0.9.5/grplot/features/log/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/log/__init__.py
--rw-rw-rw-   0        0        0      665 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/log/check_log.py
--rw-rw-rw-   0        0        0      578 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/log/log_def.py
--rw-rw-rw-   0        0        0      410 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/log/log_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.130771 grplot-0.9.5/grplot/features/pad/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/pad/__init__.py
--rw-rw-rw-   0        0        0      436 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/pad/check_pad.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.237770 grplot-0.9.5/grplot/features/plot/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/plot/__init__.py
--rw-rw-rw-   0        0        0     6521 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/plot/packedbubbles.py
--rw-rw-rw-   0        0        0    19850 2022-05-13 01:25:59.000000 grplot-0.9.5/grplot/features/plot/plot_multi_def.py
--rw-rw-rw-   0        0        0    46691 2022-07-03 13:53:35.000000 grplot-0.9.5/grplot/features/plot/plot_single_def.py
--rw-rw-rw-   0        0        0     6114 2022-05-13 01:20:56.000000 grplot-0.9.5/grplot/features/plot/plot_type.py
--rw-rw-rw-   0        0        0     7820 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/plot/treemaps.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.304774 grplot-0.9.5/grplot/features/rot/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/rot/__init__.py
--rw-rw-rw-   0        0        0      665 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/rot/check_rot.py
--rw-rw-rw-   0        0        0      491 2022-06-04 17:21:07.000000 grplot-0.9.5/grplot/features/rot/rot_def.py
--rw-rw-rw-   0        0        0      419 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/rot/rot_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.354780 grplot-0.9.5/grplot/features/saveas/
--rw-rw-rw-   0        0        0        0 2022-06-04 14:39:33.000000 grplot-0.9.5/grplot/features/saveas/__init__.py
--rw-rw-rw-   0        0        0      181 2022-06-06 08:28:15.000000 grplot-0.9.5/grplot/features/saveas/check_saveas.py
--rw-rw-rw-   0        0        0      178 2022-06-06 08:27:31.000000 grplot-0.9.5/grplot/features/saveas/saveas_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.323075 grplot-0.9.5/grplot/features/sep/
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.416783 grplot-0.9.5/grplot/features/sep/statdesc_sep/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/sep/statdesc_sep/__init__.py
--rw-rw-rw-   0        0        0      695 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/sep/statdesc_sep/statdesc_sep_data_def.py
--rw-rw-rw-   0        0        0     2051 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/sep/statdesc_sep/statdesc_sep_def.py
--rw-rw-rw-   0        0        0      502 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/sep/statdesc_sep/statdesc_sep_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.485792 grplot-0.9.5/grplot/features/sep/text_sep/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/sep/text_sep/__init__.py
--rw-rw-rw-   0        0        0      844 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/sep/text_sep/text_sep_data_def.py
--rw-rw-rw-   0        0        0     3973 2022-05-15 03:25:53.000000 grplot-0.9.5/grplot/features/sep/text_sep/text_sep_def.py
--rw-rw-rw-   0        0        0      925 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/sep/text_sep/text_sep_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.601798 grplot-0.9.5/grplot/features/sep/tick_sep/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/sep/tick_sep/__init__.py
--rw-rw-rw-   0        0        0      741 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/sep/tick_sep/check_tick_sep.py
--rw-rw-rw-   0        0        0     1001 2022-06-07 05:48:40.000000 grplot-0.9.5/grplot/features/sep/tick_sep/tick_sep_data_def.py
--rw-rw-rw-   0        0        0    31817 2022-07-04 13:31:06.000000 grplot-0.9.5/grplot/features/sep/tick_sep/tick_sep_def.py
--rw-rw-rw-   0        0        0      486 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/sep/tick_sep/tick_sep_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.719812 grplot-0.9.5/grplot/features/statdesc/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/statdesc/__init__.py
--rw-rw-rw-   0        0        0     3210 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/statdesc/check_statdesc.py
--rw-rw-rw-   0        0        0    10399 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/statdesc/statdesc_multi_def.py
--rw-rw-rw-   0        0        0      533 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/statdesc/statdesc_plot_def.py
--rw-rw-rw-   0        0        0      564 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/statdesc/statdesc_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.806543 grplot-0.9.5/grplot/features/text/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/text/__init__.py
--rw-rw-rw-   0        0        0     9041 2022-05-13 01:54:59.000000 grplot-0.9.5/grplot/features/text/check_text.py
--rw-rw-rw-   0        0        0    29166 2022-06-07 05:41:52.000000 grplot-0.9.5/grplot/features/text/text_def.py
--rw-rw-rw-   0        0        0      832 2022-05-13 02:05:53.000000 grplot-0.9.5/grplot/features/text/text_type.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.858546 grplot-0.9.5/grplot/features/title/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/title/__init__.py
--rw-rw-rw-   0        0        0      420 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/title/check_title.py
--rw-rw-rw-   0        0        0      323 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/features/title/title_def.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:43.916551 grplot-0.9.5/grplot/hotfix/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/hotfix/__init__.py
--rw-rw-rw-   0        0        0      496 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/hotfix/histplot_legend_fix.py
--rw-rw-rw-   0        0        0     1150 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/hotfix/histplot_percent_add.py
--rw-rw-rw-   0        0        0     8877 2022-05-13 01:52:13.000000 grplot-0.9.5/grplot/setting.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:44.073563 grplot-0.9.5/grplot/utils/
--rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/utils/__init__.py
--rw-rw-rw-   0        0        0     1033 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/utils/arg_ax_type.py
--rw-rw-rw-   0        0        0     2584 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/utils/arg_axis_ax_type.py
--rw-rw-rw-   0        0        0     2499 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/utils/arg_plot_ax_type.py
--rw-rw-rw-   0        0        0      686 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/utils/check_axes.py
--rw-rw-rw-   0        0        0      309 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/utils/check_pandas_index.py
--rw-rw-rw-   0        0        0      333 2022-06-07 05:40:36.000000 grplot-0.9.5/grplot/utils/first_valid_index.py
--rw-rw-rw-   0        0        0      718 2022-05-15 03:22:41.000000 grplot-0.9.5/grplot/utils/scientific_superscript.py
--rw-rw-rw-   0        0        0      282 2022-05-10 13:55:34.000000 grplot-0.9.5/grplot/utils/strtoarray.py
-drwxrwxrwx   0        0        0        0 2022-07-04 13:43:42.579094 grplot-0.9.5/grplot.egg-info/
--rw-rw-rw-   0        0        0     2532 2022-07-04 13:43:42.000000 grplot-0.9.5/grplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3655 2022-07-04 13:43:42.000000 grplot-0.9.5/grplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-04 13:43:42.000000 grplot-0.9.5/grplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2022-07-04 13:43:42.000000 grplot-0.9.5/grplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-07-04 13:43:42.000000 grplot-0.9.5/grplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-05-13 10:51:25.000000 grplot-0.9.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-04 13:43:44.100573 grplot-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0     3046 2022-07-04 13:41:36.000000 grplot-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:17.203967 grplot-0.9.6/
+-rw-rw-rw-   0        0        0     1555 2022-05-13 10:51:24.000000 grplot-0.9.6/LICENSE
+-rw-rw-rw-   0        0        0     2532 2022-07-05 10:55:17.192965 grplot-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1506 2022-05-15 05:16:52.000000 grplot-0.9.6/README.md
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.005349 grplot-0.9.6/grplot/
+-rw-rw-rw-   0        0        0    50388 2022-07-05 08:56:22.000000 grplot-0.9.6/grplot/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.077355 grplot-0.9.6/grplot/features/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:15.893341 grplot-0.9.6/grplot/features/add/
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.120358 grplot-0.9.6/grplot/features/add/label_add/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/label_add/__init__.py
+-rw-rw-rw-   0        0        0      717 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/label_add/check_label_add.py
+-rw-rw-rw-   0        0        0     1015 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/label_add/label_add_def.py
+-rw-rw-rw-   0        0        0      450 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/label_add/label_add_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.167363 grplot-0.9.6/grplot/features/add/log_label_add/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/log_label_add/__init__.py
+-rw-rw-rw-   0        0        0      749 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/log_label_add/check_log_label_add.py
+-rw-rw-rw-   0        0        0      279 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/log_label_add/log_label_add_def.py
+-rw-rw-rw-   0        0        0      474 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/log_label_add/log_label_add_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.202367 grplot-0.9.6/grplot/features/add/statdesc_add/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/statdesc_add/__init__.py
+-rw-rw-rw-   0        0        0     1394 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/statdesc_add/statdesc_add_def.py
+-rw-rw-rw-   0        0        0      461 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/statdesc_add/statdesc_add_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.238368 grplot-0.9.6/grplot/features/add/text_add/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/text_add/__init__.py
+-rw-rw-rw-   0        0        0     1386 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/text_add/text_add_def.py
+-rw-rw-rw-   0        0        0      621 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/text_add/text_add_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.293880 grplot-0.9.6/grplot/features/add/tick_add/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/tick_add/__init__.py
+-rw-rw-rw-   0        0        0      709 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/tick_add/check_tick_add.py
+-rw-rw-rw-   0        0        0     3618 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/tick_add/tick_add_def.py
+-rw-rw-rw-   0        0        0      444 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/add/tick_add/tick_add_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.346884 grplot-0.9.6/grplot/features/dt/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/dt/__init__.py
+-rw-rw-rw-   0        0        0      644 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/dt/check_dt.py
+-rw-rw-rw-   0        0        0      484 2022-06-06 03:30:17.000000 grplot-0.9.6/grplot/features/dt/dt_def.py
+-rw-rw-rw-   0        0        0      397 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/dt/dt_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.383892 grplot-0.9.6/grplot/features/font/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/font/__init__.py
+-rw-rw-rw-   0        0        0     1061 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/font/check_fontsize.py
+-rw-rw-rw-   0        0        0     3408 2022-06-07 05:45:38.000000 grplot-0.9.6/grplot/features/font/font_def.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.409890 grplot-0.9.6/grplot/features/legend/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/legend/__init__.py
+-rw-rw-rw-   0        0        0     2174 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/legend/check_legend.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.462893 grplot-0.9.6/grplot/features/lim/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/lim/__init__.py
+-rw-rw-rw-   0        0        0      665 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/lim/check_lim.py
+-rw-rw-rw-   0        0        0      373 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/lim/lim_def.py
+-rw-rw-rw-   0        0        0      411 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/lim/lim_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.513898 grplot-0.9.6/grplot/features/log/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/log/__init__.py
+-rw-rw-rw-   0        0        0      665 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/log/check_log.py
+-rw-rw-rw-   0        0        0      578 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/log/log_def.py
+-rw-rw-rw-   0        0        0      410 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/log/log_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.538902 grplot-0.9.6/grplot/features/pad/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/pad/__init__.py
+-rw-rw-rw-   0        0        0      436 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/pad/check_pad.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.626037 grplot-0.9.6/grplot/features/plot/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/plot/__init__.py
+-rw-rw-rw-   0        0        0     6521 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/plot/packedbubbles.py
+-rw-rw-rw-   0        0        0    19850 2022-05-13 01:25:59.000000 grplot-0.9.6/grplot/features/plot/plot_multi_def.py
+-rw-rw-rw-   0        0        0    46691 2022-07-03 13:53:35.000000 grplot-0.9.6/grplot/features/plot/plot_single_def.py
+-rw-rw-rw-   0        0        0     6114 2022-05-13 01:20:56.000000 grplot-0.9.6/grplot/features/plot/plot_type.py
+-rw-rw-rw-   0        0        0     7820 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/plot/treemaps.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.678044 grplot-0.9.6/grplot/features/rot/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/rot/__init__.py
+-rw-rw-rw-   0        0        0      665 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/rot/check_rot.py
+-rw-rw-rw-   0        0        0      491 2022-06-04 17:21:07.000000 grplot-0.9.6/grplot/features/rot/rot_def.py
+-rw-rw-rw-   0        0        0      419 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/rot/rot_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.714045 grplot-0.9.6/grplot/features/saveas/
+-rw-rw-rw-   0        0        0        0 2022-06-04 14:39:33.000000 grplot-0.9.6/grplot/features/saveas/__init__.py
+-rw-rw-rw-   0        0        0      181 2022-06-06 08:28:15.000000 grplot-0.9.6/grplot/features/saveas/check_saveas.py
+-rw-rw-rw-   0        0        0      178 2022-06-06 08:27:31.000000 grplot-0.9.6/grplot/features/saveas/saveas_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:15.913343 grplot-0.9.6/grplot/features/sep/
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.771053 grplot-0.9.6/grplot/features/sep/statdesc_sep/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/sep/statdesc_sep/__init__.py
+-rw-rw-rw-   0        0        0      713 2022-07-05 08:55:08.000000 grplot-0.9.6/grplot/features/sep/statdesc_sep/statdesc_sep_data_def.py
+-rw-rw-rw-   0        0        0     2051 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/sep/statdesc_sep/statdesc_sep_def.py
+-rw-rw-rw-   0        0        0      502 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/sep/statdesc_sep/statdesc_sep_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.817052 grplot-0.9.6/grplot/features/sep/text_sep/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/sep/text_sep/__init__.py
+-rw-rw-rw-   0        0        0      844 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/sep/text_sep/text_sep_data_def.py
+-rw-rw-rw-   0        0        0     3973 2022-05-15 03:25:53.000000 grplot-0.9.6/grplot/features/sep/text_sep/text_sep_def.py
+-rw-rw-rw-   0        0        0      925 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/sep/text_sep/text_sep_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.884058 grplot-0.9.6/grplot/features/sep/tick_sep/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/sep/tick_sep/__init__.py
+-rw-rw-rw-   0        0        0      741 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/sep/tick_sep/check_tick_sep.py
+-rw-rw-rw-   0        0        0     1001 2022-06-07 05:48:40.000000 grplot-0.9.6/grplot/features/sep/tick_sep/tick_sep_data_def.py
+-rw-rw-rw-   0        0        0    31817 2022-07-04 13:31:06.000000 grplot-0.9.6/grplot/features/sep/tick_sep/tick_sep_def.py
+-rw-rw-rw-   0        0        0      486 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/sep/tick_sep/tick_sep_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.951064 grplot-0.9.6/grplot/features/statdesc/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/statdesc/__init__.py
+-rw-rw-rw-   0        0        0     3210 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/statdesc/check_statdesc.py
+-rw-rw-rw-   0        0        0    11566 2022-07-05 08:52:19.000000 grplot-0.9.6/grplot/features/statdesc/statdesc_multi_def.py
+-rw-rw-rw-   0        0        0      533 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/statdesc/statdesc_plot_def.py
+-rw-rw-rw-   0        0        0      564 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/statdesc/statdesc_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:17.009068 grplot-0.9.6/grplot/features/text/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/text/__init__.py
+-rw-rw-rw-   0        0        0     9041 2022-05-13 01:54:59.000000 grplot-0.9.6/grplot/features/text/check_text.py
+-rw-rw-rw-   0        0        0    29364 2022-07-05 10:52:59.000000 grplot-0.9.6/grplot/features/text/text_def.py
+-rw-rw-rw-   0        0        0      832 2022-05-13 02:05:53.000000 grplot-0.9.6/grplot/features/text/text_type.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:17.043068 grplot-0.9.6/grplot/features/title/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/title/__init__.py
+-rw-rw-rw-   0        0        0      420 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/title/check_title.py
+-rw-rw-rw-   0        0        0      323 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/features/title/title_def.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:17.075400 grplot-0.9.6/grplot/hotfix/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/hotfix/__init__.py
+-rw-rw-rw-   0        0        0      496 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/hotfix/histplot_legend_fix.py
+-rw-rw-rw-   0        0        0     1150 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/hotfix/histplot_percent_add.py
+-rw-rw-rw-   0        0        0     8877 2022-05-13 01:52:13.000000 grplot-0.9.6/grplot/setting.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:17.179962 grplot-0.9.6/grplot/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/utils/__init__.py
+-rw-rw-rw-   0        0        0     1033 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/utils/arg_ax_type.py
+-rw-rw-rw-   0        0        0     2584 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/utils/arg_axis_ax_type.py
+-rw-rw-rw-   0        0        0     2499 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/utils/arg_plot_ax_type.py
+-rw-rw-rw-   0        0        0      686 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/utils/check_axes.py
+-rw-rw-rw-   0        0        0      309 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/utils/check_pandas_index.py
+-rw-rw-rw-   0        0        0      333 2022-06-07 05:40:36.000000 grplot-0.9.6/grplot/utils/first_valid_index.py
+-rw-rw-rw-   0        0        0      718 2022-05-15 03:22:41.000000 grplot-0.9.6/grplot/utils/scientific_superscript.py
+-rw-rw-rw-   0        0        0      282 2022-05-10 13:55:34.000000 grplot-0.9.6/grplot/utils/strtoarray.py
+drwxrwxrwx   0        0        0        0 2022-07-05 10:55:16.069354 grplot-0.9.6/grplot.egg-info/
+-rw-rw-rw-   0        0        0     2532 2022-07-05 10:55:15.000000 grplot-0.9.6/grplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3655 2022-07-05 10:55:15.000000 grplot-0.9.6/grplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-05 10:55:15.000000 grplot-0.9.6/grplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2022-07-05 10:55:15.000000 grplot-0.9.6/grplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-07-05 10:55:15.000000 grplot-0.9.6/grplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-05-13 10:51:25.000000 grplot-0.9.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-07-05 10:55:17.204966 grplot-0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     3046 2022-07-05 08:56:41.000000 grplot-0.9.6/setup.py
```

### Comparing `grplot-0.9.5/LICENSE` & `grplot-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/PKG-INFO` & `grplot-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grplot
-Version: 0.9.5
+Version: 0.9.6
 Summary: grplot: lazy statistical data visualization
 Home-page: https://github.com/ghiffaryr/grplot
 Download-URL: https://github.com/ghiffaryr/grplot
 Author: Ghiffary Rifqialdi
 Author-email: grifqialdi@gmail.com
 Maintainer: Ghiffary Rifqialdi
 Maintainer-email: grifqialdi@gmail.com
```

### Comparing `grplot-0.9.5/README.md` & `grplot-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/__init__.py` & `grplot-0.9.6/grplot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,18 +189,18 @@
     '''
     -----------------------------------------------
     grplot: lazy statistical data visualization
     
     by ghiffary rifqialdi
     based on numpy, scipy, matplotlib, seaborn, squarify, and pandas
     
-    version = '0.9.5'
+    version = '0.9.6'
 
     release date
-    04/07/2022
+    05/07/2022
     -----------------------------------------------
 
     documentation is available at https://github.com/ghiffaryr/grplot
     '''    
     # initialization
     # creating figure
     Nx, Ny = check_axes(x, y, Nx, Ny)
```

### Comparing `grplot-0.9.5/grplot/features/add/label_add/check_label_add.py` & `grplot-0.9.6/grplot/features/add/label_add/check_label_add.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/add/label_add/label_add_def.py` & `grplot-0.9.6/grplot/features/add/label_add/label_add_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/add/log_label_add/check_log_label_add.py` & `grplot-0.9.6/grplot/features/add/log_label_add/check_log_label_add.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/add/statdesc_add/statdesc_add_def.py` & `grplot-0.9.6/grplot/features/add/statdesc_add/statdesc_add_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/add/text_add/text_add_def.py` & `grplot-0.9.6/grplot/features/add/text_add/text_add_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/add/text_add/text_add_type.py` & `grplot-0.9.6/grplot/features/add/text_add/text_add_type.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/add/tick_add/check_tick_add.py` & `grplot-0.9.6/grplot/features/add/tick_add/check_tick_add.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/add/tick_add/tick_add_def.py` & `grplot-0.9.6/grplot/features/add/tick_add/tick_add_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/dt/check_dt.py` & `grplot-0.9.6/grplot/features/dt/check_dt.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/font/check_fontsize.py` & `grplot-0.9.6/grplot/features/font/check_fontsize.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/font/font_def.py` & `grplot-0.9.6/grplot/features/font/font_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/legend/check_legend.py` & `grplot-0.9.6/grplot/features/legend/check_legend.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/lim/check_lim.py` & `grplot-0.9.6/grplot/features/lim/check_lim.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/log/check_log.py` & `grplot-0.9.6/grplot/features/log/check_log.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/log/log_def.py` & `grplot-0.9.6/grplot/features/log/log_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/plot/packedbubbles.py` & `grplot-0.9.6/grplot/features/plot/packedbubbles.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/plot/plot_multi_def.py` & `grplot-0.9.6/grplot/features/plot/plot_multi_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/plot/plot_single_def.py` & `grplot-0.9.6/grplot/features/plot/plot_single_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/plot/plot_type.py` & `grplot-0.9.6/grplot/features/plot/plot_type.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/plot/treemaps.py` & `grplot-0.9.6/grplot/features/plot/treemaps.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/rot/check_rot.py` & `grplot-0.9.6/grplot/features/rot/check_rot.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/sep/statdesc_sep/statdesc_sep_data_def.py` & `grplot-0.9.6/grplot/features/sep/statdesc_sep/statdesc_sep_data_def.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pandas.api.types import is_numeric_dtype
 from grplot.features.sep.statdesc_sep.statdesc_sep_def import statdesc_sep_def
 
 
 def statdesc_sep_data_def(num, stat_label, sep):
     if is_numeric_dtype(type(num)) == True:
-        if stat_label in ['count', 'unique count']:
+        if stat_label in ['count', 'non zero count', 'unique count']:
             if sep in [',c', ',cL']:
                 num = statdesc_sep_def(num=num, sep=',')
             elif sep in ['.c', '.cL']:
                 num = statdesc_sep_def(num=num, sep='.')
             else:
                 num = statdesc_sep_def(num=num, sep=sep)
         else:
```

### Comparing `grplot-0.9.5/grplot/features/sep/statdesc_sep/statdesc_sep_def.py` & `grplot-0.9.6/grplot/features/sep/statdesc_sep/statdesc_sep_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/sep/text_sep/text_sep_data_def.py` & `grplot-0.9.6/grplot/features/sep/text_sep/text_sep_data_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/sep/text_sep/text_sep_def.py` & `grplot-0.9.6/grplot/features/sep/text_sep/text_sep_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/sep/text_sep/text_sep_type.py` & `grplot-0.9.6/grplot/features/sep/text_sep/text_sep_type.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/sep/tick_sep/check_tick_sep.py` & `grplot-0.9.6/grplot/features/sep/tick_sep/check_tick_sep.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/sep/tick_sep/tick_sep_data_def.py` & `grplot-0.9.6/grplot/features/sep/tick_sep/tick_sep_data_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/sep/tick_sep/tick_sep_def.py` & `grplot-0.9.6/grplot/features/sep/tick_sep/tick_sep_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/statdesc/check_statdesc.py` & `grplot-0.9.6/grplot/features/statdesc/check_statdesc.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/statdesc/statdesc_multi_def.py` & `grplot-0.9.6/grplot/features/statdesc/statdesc_multi_def.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,154 +11,169 @@
         data = numpy.array(df[axislabel])
     elif numpy.issubdtype(type(df[axislabel]), numpy.ndarray) == True:
         data = df[axislabel]
     else:
         raise Exception('Unsupported dtype')
     # drop numpy.nan
     try:
-        data = data[~numpy.isnan(data)]
+        data_notnan = data[~numpy.isnan(data)]
     except:
-        data = numpy.array([value for value in data if str(value) != 'nan'])
+        data_notnan = numpy.array([value for value in data if str(value) != 'nan'])
     if type(statdesc) == str:
         if 'general' in statdesc:
-            statdesc = statdesc.replace('general', 'count+unique+std+min+q1+median+mean+q3+max')
+            statdesc = statdesc.replace('general', 'count+nonzero+unique+std+range+min+q1+median+mean+q3+max')
         elif 'boxplot' in statdesc:
             statdesc = statdesc.replace('boxplot', 'min+whislo+q1+cilo+median+mean+cihi+q3+whishi+max')
         else:
             pass
         for stat in statdesc.split('+'):
             if 'count' in stat:
                 try:
-                    count = numpy.count_nonzero(data)
+                    count = data_notnan.size
                     count_sep = statdesc_sep_type(num=count, stat_label='count', sep=sep, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=count, color=None, stat_label='count', stat_fmt=count_sep)
+            elif 'nonzero' in stat:
+                try:
+                    nonzero = numpy.count_nonzero(data_notnan)
+                    nonzero_sep = statdesc_sep_type(num=nonzero, stat_label='non zero count', sep=sep, axislabel=axislabel, axes=axes)
+                except:
+                    raise Exception('Label not in the dataframe!')
+                statdesc_plot_def(ax=ax, axis=axis, stat=nonzero, color=None, stat_label='non zero count', stat_fmt=nonzero_sep)
             elif 'unique' in stat:
                 try:
-                    unique = len(numpy.unique(data))
+                    unique = len(numpy.unique(data_notnan))
                     unique_sep = statdesc_sep_type(num=unique, stat_label='unique count', sep=sep, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=unique, color=None, stat_label='unique count', stat_fmt=unique_sep)
             elif 'std' in stat:
                 try:
-                    std = numpy.std(data)
+                    std = numpy.std(data_notnan, ddof=1)
                     std_sep = statdesc_sep_type(num=std, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     std_add = statdesc_add_type(num=std_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=std, color=None, stat_label='std', stat_fmt=std_add)
+            elif 'range' in stat:
+                try:
+                    range = numpy.ptp(data_notnan)
+                    range_sep = statdesc_sep_type(num=range, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
+                    range_add = statdesc_add_type(num=range_sep, add=add, axislabel=axislabel, axes=axes)
+                except:
+                    raise Exception('Label not in the dataframe!')
+                statdesc_plot_def(ax=ax, axis=axis, stat=range, color=None, stat_label='range', stat_fmt=range_add)
             elif 'min' in stat:
                 try:
-                    mini = numpy.min(data)
+                    mini = numpy.min(data_notnan)
                     mini_sep = statdesc_sep_type(num=mini, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     mini_add = statdesc_add_type(num=mini_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=mini, color='red', stat_label='min', stat_fmt=mini_add)
             elif 'pct1' in stat:
                 try:
-                    pct1 = numpy.percentile(data, 1)
+                    pct1 = numpy.percentile(data_notnan, 1)
                     pct1_sep = statdesc_sep_type(num=pct1, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     pct1_add = statdesc_add_type(num=pct1_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=pct1, color='orange', stat_label='1st pct', stat_fmt=pct1_add)
             elif 'whislo' in stat:
                 try:
-                    whislo = cbook.boxplot_stats(data)[0]['whislo']
+                    whislo = cbook.boxplot_stats(data_notnan)[0]['whislo']
                     whislo_sep = statdesc_sep_type(num=whislo, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     whislo_add = statdesc_add_type(num=whislo_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=whislo, color='orange', stat_label='lower whisker', stat_fmt=whislo_add)
             elif 'pct5' in stat:
                 try:
-                    pct5 = numpy.percentile(data, 5)
+                    pct5 = numpy.percentile(data_notnan, 5)
                     pct5_sep = statdesc_sep_type(num=pct5, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     pct5_add = statdesc_add_type(num=pct5_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=pct5, color='green', stat_label='5th pct', stat_fmt=pct5_add)
             elif 'q1' in stat:
                 try:
-                    q1 = numpy.percentile(data, 25)
+                    q1 = numpy.percentile(data_notnan, 25)
                     q1_sep = statdesc_sep_type(num=q1, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     q1_add = statdesc_add_type(num=q1_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=q1, color='gold', stat_label='q1', stat_fmt=q1_add)
             elif 'cilo' in stat:
                 try:
-                    cilo = cbook.boxplot_stats(data)[0]['cilo']
+                    cilo = cbook.boxplot_stats(data_notnan)[0]['cilo']
                     cilo_sep = statdesc_sep_type(num=cilo, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     cilo_add = statdesc_add_type(num=cilo_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=cilo, color='green', stat_label='95% CI low', stat_fmt=cilo_add)
             elif 'median' in stat:
                 try:
-                    median = numpy.median(data)
+                    median = numpy.median(data_notnan)
                     median_sep = statdesc_sep_type(num=median, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     median_add = statdesc_add_type(num=median_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=median, color='blue', stat_label='median', stat_fmt=median_add)
             elif 'mean' in stat:
                 try:
-                    mean = numpy.mean(data)
+                    mean = numpy.mean(data_notnan)
                     mean_sep = statdesc_sep_type(num=mean, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     mean_add = statdesc_add_type(num=mean_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=mean, color='blue', stat_label='mean', stat_fmt=mean_add)
             elif 'cihi' in stat:
                 try:
-                    cihi = cbook.boxplot_stats(data)[0]['cihi']
+                    cihi = cbook.boxplot_stats(data_notnan)[0]['cihi']
                     cihi_sep = statdesc_sep_type(num=cihi, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     cihi_add = statdesc_add_type(num=cihi_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=cihi, color='green', stat_label='95% CI hi', stat_fmt=cihi_add)
             elif 'q3' in stat:
                 try:
-                    q3 = numpy.percentile(data, 75)
+                    q3 = numpy.percentile(data_notnan, 75)
                     q3_sep = statdesc_sep_type(num=q3, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     q3_add = statdesc_add_type(num=q3_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=q3, color='gold', stat_label='q3', stat_fmt=q3_add)
             elif 'pct95' in stat:
                 try:
-                    pct95 = numpy.percentile(data, 95)
+                    pct95 = numpy.percentile(data_notnan, 95)
                     pct95_sep = statdesc_sep_type(num=pct95, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     pct95_add = statdesc_add_type(num=pct95_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=pct95, color='green', stat_label='95th pct', stat_fmt=pct95_add)
             elif 'whishi' in stat:
                 try:
-                    whishi = cbook.boxplot_stats(data)[0]['whishi']
+                    whishi = cbook.boxplot_stats(data_notnan)[0]['whishi']
                     whishi_sep = statdesc_sep_type(num=whishi, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     whishi_add = statdesc_add_type(num=whishi_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=whishi, color='orange', stat_label='upper whisker', stat_fmt=whishi_add)
             elif 'pct99' in stat:
                 try:
-                    pct99 = numpy.percentile(data, 99)
+                    pct99 = numpy.percentile(data_notnan, 99)
                     pct99_sep = statdesc_sep_type(num=pct99, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     pct99_add = statdesc_add_type(num=pct99_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=pct99, color='orange', stat_label='99th pct', stat_fmt=pct99_add)
             elif 'max' in stat:
                 try:
-                    maxi = numpy.max(data)
+                    maxi = numpy.max(data_notnan)
                     maxi_sep = statdesc_sep_type(num=maxi, stat_label=None, sep=sep, axislabel=axislabel, axes=axes)
                     maxi_add = statdesc_add_type(num=maxi_sep, add=add, axislabel=axislabel, axes=axes)
                 except:
                     raise Exception('Label not in the dataframe!')
                 statdesc_plot_def(ax=ax, axis=axis, stat=maxi, color='red', stat_label='max', stat_fmt=maxi_add)
             else:
                 pass
```

### Comparing `grplot-0.9.5/grplot/features/statdesc/statdesc_plot_def.py` & `grplot-0.9.6/grplot/features/statdesc/statdesc_plot_def.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/statdesc/statdesc_type.py` & `grplot-0.9.6/grplot/features/statdesc/statdesc_type.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/text/check_text.py` & `grplot-0.9.6/grplot/features/text/check_text.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/features/text/text_def.py` & `grplot-0.9.6/grplot/features/text/text_def.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,65 +309,70 @@
                         pass
             else:
                 raise Exception('Unsupported axis!')
         else:
             pass
     else:
         pass
-    if (plot == 'scatterplot') and (text == True):
+    if (plot in ['scatterplot', 'residplot']) and (text == True):
         x_arr, y_arr = numpy.array([x for x, _ in ax.collections[0].get_offsets()]), numpy.array([y for _, y in ax.collections[0].get_offsets()])
         # get max and min y data points
         if y_arr.size != 0:
             max_y = max(y_arr)
             min_y = min(y_arr)
         else:
             pass
+        # position calibrator
+        if plot == 'residplot':
+            weight = 5
+        else:
+            weight = 1
         if (x_arr.size != 0) and (y_arr.size != 0):
             for x, y in ax.collections[0].get_offsets():
                 # annotate
                 if axis == 'x':
                     x_sep = text_sep_type(plot=plot, df=df, num=x, sep=sep, axislabel=axislabel, axes=axes)
                     x_add = text_add_type(plot=plot, num=x_sep, add=add, axislabel=axislabel, axes=axes)
                     if y > 0:
                         if text_fontsize is not None:
                             try:
-                                ax.annotate(f'{x_add}', xy=(x, y-max_y*0.0325*text_fontsize/10), fontsize=text_fontsize, ha='center', va='center')
+                                ax.annotate(f'{x_add}', xy=(x, y-max_y*0.0325*weight*text_fontsize/10), fontsize=text_fontsize, ha='center', va='center')
                             except:
                                 raise Exception('Unknown text fontsize argument!')
                         else:
-                            ax.annotate(f'{x_add}', xy=(x, y-max_y*0.0325), ha='center', va='center')
+                            ax.annotate(f'{x_add}', xy=(x, y-max_y*0.0325*weight), ha='center', va='center')
                     elif y < 0:
                         if text_fontsize is not None:
                             try:
-                                ax.annotate(f'{x_add}', xy=(x, y+min_y*0.0325*text_fontsize/10), fontsize=text_fontsize, ha='center', va='center')
+                                ax.annotate(f'{x_add}', xy=(x, y+min_y*0.0325*weight*text_fontsize/10), fontsize=text_fontsize, ha='center', va='center')
                             except:
                                 raise Exception('Unknown text fontsize argument!')
                         else:
-                            ax.annotate(f'{x_add}', xy=(x, y+min_y*0.0325), ha='center', va='center')
+                            ax.annotate(f'{x_add}', xy=(x, y+min_y*0.0325*weight), ha='center', va='center')
                     else:
                         pass
                 elif axis == 'y':
                     y_sep = text_sep_type(plot=plot, df=df, num=y, sep=sep, axislabel=axislabel, axes=axes)
                     y_add = text_add_type(plot=plot, num=y_sep, add=add, axislabel=axislabel, axes=axes)
                     if y > 0:
                         if text_fontsize is not None:
                             try:
-                                ax.annotate(f'{y_add}', xy=(x, y+max_y*0.03*text_fontsize/10), fontsize=text_fontsize, ha='center', va='center')
+                                ax.annotate(f'{y_add}', xy=(x, y+max_y*0.03*weight*text_fontsize/10), fontsize=text_fontsize, ha='center', va='center')
                             except:
                                 raise Exception('Unknown text fontsize argument!')
                         else:
-                            ax.annotate(f'{y_add}', xy=(x, y+max_y*0.03), ha='center', va='center')
+                            ax.annotate(f'{y_add}', xy=(x, y+max_y*0.03*weight), ha='center', va='center')
                     elif y < 0:
                         if text_fontsize is not None:
                             try:
-                                ax.annotate(f'{y_add}', xy=(x, y-min_y*0.03*text_fontsize/10), fontsize=text_fontsize, ha='center', va='center')
+                                ax.annotate(f'{y_add}', xy=(x, y-min_y*0.03*weight*text_fontsize/10), fontsize=text_fontsize, ha='center', va='center')
                             except:
                                 raise Exception('Unknown text fontsize argument!')
                         else:
-                            ax.annotate(f'{y_add}', xy=(x, y-min_y*0.03), ha='center', va='center')
+                            ax.annotate(f'{y_add}', xy=(x, y-min_y*0.03*weight), ha='center', va='center')
                     else:
                         pass
                 else:
                     raise Exception('Unsupported axis!')
         else:
             pass
     else:
```

### Comparing `grplot-0.9.5/grplot/features/text/text_type.py` & `grplot-0.9.6/grplot/features/text/text_type.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/hotfix/histplot_percent_add.py` & `grplot-0.9.6/grplot/hotfix/histplot_percent_add.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/setting.py` & `grplot-0.9.6/grplot/setting.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/utils/arg_ax_type.py` & `grplot-0.9.6/grplot/utils/arg_ax_type.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/utils/arg_axis_ax_type.py` & `grplot-0.9.6/grplot/utils/arg_axis_ax_type.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/utils/arg_plot_ax_type.py` & `grplot-0.9.6/grplot/utils/arg_plot_ax_type.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/utils/check_axes.py` & `grplot-0.9.6/grplot/utils/check_axes.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot/utils/scientific_superscript.py` & `grplot-0.9.6/grplot/utils/scientific_superscript.py`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/grplot.egg-info/PKG-INFO` & `grplot-0.9.6/grplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grplot
-Version: 0.9.5
+Version: 0.9.6
 Summary: grplot: lazy statistical data visualization
 Home-page: https://github.com/ghiffaryr/grplot
 Download-URL: https://github.com/ghiffaryr/grplot
 Author: Ghiffary Rifqialdi
 Author-email: grifqialdi@gmail.com
 Maintainer: Ghiffary Rifqialdi
 Maintainer-email: grifqialdi@gmail.com
```

### Comparing `grplot-0.9.5/grplot.egg-info/SOURCES.txt` & `grplot-0.9.6/grplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grplot-0.9.5/setup.py` & `grplot-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 DISTNAME = "grplot"
-VERSION = "0.9.5"
+VERSION = "0.9.6"
 MAINTAINER = "Ghiffary Rifqialdi"
 MAINTAINER_EMAIL = "grifqialdi@gmail.com"
 DESCRIPTION = "grplot: lazy statistical data visualization"
 LICENSE = "BSD (3-clause)"
 URL = "https://github.com/ghiffaryr/grplot"
 PROJECT_URLS = {
                 "Bug Tracker": "https://github.com/ghiffaryr/grplot/issues"
```

