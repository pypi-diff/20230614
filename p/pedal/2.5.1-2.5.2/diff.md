# Comparing `tmp/pedal-2.5.1.tar.gz` & `tmp/pedal-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedal-2.5.1.tar", last modified: Sun Jun 11 14:14:30 2023, max compression
+gzip compressed data, was "pedal-2.5.2.tar", last modified: Wed Jun 14 16:24:51 2023, max compression
```

## Comparing `pedal-2.5.1.tar` & `pedal-2.5.2.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.832032 pedal-2.5.1/
--rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.5.1/LICENSE
--rw-rw-rw-   0        0        0     2564 2023-06-11 14:14:30.832032 pedal-2.5.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.662032 pedal-2.5.1/Pedal.egg-info/
--rw-rw-rw-   0        0        0     2564 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3759 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1958 2023-05-18 18:40:27.000000 pedal-2.5.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.660032 pedal-2.5.1/pedal/
--rw-rw-rw-   0        0        0      382 2023-05-18 18:14:23.000000 pedal-2.5.1/pedal/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.679032 pedal-2.5.1/pedal/assertions/
--rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/assertions/__init__.py
--rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.5.1/pedal/assertions/classes.py
--rw-rw-rw-   0        0        0    13288 2023-01-17 17:53:58.000000 pedal-2.5.1/pedal/assertions/commands.py
--rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/assertions/constants.py
--rw-rw-rw-   0        0        0    20355 2023-05-27 15:44:30.000000 pedal-2.5.1/pedal/assertions/feedbacks.py
--rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.5.1/pedal/assertions/functions.py
--rw-rw-rw-   0        0        0     5722 2021-01-26 15:12:38.000000 pedal-2.5.1/pedal/assertions/organizers.py
--rw-rw-rw-   0        0        0    33752 2023-05-22 19:35:19.000000 pedal-2.5.1/pedal/assertions/runtime.py
--rw-rw-rw-   0        0        0     3254 2023-05-26 21:11:25.000000 pedal-2.5.1/pedal/assertions/setup.py
--rw-rw-rw-   0        0        0    30229 2023-05-26 20:52:09.000000 pedal-2.5.1/pedal/assertions/static.py
--rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/assertions/unittest.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.689033 pedal-2.5.1/pedal/cait/
--rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.5.1/pedal/cait/__init__.py
--rw-rw-rw-   0        0        0     2255 2023-05-27 15:47:12.000000 pedal-2.5.1/pedal/cait/ast_helpers.py
--rw-rw-rw-   0        0        0    11371 2021-03-12 21:12:46.000000 pedal-2.5.1/pedal/cait/ast_map.py
--rw-rw-rw-   0        0        0    10523 2021-01-08 04:00:46.000000 pedal-2.5.1/pedal/cait/cait_api.py
--rw-rw-rw-   0        0        0    22471 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/cait/cait_node.py
--rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/cait/constants.py
--rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.5.1/pedal/cait/find_node.py
--rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.5.1/pedal/cait/stretchy_tree_matching.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.697032 pedal-2.5.1/pedal/command_line/
--rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/command_line/__init__.py
--rw-rw-rw-   0        0        0     7897 2022-04-30 18:25:37.000000 pedal-2.5.1/pedal/command_line/command_line.py
--rw-rw-rw-   0        0        0     7301 2023-05-27 15:42:09.000000 pedal-2.5.1/pedal/command_line/mocks.py
--rw-rw-rw-   0        0        0    24491 2023-05-26 20:56:48.000000 pedal-2.5.1/pedal/command_line/modes.py
--rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.5.1/pedal/command_line/report.py
--rw-rw-rw-   0        0        0     3540 2020-11-08 16:28:36.000000 pedal-2.5.1/pedal/command_line/verify.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.717032 pedal-2.5.1/pedal/core/
--rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/__init__.py
--rw-rw-rw-   0        0        0     9342 2023-05-26 21:10:34.000000 pedal-2.5.1/pedal/core/commands.py
--rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/environment.py
--rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/errors.py
--rw-rw-rw-   0        0        0    21081 2023-06-09 14:02:52.000000 pedal-2.5.1/pedal/core/feedback.py
--rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/feedback_category.py
--rw-rw-rw-   0        0        0     7383 2023-05-26 21:59:43.000000 pedal-2.5.1/pedal/core/final_feedback.py
--rw-rw-rw-   0        0        0     8008 2023-06-10 15:13:23.000000 pedal-2.5.1/pedal/core/formatting.py
--rw-rw-rw-   0        0        0     1962 2023-05-26 21:48:15.000000 pedal-2.5.1/pedal/core/location.py
--rw-rw-rw-   0        0        0    13385 2022-11-28 05:44:51.000000 pedal-2.5.1/pedal/core/report.py
--rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/resolver.py
--rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.5.1/pedal/core/scoring.py
--rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.5.1/pedal/core/submission.py
--rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/tag.py
--rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.5.1/pedal/core/tool.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.729031 pedal-2.5.1/pedal/environments/
--rw-rw-rw-   0        0        0      658 2023-05-27 15:45:02.000000 pedal-2.5.1/pedal/environments/__init__.py
--rw-rw-rw-   0        0        0     3060 2023-05-26 21:12:20.000000 pedal-2.5.1/pedal/environments/blockpy.py
--rw-rw-rw-   0        0        0     9587 2023-05-26 21:13:02.000000 pedal-2.5.1/pedal/environments/gradescope.py
--rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.5.1/pedal/environments/jupyter.py
--rw-rw-rw-   0        0        0    10369 2023-05-26 21:13:02.000000 pedal-2.5.1/pedal/environments/nbgrader.py
--rw-rw-rw-   0        0        0      369 2023-06-08 11:46:52.000000 pedal-2.5.1/pedal/environments/none.py
--rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/environments/sandbox.py
--rw-rw-rw-   0        0        0     3684 2023-05-26 21:13:56.000000 pedal-2.5.1/pedal/environments/standard.py
--rw-rw-rw-   0        0        0     2605 2023-06-09 12:58:17.000000 pedal-2.5.1/pedal/environments/terminal.py
--rw-rw-rw-   0        0        0     6423 2023-06-08 18:48:18.000000 pedal-2.5.1/pedal/environments/vpl.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.735033 pedal-2.5.1/pedal/extensions/
--rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/extensions/__init__.py
--rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.5.1/pedal/extensions/microbit.py
--rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.5.1/pedal/extensions/plotting.py
--rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.5.1/pedal/extensions/turtles.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.744032 pedal-2.5.1/pedal/questions/
--rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.5.1/pedal/questions/__init__.py
--rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/questions/constants.py
--rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.5.1/pedal/questions/feedbacks.py
--rw-rw-rw-   0        0        0     6043 2023-05-27 15:45:43.000000 pedal-2.5.1/pedal/questions/graders.py
--rw-rw-rw-   0        0        0     3477 2023-05-26 21:13:56.000000 pedal-2.5.1/pedal/questions/loader.py
--rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.5.1/pedal/questions/pool.py
--rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.5.1/pedal/questions/questions.py
--rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.5.1/pedal/questions/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.754032 pedal-2.5.1/pedal/resolvers/
--rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.5.1/pedal/resolvers/__init__.py
--rw-rw-rw-   0        0        0      650 2023-05-27 15:45:59.000000 pedal-2.5.1/pedal/resolvers/core.py
--rw-rw-rw-   0        0        0     1504 2023-05-26 21:58:00.000000 pedal-2.5.1/pedal/resolvers/export.py
--rw-rw-rw-   0        0        0     1753 2023-05-26 21:21:28.000000 pedal-2.5.1/pedal/resolvers/full.py
--rw-rw-rw-   0        0        0     1545 2023-05-26 21:21:46.000000 pedal-2.5.1/pedal/resolvers/sectional.py
--rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.5.1/pedal/resolvers/silent.py
--rw-rw-rw-   0        0        0     4798 2023-05-26 21:21:54.000000 pedal-2.5.1/pedal/resolvers/simple.py
--rw-rw-rw-   0        0        0     1124 2023-05-26 21:34:10.000000 pedal-2.5.1/pedal/resolvers/statistics.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.767033 pedal-2.5.1/pedal/sandbox/
--rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.5.1/pedal/sandbox/__init__.py
--rw-rw-rw-   0        0        0    17919 2023-05-18 18:30:27.000000 pedal-2.5.1/pedal/sandbox/commands.py
--rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/sandbox/constants.py
--rw-rw-rw-   0        0        0     9807 2023-05-26 21:45:59.000000 pedal-2.5.1/pedal/sandbox/data.py
--rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.5.1/pedal/sandbox/exceptions.py
--rw-rw-rw-   0        0        0    10695 2023-06-10 15:55:30.000000 pedal-2.5.1/pedal/sandbox/feedbacks.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.773032 pedal-2.5.1/pedal/sandbox/library/
--rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.5.1/pedal/sandbox/library/__init__.py
--rw-rw-rw-   0        0        0     5032 2023-05-27 15:46:08.000000 pedal-2.5.1/pedal/sandbox/library/designer.py
--rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.5.1/pedal/sandbox/library/matplotlib.py
--rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.5.1/pedal/sandbox/library/microbit.py
--rw-rw-rw-   0        0        0     3404 2023-05-27 15:46:26.000000 pedal-2.5.1/pedal/sandbox/library/turtles.py
--rw-rw-rw-   0        0        0    10128 2023-05-27 15:46:15.000000 pedal-2.5.1/pedal/sandbox/mocked.py
--rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.5.1/pedal/sandbox/result.py
--rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.5.1/pedal/sandbox/sandbox.py
--rw-rw-rw-   0        0        0     5048 2023-05-27 15:46:22.000000 pedal-2.5.1/pedal/sandbox/timeout.py
--rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.5.1/pedal/sandbox/tracer.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.780031 pedal-2.5.1/pedal/source/
--rw-rw-rw-   0        0        0      914 2023-05-27 15:44:56.000000 pedal-2.5.1/pedal/source/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/source/constants.py
--rw-rw-rw-   0        0        0     5913 2023-06-10 16:42:17.000000 pedal-2.5.1/pedal/source/feedbacks.py
--rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/source/sections.py
--rw-rw-rw-   0        0        0     7716 2023-06-10 14:14:43.000000 pedal-2.5.1/pedal/source/source.py
--rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/source/substitutions.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.796032 pedal-2.5.1/pedal/tifa/
--rw-rw-rw-   0        0        0     3046 2023-05-27 15:47:23.000000 pedal-2.5.1/pedal/tifa/__init__.py
--rw-rw-rw-   0        0        0     2143 2022-10-06 14:36:45.000000 pedal-2.5.1/pedal/tifa/commands.py
--rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/tifa/constants.py
--rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.5.1/pedal/tifa/contexts.py
--rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:08.000000 pedal-2.5.1/pedal/tifa/feedbacks.py
--rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/tifa/identifier.py
--rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.5.1/pedal/tifa/settings.py
--rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.5.1/pedal/tifa/state.py
--rw-rw-rw-   0        0        0    24173 2022-10-07 14:11:04.000000 pedal-2.5.1/pedal/tifa/tifa_core.py
--rw-rw-rw-   0        0        0    42475 2023-06-08 18:43:14.000000 pedal-2.5.1/pedal/tifa/tifa_visitor.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.807034 pedal-2.5.1/pedal/types/
--rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.5.1/pedal/types/__init__.py
--rw-rw-rw-   0        0        0     9162 2023-05-27 15:45:10.000000 pedal-2.5.1/pedal/types/builtin.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.816032 pedal-2.5.1/pedal/types/library/
--rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.5.1/pedal/types/library/__init__.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.5.1/pedal/types/library/cs1_curriculum.py
--rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.5.1/pedal/types/library/designer.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.5.1/pedal/types/library/matplotlib.py
--rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.5.1/pedal/types/library/microbit.py
--rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.5.1/pedal/types/library/turtles.py
--rw-rw-rw-   0        0        0    51761 2023-05-27 15:40:45.000000 pedal-2.5.1/pedal/types/new_types.py
--rw-rw-rw-   0        0        0    14912 2023-06-08 18:43:02.000000 pedal-2.5.1/pedal/types/normalize.py
--rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.5.1/pedal/types/operations.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.831032 pedal-2.5.1/pedal/utilities/
--rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/utilities/__init__.py
--rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.5.1/pedal/utilities/ast_tools.py
--rw-rw-rw-   0        0        0     6580 2022-07-27 17:31:05.000000 pedal-2.5.1/pedal/utilities/comparisons.py
--rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/utilities/dictionaries.py
--rw-rw-rw-   0        0        0     9918 2023-06-10 16:39:35.000000 pedal-2.5.1/pedal/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.5.1/pedal/utilities/files.py
--rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/utilities/operators.py
--rw-rw-rw-   0        0        0     7037 2022-12-31 17:53:00.000000 pedal-2.5.1/pedal/utilities/progsnap.py
--rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/utilities/sorting.py
--rw-rw-rw-   0        0        0      449 2023-06-08 22:09:02.000000 pedal-2.5.1/pedal/utilities/system.py
--rw-rw-rw-   0        0        0     2457 2023-06-10 15:07:25.000000 pedal-2.5.1/pedal/utilities/text.py
--rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/utilities/types.py
--rw-rw-rw-   0        0        0      121 2023-06-11 14:14:30.833032 pedal-2.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-06-09 13:00:00.000000 pedal-2.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:51.045547 pedal-2.5.2/
+-rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.5.2/LICENSE
+-rw-rw-rw-   0        0        0     2981 2023-06-14 16:24:51.046546 pedal-2.5.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.862276 pedal-2.5.2/Pedal.egg-info/
+-rw-rw-rw-   0        0        0     2981 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3759 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 16:24:50.000000 pedal-2.5.2/Pedal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1958 2023-06-14 16:24:47.000000 pedal-2.5.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.858280 pedal-2.5.2/pedal/
+-rw-rw-rw-   0        0        0      382 2023-05-18 18:14:23.000000 pedal-2.5.2/pedal/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.878274 pedal-2.5.2/pedal/assertions/
+-rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/assertions/__init__.py
+-rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.5.2/pedal/assertions/classes.py
+-rw-rw-rw-   0        0        0    13288 2023-01-17 17:53:58.000000 pedal-2.5.2/pedal/assertions/commands.py
+-rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/assertions/constants.py
+-rw-rw-rw-   0        0        0    20355 2023-05-27 15:44:30.000000 pedal-2.5.2/pedal/assertions/feedbacks.py
+-rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.5.2/pedal/assertions/functions.py
+-rw-rw-rw-   0        0        0     5722 2021-01-26 15:12:38.000000 pedal-2.5.2/pedal/assertions/organizers.py
+-rw-rw-rw-   0        0        0    33752 2023-05-22 19:35:19.000000 pedal-2.5.2/pedal/assertions/runtime.py
+-rw-rw-rw-   0        0        0     3254 2023-05-26 21:11:25.000000 pedal-2.5.2/pedal/assertions/setup.py
+-rw-rw-rw-   0        0        0    30229 2023-05-26 20:52:09.000000 pedal-2.5.2/pedal/assertions/static.py
+-rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/assertions/unittest.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.889302 pedal-2.5.2/pedal/cait/
+-rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.5.2/pedal/cait/__init__.py
+-rw-rw-rw-   0        0        0     2255 2023-05-27 15:47:12.000000 pedal-2.5.2/pedal/cait/ast_helpers.py
+-rw-rw-rw-   0        0        0    11371 2021-03-12 21:12:46.000000 pedal-2.5.2/pedal/cait/ast_map.py
+-rw-rw-rw-   0        0        0    10523 2021-01-08 04:00:46.000000 pedal-2.5.2/pedal/cait/cait_api.py
+-rw-rw-rw-   0        0        0    22471 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/cait/cait_node.py
+-rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/cait/constants.py
+-rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.5.2/pedal/cait/find_node.py
+-rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.5.2/pedal/cait/stretchy_tree_matching.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.899304 pedal-2.5.2/pedal/command_line/
+-rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/command_line/__init__.py
+-rw-rw-rw-   0        0        0     7971 2023-06-14 15:23:15.000000 pedal-2.5.2/pedal/command_line/command_line.py
+-rw-rw-rw-   0        0        0     7301 2023-05-27 15:42:09.000000 pedal-2.5.2/pedal/command_line/mocks.py
+-rw-rw-rw-   0        0        0    24546 2023-06-14 15:43:56.000000 pedal-2.5.2/pedal/command_line/modes.py
+-rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.5.2/pedal/command_line/report.py
+-rw-rw-rw-   0        0        0     3540 2020-11-08 16:28:36.000000 pedal-2.5.2/pedal/command_line/verify.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.920224 pedal-2.5.2/pedal/core/
+-rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/__init__.py
+-rw-rw-rw-   0        0        0     9342 2023-05-26 21:10:34.000000 pedal-2.5.2/pedal/core/commands.py
+-rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/environment.py
+-rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/errors.py
+-rw-rw-rw-   0        0        0    21081 2023-06-09 14:02:52.000000 pedal-2.5.2/pedal/core/feedback.py
+-rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/feedback_category.py
+-rw-rw-rw-   0        0        0     7614 2023-06-14 16:05:08.000000 pedal-2.5.2/pedal/core/final_feedback.py
+-rw-rw-rw-   0        0        0     8008 2023-06-10 15:13:23.000000 pedal-2.5.2/pedal/core/formatting.py
+-rw-rw-rw-   0        0        0     1962 2023-05-26 21:48:15.000000 pedal-2.5.2/pedal/core/location.py
+-rw-rw-rw-   0        0        0    13385 2022-11-28 05:44:51.000000 pedal-2.5.2/pedal/core/report.py
+-rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/resolver.py
+-rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.5.2/pedal/core/scoring.py
+-rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.5.2/pedal/core/submission.py
+-rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/core/tag.py
+-rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.5.2/pedal/core/tool.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.935551 pedal-2.5.2/pedal/environments/
+-rw-rw-rw-   0        0        0      670 2023-06-14 15:19:32.000000 pedal-2.5.2/pedal/environments/__init__.py
+-rw-rw-rw-   0        0        0     3060 2023-05-26 21:12:20.000000 pedal-2.5.2/pedal/environments/blockpy.py
+-rw-rw-rw-   0        0        0     9587 2023-05-26 21:13:02.000000 pedal-2.5.2/pedal/environments/gradescope.py
+-rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.5.2/pedal/environments/jupyter.py
+-rw-rw-rw-   0        0        0    10369 2023-05-26 21:13:02.000000 pedal-2.5.2/pedal/environments/nbgrader.py
+-rw-rw-rw-   0        0        0      369 2023-06-08 11:46:52.000000 pedal-2.5.2/pedal/environments/none.py
+-rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/environments/sandbox.py
+-rw-rw-rw-   0        0        0     3684 2023-05-26 21:13:56.000000 pedal-2.5.2/pedal/environments/standard.py
+-rw-rw-rw-   0        0        0     3201 2023-06-14 16:08:09.000000 pedal-2.5.2/pedal/environments/terminal.py
+-rw-rw-rw-   0        0        0     6423 2023-06-08 18:48:18.000000 pedal-2.5.2/pedal/environments/vpl.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.941546 pedal-2.5.2/pedal/extensions/
+-rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/extensions/__init__.py
+-rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.5.2/pedal/extensions/microbit.py
+-rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.5.2/pedal/extensions/plotting.py
+-rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.5.2/pedal/extensions/turtles.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.953545 pedal-2.5.2/pedal/questions/
+-rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.5.2/pedal/questions/__init__.py
+-rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/questions/constants.py
+-rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.5.2/pedal/questions/feedbacks.py
+-rw-rw-rw-   0        0        0     6043 2023-05-27 15:45:43.000000 pedal-2.5.2/pedal/questions/graders.py
+-rw-rw-rw-   0        0        0     3477 2023-05-26 21:13:56.000000 pedal-2.5.2/pedal/questions/loader.py
+-rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.5.2/pedal/questions/pool.py
+-rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.5.2/pedal/questions/questions.py
+-rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.5.2/pedal/questions/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.966547 pedal-2.5.2/pedal/resolvers/
+-rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.5.2/pedal/resolvers/__init__.py
+-rw-rw-rw-   0        0        0      650 2023-05-27 15:45:59.000000 pedal-2.5.2/pedal/resolvers/core.py
+-rw-rw-rw-   0        0        0     1504 2023-05-26 21:58:00.000000 pedal-2.5.2/pedal/resolvers/export.py
+-rw-rw-rw-   0        0        0     1753 2023-05-26 21:21:28.000000 pedal-2.5.2/pedal/resolvers/full.py
+-rw-rw-rw-   0        0        0     1545 2023-05-26 21:21:46.000000 pedal-2.5.2/pedal/resolvers/sectional.py
+-rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.5.2/pedal/resolvers/silent.py
+-rw-rw-rw-   0        0        0     4798 2023-05-26 21:21:54.000000 pedal-2.5.2/pedal/resolvers/simple.py
+-rw-rw-rw-   0        0        0     1124 2023-05-26 21:34:10.000000 pedal-2.5.2/pedal/resolvers/statistics.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.982547 pedal-2.5.2/pedal/sandbox/
+-rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.5.2/pedal/sandbox/__init__.py
+-rw-rw-rw-   0        0        0    17919 2023-05-18 18:30:27.000000 pedal-2.5.2/pedal/sandbox/commands.py
+-rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/sandbox/constants.py
+-rw-rw-rw-   0        0        0     9807 2023-05-26 21:45:59.000000 pedal-2.5.2/pedal/sandbox/data.py
+-rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.5.2/pedal/sandbox/exceptions.py
+-rw-rw-rw-   0        0        0    10695 2023-06-10 15:55:30.000000 pedal-2.5.2/pedal/sandbox/feedbacks.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.989546 pedal-2.5.2/pedal/sandbox/library/
+-rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.5.2/pedal/sandbox/library/__init__.py
+-rw-rw-rw-   0        0        0     5032 2023-05-27 15:46:08.000000 pedal-2.5.2/pedal/sandbox/library/designer.py
+-rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.5.2/pedal/sandbox/library/matplotlib.py
+-rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.5.2/pedal/sandbox/library/microbit.py
+-rw-rw-rw-   0        0        0     3404 2023-05-27 15:46:26.000000 pedal-2.5.2/pedal/sandbox/library/turtles.py
+-rw-rw-rw-   0        0        0    10128 2023-05-27 15:46:15.000000 pedal-2.5.2/pedal/sandbox/mocked.py
+-rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.5.2/pedal/sandbox/result.py
+-rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.5.2/pedal/sandbox/sandbox.py
+-rw-rw-rw-   0        0        0     5048 2023-05-27 15:46:22.000000 pedal-2.5.2/pedal/sandbox/timeout.py
+-rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.5.2/pedal/sandbox/tracer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:50.997547 pedal-2.5.2/pedal/source/
+-rw-rw-rw-   0        0        0      914 2023-05-27 15:44:56.000000 pedal-2.5.2/pedal/source/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/source/constants.py
+-rw-rw-rw-   0        0        0     5913 2023-06-10 16:42:17.000000 pedal-2.5.2/pedal/source/feedbacks.py
+-rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/source/sections.py
+-rw-rw-rw-   0        0        0     7716 2023-06-10 14:14:43.000000 pedal-2.5.2/pedal/source/source.py
+-rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/source/substitutions.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:51.011547 pedal-2.5.2/pedal/tifa/
+-rw-rw-rw-   0        0        0     3046 2023-05-27 15:47:23.000000 pedal-2.5.2/pedal/tifa/__init__.py
+-rw-rw-rw-   0        0        0     2143 2022-10-06 14:36:45.000000 pedal-2.5.2/pedal/tifa/commands.py
+-rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/tifa/constants.py
+-rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.5.2/pedal/tifa/contexts.py
+-rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:08.000000 pedal-2.5.2/pedal/tifa/feedbacks.py
+-rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/tifa/identifier.py
+-rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.5.2/pedal/tifa/settings.py
+-rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.5.2/pedal/tifa/state.py
+-rw-rw-rw-   0        0        0    24173 2022-10-07 14:11:04.000000 pedal-2.5.2/pedal/tifa/tifa_core.py
+-rw-rw-rw-   0        0        0    42475 2023-06-08 18:43:14.000000 pedal-2.5.2/pedal/tifa/tifa_visitor.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:51.018548 pedal-2.5.2/pedal/types/
+-rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.5.2/pedal/types/__init__.py
+-rw-rw-rw-   0        0        0     9162 2023-05-27 15:45:10.000000 pedal-2.5.2/pedal/types/builtin.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:51.026546 pedal-2.5.2/pedal/types/library/
+-rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.5.2/pedal/types/library/__init__.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.5.2/pedal/types/library/cs1_curriculum.py
+-rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.5.2/pedal/types/library/designer.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.5.2/pedal/types/library/matplotlib.py
+-rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.5.2/pedal/types/library/microbit.py
+-rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.5.2/pedal/types/library/turtles.py
+-rw-rw-rw-   0        0        0    51761 2023-05-27 15:40:45.000000 pedal-2.5.2/pedal/types/new_types.py
+-rw-rw-rw-   0        0        0    14912 2023-06-08 18:43:02.000000 pedal-2.5.2/pedal/types/normalize.py
+-rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.5.2/pedal/types/operations.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:24:51.044546 pedal-2.5.2/pedal/utilities/
+-rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.5.2/pedal/utilities/ast_tools.py
+-rw-rw-rw-   0        0        0     6580 2022-07-27 17:31:05.000000 pedal-2.5.2/pedal/utilities/comparisons.py
+-rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/utilities/dictionaries.py
+-rw-rw-rw-   0        0        0     9918 2023-06-10 16:39:35.000000 pedal-2.5.2/pedal/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.5.2/pedal/utilities/files.py
+-rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/utilities/operators.py
+-rw-rw-rw-   0        0        0     7037 2022-12-31 17:53:00.000000 pedal-2.5.2/pedal/utilities/progsnap.py
+-rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/utilities/sorting.py
+-rw-rw-rw-   0        0        0      449 2023-06-08 22:09:02.000000 pedal-2.5.2/pedal/utilities/system.py
+-rw-rw-rw-   0        0        0     2457 2023-06-10 15:07:25.000000 pedal-2.5.2/pedal/utilities/text.py
+-rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.5.2/pedal/utilities/types.py
+-rw-rw-rw-   0        0        0      121 2023-06-14 16:24:51.047546 pedal-2.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-06-14 16:22:25.000000 pedal-2.5.2/setup.py
```

### Comparing `pedal-2.5.1/LICENSE` & `pedal-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/PKG-INFO` & `pedal-2.5.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: pedal
-Version: 2.5.1
+Version: 2.5.2
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
+Description: Pedal
+        =====
+        
+        .. image:: https://github.com/pedal-edu/pedal/workflows/Test%20and%20Lint/badge.svg
+            :alt: Unit Tests for 3.6, 3.7, 3.8, 3.9
+        
+        
+        .. image:: https://github.com/pedal-edu/pedal/workflows/Build%20Documentation/badge.svg
+            :alt: Documentation
+        
+        A collection of tools to analyze student's work in a pipeline.
+        Pedal not only provides some of these tools, but it provides a *framework*
+        around those tools.
+        
+        Installation
+        ============
+        
+        Install from PyPi::
+            
+            pip install pedal
+        
+        Or install from the https://github.com/acbart/pedal repository
+        
+        Important Concepts
+        ==================
+        
+        Pedal revolves around providing *Feedback Functions* that can be called in an
+        Instructor Control Script to generate *Feedback* for a *Submission*, which are
+        all attached to a *Report*. A *Resolver* can then transform that Feedback into
+        something that an *Environment* can hand off to a learner (or other interested
+        party). These Feedback Functions are organized into *Tools*.
+        
+        .. image:: https://raw.githubusercontent.com/pedal-edu/pedal/master/docsrc/_static/pedal-overview-v3.png
+        
+        One of our major goals is to attach metadata to feedback to enable easier
+        analysis, versioning, and evaluation. Although Instructor Control Scripts can
+        be written very imperatively to specify very complex (or simple) grading logic,
+        we are trying to reach an elegant, declarative style. This will enable tooling
+        to automatically generate reports on occurrences of feedback, connect to
+        datasets like those in the ProgSnap format, and allow us to "unit test our
+        unit tests".
+        
+        One of our other goals for this project is to categorize Feedbacks' Conditions
+        and Responses, using concepts established by Narciss 2006. For example, we
+        say some Kinds of Responses are "hints" instead of "mistakes". We also say
+        that Conditions can be Categorized as being from "Specifications" or
+        "Runtime".
+        
+        For more information, check out the docs for Pedal_.
+        
+        .. _Pedal: https://pedal-edu.github.io/pedal
+        
 Keywords: feedback education teaching program analysis tifa cait sandbox pedal grading grader grade
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Requires-Python: >=3.7
-License-File: LICENSE
-
-Pedal
-=====
-
-.. image:: https://github.com/pedal-edu/pedal/workflows/Test%20and%20Lint/badge.svg
-    :alt: Unit Tests for 3.6, 3.7, 3.8, 3.9
-
-
-.. image:: https://github.com/pedal-edu/pedal/workflows/Build%20Documentation/badge.svg
-    :alt: Documentation
-
-A collection of tools to analyze student's work in a pipeline.
-Pedal not only provides some of these tools, but it provides a *framework*
-around those tools.
-
-Installation
-============
-
-Install from PyPi::
-    
-    pip install pedal
-
-Or install from the https://github.com/acbart/pedal repository
-
-Important Concepts
-==================
-
-Pedal revolves around providing *Feedback Functions* that can be called in an
-Instructor Control Script to generate *Feedback* for a *Submission*, which are
-all attached to a *Report*. A *Resolver* can then transform that Feedback into
-something that an *Environment* can hand off to a learner (or other interested
-party). These Feedback Functions are organized into *Tools*.
-
-.. image:: https://raw.githubusercontent.com/pedal-edu/pedal/master/docsrc/_static/pedal-overview-v3.png
-
-One of our major goals is to attach metadata to feedback to enable easier
-analysis, versioning, and evaluation. Although Instructor Control Scripts can
-be written very imperatively to specify very complex (or simple) grading logic,
-we are trying to reach an elegant, declarative style. This will enable tooling
-to automatically generate reports on occurrences of feedback, connect to
-datasets like those in the ProgSnap format, and allow us to "unit test our
-unit tests".
-
-One of our other goals for this project is to categorize Feedbacks' Conditions
-and Responses, using concepts established by Narciss 2006. For example, we
-say some Kinds of Responses are "hints" instead of "mistakes". We also say
-that Conditions can be Categorized as being from "Specifications" or
-"Runtime".
-
-For more information, check out the docs for Pedal_.
-
-.. _Pedal: https://pedal-edu.github.io/pedal
```

### Comparing `pedal-2.5.1/Pedal.egg-info/PKG-INFO` & `pedal-2.5.2/Pedal.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: pedal
-Version: 2.5.1
+Version: 2.5.2
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
+Description: Pedal
+        =====
+        
+        .. image:: https://github.com/pedal-edu/pedal/workflows/Test%20and%20Lint/badge.svg
+            :alt: Unit Tests for 3.6, 3.7, 3.8, 3.9
+        
+        
+        .. image:: https://github.com/pedal-edu/pedal/workflows/Build%20Documentation/badge.svg
+            :alt: Documentation
+        
+        A collection of tools to analyze student's work in a pipeline.
+        Pedal not only provides some of these tools, but it provides a *framework*
+        around those tools.
+        
+        Installation
+        ============
+        
+        Install from PyPi::
+            
+            pip install pedal
+        
+        Or install from the https://github.com/acbart/pedal repository
+        
+        Important Concepts
+        ==================
+        
+        Pedal revolves around providing *Feedback Functions* that can be called in an
+        Instructor Control Script to generate *Feedback* for a *Submission*, which are
+        all attached to a *Report*. A *Resolver* can then transform that Feedback into
+        something that an *Environment* can hand off to a learner (or other interested
+        party). These Feedback Functions are organized into *Tools*.
+        
+        .. image:: https://raw.githubusercontent.com/pedal-edu/pedal/master/docsrc/_static/pedal-overview-v3.png
+        
+        One of our major goals is to attach metadata to feedback to enable easier
+        analysis, versioning, and evaluation. Although Instructor Control Scripts can
+        be written very imperatively to specify very complex (or simple) grading logic,
+        we are trying to reach an elegant, declarative style. This will enable tooling
+        to automatically generate reports on occurrences of feedback, connect to
+        datasets like those in the ProgSnap format, and allow us to "unit test our
+        unit tests".
+        
+        One of our other goals for this project is to categorize Feedbacks' Conditions
+        and Responses, using concepts established by Narciss 2006. For example, we
+        say some Kinds of Responses are "hints" instead of "mistakes". We also say
+        that Conditions can be Categorized as being from "Specifications" or
+        "Runtime".
+        
+        For more information, check out the docs for Pedal_.
+        
+        .. _Pedal: https://pedal-edu.github.io/pedal
+        
 Keywords: feedback education teaching program analysis tifa cait sandbox pedal grading grader grade
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Requires-Python: >=3.7
-License-File: LICENSE
-
-Pedal
-=====
-
-.. image:: https://github.com/pedal-edu/pedal/workflows/Test%20and%20Lint/badge.svg
-    :alt: Unit Tests for 3.6, 3.7, 3.8, 3.9
-
-
-.. image:: https://github.com/pedal-edu/pedal/workflows/Build%20Documentation/badge.svg
-    :alt: Documentation
-
-A collection of tools to analyze student's work in a pipeline.
-Pedal not only provides some of these tools, but it provides a *framework*
-around those tools.
-
-Installation
-============
-
-Install from PyPi::
-    
-    pip install pedal
-
-Or install from the https://github.com/acbart/pedal repository
-
-Important Concepts
-==================
-
-Pedal revolves around providing *Feedback Functions* that can be called in an
-Instructor Control Script to generate *Feedback* for a *Submission*, which are
-all attached to a *Report*. A *Resolver* can then transform that Feedback into
-something that an *Environment* can hand off to a learner (or other interested
-party). These Feedback Functions are organized into *Tools*.
-
-.. image:: https://raw.githubusercontent.com/pedal-edu/pedal/master/docsrc/_static/pedal-overview-v3.png
-
-One of our major goals is to attach metadata to feedback to enable easier
-analysis, versioning, and evaluation. Although Instructor Control Scripts can
-be written very imperatively to specify very complex (or simple) grading logic,
-we are trying to reach an elegant, declarative style. This will enable tooling
-to automatically generate reports on occurrences of feedback, connect to
-datasets like those in the ProgSnap format, and allow us to "unit test our
-unit tests".
-
-One of our other goals for this project is to categorize Feedbacks' Conditions
-and Responses, using concepts established by Narciss 2006. For example, we
-say some Kinds of Responses are "hints" instead of "mistakes". We also say
-that Conditions can be Categorized as being from "Specifications" or
-"Runtime".
-
-For more information, check out the docs for Pedal_.
-
-.. _Pedal: https://pedal-edu.github.io/pedal
```

### Comparing `pedal-2.5.1/Pedal.egg-info/SOURCES.txt` & `pedal-2.5.2/Pedal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/README.rst` & `pedal-2.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/assertions/__init__.py` & `pedal-2.5.2/pedal/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/assertions/classes.py` & `pedal-2.5.2/pedal/assertions/classes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/assertions/commands.py` & `pedal-2.5.2/pedal/assertions/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/assertions/feedbacks.py` & `pedal-2.5.2/pedal/assertions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/assertions/functions.py` & `pedal-2.5.2/pedal/assertions/functions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/assertions/organizers.py` & `pedal-2.5.2/pedal/assertions/organizers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/assertions/runtime.py` & `pedal-2.5.2/pedal/assertions/runtime.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/assertions/setup.py` & `pedal-2.5.2/pedal/assertions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/assertions/static.py` & `pedal-2.5.2/pedal/assertions/static.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/assertions/unittest.py` & `pedal-2.5.2/pedal/assertions/unittest.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/cait/ast_helpers.py` & `pedal-2.5.2/pedal/cait/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/cait/ast_map.py` & `pedal-2.5.2/pedal/cait/ast_map.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/cait/cait_api.py` & `pedal-2.5.2/pedal/cait/cait_api.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/cait/cait_node.py` & `pedal-2.5.2/pedal/cait/cait_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/cait/find_node.py` & `pedal-2.5.2/pedal/cait/find_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/cait/stretchy_tree_matching.py` & `pedal-2.5.2/pedal/cait/stretchy_tree_matching.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/command_line/command_line.py` & `pedal-2.5.2/pedal/command_line/command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 Config settings
     seed
     create_missing_outputs
 """
 
 import argparse
 from pedal.command_line.modes import MODES
+from pedal.environments import ALL_ENVIRONMENTS
 
 
 def main(args=None):
     """
     Actually runs Pedal from the command line.
 
     Args:
@@ -94,15 +95,15 @@
                         help="Uses the configuration file to get settings.")
     parser.add_argument('--create_output', '-m',
                         help="In verify mode, creates any missing outputs.",
                         action='store_true')
     parser.add_argument('--environment', '-e',
                         help="Sets the environment context for this script, which"
                              " can run special setups and override tools as"
-                             " needed.", default='standard')
+                             " needed.", default='standard', choices=ALL_ENVIRONMENTS)
     parser.add_argument('--instructor_name',
                         help="Sets the name of the instructor file to something"
                              " more friendly. If not given, then will default"
                              " to the instructor filename.", default=None)
     parser.add_argument('--progsnap_profile',
                         default='blockpy', # TODO: Change this biased default
                         help="Uses the given profile's default settings for"
```

### Comparing `pedal-2.5.1/pedal/command_line/mocks.py` & `pedal-2.5.2/pedal/command_line/mocks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/command_line/modes.py` & `pedal-2.5.2/pedal/command_line/modes.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,24 +313,25 @@
                   bundle.submission.main_file,
                   bool(bundle.result.error))
 
 
 class FeedbackPipeline(AbstractPipeline):
     def process_output(self):
         for bundle in self.submissions:
-            print(bundle.submission.instructor_file,
-                  bundle.submission.main_file)
+            #print(bundle.submission.instructor_file,
+            #      bundle.submission.main_file)
             if bundle.result.error:
                 print(bundle.result.error)
             elif bundle.result.resolution:
                 # report = bundle.result.data['MAIN_REPORT']
-                print(bundle.result.resolution.title)
-                print(bundle.result.resolution.message)
+                #print(bundle.result.resolution.title)
+                #print(bundle.result.resolution.message)
+                print(bundle.result.output)
             else:
-                print("No feedback determined.")
+                print("Error: No feedback determined.")
 
 
 class RunPipeline(AbstractPipeline):
     def process_output(self):
         for bundle in self.submissions:
             print(bundle.submission.instructor_file,
                   bundle.submission.main_file)
```

### Comparing `pedal-2.5.1/pedal/command_line/report.py` & `pedal-2.5.2/pedal/command_line/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/command_line/verify.py` & `pedal-2.5.2/pedal/command_line/verify.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/commands.py` & `pedal-2.5.2/pedal/core/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/environment.py` & `pedal-2.5.2/pedal/core/environment.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/errors.py` & `pedal-2.5.2/pedal/core/errors.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/feedback.py` & `pedal-2.5.2/pedal/core/feedback.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/feedback_category.py` & `pedal-2.5.2/pedal/core/feedback_category.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/final_feedback.py` & `pedal-2.5.2/pedal/core/final_feedback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from pedal.core.feedback import Feedback
 from pedal.core.commands import set_correct
 from pedal.core.report import Report
 from pedal.core.scoring import Score, combine_scores
 
 
 def parse_feedback(feedback):
@@ -170,14 +171,20 @@
             'title': self.title,
             'message': self.message,
             'data': self.data,
             'hide_correctness': self.hide_correctness,
             'location': self.data.get('location', None) if self.data else None
         }
 
+    def to_file(self, path, format='json'):
+        with open(path, 'w') as f:
+            if format == 'json':
+                json.dump(self.to_json(), f)
+            else:
+                f.write(self.for_console())
 
 def set_correct_no_errors(report: Report) -> FinalFeedback:
     return FinalFeedback(correct=True, score=0,
                          title=None, message=None,
                          category=Feedback.CATEGORIES.COMPLETE,
                          label=FinalFeedback.DEFAULT_NO_FEEDBACK_LABEL,
                          data=[], hide_correctness=False,
```

### Comparing `pedal-2.5.1/pedal/core/formatting.py` & `pedal-2.5.2/pedal/core/formatting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/location.py` & `pedal-2.5.2/pedal/core/location.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/report.py` & `pedal-2.5.2/pedal/core/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/resolver.py` & `pedal-2.5.2/pedal/core/resolver.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/scoring.py` & `pedal-2.5.2/pedal/core/scoring.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/submission.py` & `pedal-2.5.2/pedal/core/submission.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/core/tool.py` & `pedal-2.5.2/pedal/core/tool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/environments/__init__.py` & `pedal-2.5.2/pedal/environments/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,9 +28,9 @@
         results.append(execute())
     return tuple(results)
 '''
 
 from pedal.environments.standard import setup_environment
 
 ALL_ENVIRONMENTS = [
-    'blockpy', 'gradescope', 'jupyter', 'standard', 'vpl'
+    'blockpy', 'gradescope', 'jupyter', 'standard', 'vpl', 'terminal'
 ]
```

### Comparing `pedal-2.5.1/pedal/environments/blockpy.py` & `pedal-2.5.2/pedal/environments/blockpy.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/environments/gradescope.py` & `pedal-2.5.2/pedal/environments/gradescope.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/environments/jupyter.py` & `pedal-2.5.2/pedal/environments/jupyter.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/environments/nbgrader.py` & `pedal-2.5.2/pedal/environments/nbgrader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/environments/sandbox.py` & `pedal-2.5.2/pedal/environments/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/environments/standard.py` & `pedal-2.5.2/pedal/environments/standard.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/environments/vpl.py` & `pedal-2.5.2/pedal/environments/vpl.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/extensions/microbit.py` & `pedal-2.5.2/pedal/extensions/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/extensions/plotting.py` & `pedal-2.5.2/pedal/extensions/plotting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/questions/__init__.py` & `pedal-2.5.2/pedal/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/questions/feedbacks.py` & `pedal-2.5.2/pedal/questions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/questions/graders.py` & `pedal-2.5.2/pedal/questions/graders.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/questions/loader.py` & `pedal-2.5.2/pedal/questions/loader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/questions/pool.py` & `pedal-2.5.2/pedal/questions/pool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/questions/questions.py` & `pedal-2.5.2/pedal/questions/questions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/questions/setup.py` & `pedal-2.5.2/pedal/questions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/resolvers/__init__.py` & `pedal-2.5.2/pedal/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/resolvers/core.py` & `pedal-2.5.2/pedal/resolvers/core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/resolvers/export.py` & `pedal-2.5.2/pedal/resolvers/export.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/resolvers/full.py` & `pedal-2.5.2/pedal/resolvers/full.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/resolvers/sectional.py` & `pedal-2.5.2/pedal/resolvers/sectional.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/resolvers/simple.py` & `pedal-2.5.2/pedal/resolvers/simple.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/resolvers/statistics.py` & `pedal-2.5.2/pedal/resolvers/statistics.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/__init__.py` & `pedal-2.5.2/pedal/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/commands.py` & `pedal-2.5.2/pedal/sandbox/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/data.py` & `pedal-2.5.2/pedal/sandbox/data.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/exceptions.py` & `pedal-2.5.2/pedal/sandbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/feedbacks.py` & `pedal-2.5.2/pedal/sandbox/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/library/designer.py` & `pedal-2.5.2/pedal/sandbox/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/library/matplotlib.py` & `pedal-2.5.2/pedal/sandbox/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/library/microbit.py` & `pedal-2.5.2/pedal/sandbox/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/library/turtles.py` & `pedal-2.5.2/pedal/sandbox/library/turtles.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/mocked.py` & `pedal-2.5.2/pedal/sandbox/mocked.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/result.py` & `pedal-2.5.2/pedal/sandbox/result.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/sandbox.py` & `pedal-2.5.2/pedal/sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/timeout.py` & `pedal-2.5.2/pedal/sandbox/timeout.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/sandbox/tracer.py` & `pedal-2.5.2/pedal/sandbox/tracer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/source/__init__.py` & `pedal-2.5.2/pedal/source/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/source/feedbacks.py` & `pedal-2.5.2/pedal/source/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/source/sections.py` & `pedal-2.5.2/pedal/source/sections.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/source/source.py` & `pedal-2.5.2/pedal/source/source.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/tifa/__init__.py` & `pedal-2.5.2/pedal/tifa/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/tifa/commands.py` & `pedal-2.5.2/pedal/tifa/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/tifa/contexts.py` & `pedal-2.5.2/pedal/tifa/contexts.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/tifa/feedbacks.py` & `pedal-2.5.2/pedal/tifa/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/tifa/identifier.py` & `pedal-2.5.2/pedal/tifa/identifier.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/tifa/settings.py` & `pedal-2.5.2/pedal/tifa/settings.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/tifa/state.py` & `pedal-2.5.2/pedal/tifa/state.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/tifa/tifa_core.py` & `pedal-2.5.2/pedal/tifa/tifa_core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/tifa/tifa_visitor.py` & `pedal-2.5.2/pedal/tifa/tifa_visitor.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/types/builtin.py` & `pedal-2.5.2/pedal/types/builtin.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/types/library/cs1_curriculum.py` & `pedal-2.5.2/pedal/types/library/cs1_curriculum.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/types/library/designer.py` & `pedal-2.5.2/pedal/types/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/types/library/matplotlib.py` & `pedal-2.5.2/pedal/types/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/types/library/microbit.py` & `pedal-2.5.2/pedal/types/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/types/new_types.py` & `pedal-2.5.2/pedal/types/new_types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/types/normalize.py` & `pedal-2.5.2/pedal/types/normalize.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/types/operations.py` & `pedal-2.5.2/pedal/types/operations.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/utilities/__init__.py` & `pedal-2.5.2/pedal/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/utilities/ast_tools.py` & `pedal-2.5.2/pedal/utilities/ast_tools.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/utilities/comparisons.py` & `pedal-2.5.2/pedal/utilities/comparisons.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/utilities/dictionaries.py` & `pedal-2.5.2/pedal/utilities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/utilities/exceptions.py` & `pedal-2.5.2/pedal/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/utilities/files.py` & `pedal-2.5.2/pedal/utilities/files.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/utilities/operators.py` & `pedal-2.5.2/pedal/utilities/operators.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/utilities/progsnap.py` & `pedal-2.5.2/pedal/utilities/progsnap.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/utilities/sorting.py` & `pedal-2.5.2/pedal/utilities/sorting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/utilities/text.py` & `pedal-2.5.2/pedal/utilities/text.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/pedal/utilities/types.py` & `pedal-2.5.2/pedal/utilities/types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.1/setup.py` & `pedal-2.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pedal',
-    version='2.5.1',
+    version='2.5.2',
     python_requires='>=3.7',
     author='acbart,lukesg08',
     author_email='acbart@udel.edu',
     description='Tools to provide feedback on student code.',
     keywords='feedback education teaching program analysis tifa cait sandbox pedal grading grader grade',
     packages=['pedal', 'pedal.core', 'pedal.utilities', 'pedal.environments',
               'pedal.resolvers', 'pedal.command_line',
```

