# Comparing `tmp/microt_prompt-0.1.8.tar.gz` & `tmp/microt_prompt-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jixin\Documents\Bitbucket\microt_compliance\dist\.tmp-im_ybp7y\microt_prompt-0.1.8.tar", last modified: Sat Feb 11 17:20:33 2023, max compression
+gzip compressed data, was "C:\Users\jixin\Documents\Bitbucket\microt_compliance\dist\.tmp-5qtb0mxe\microt_prompt-0.1.9.tar", last modified: Sat Feb 11 18:40:48 2023, max compression
```

## Comparing `microt_prompt-0.1.8.tar` & `microt_prompt-0.1.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-02-11 17:20:33.043031 microt_prompt-0.1.8/
--rw-rw-rw-   0        0        0     1108 2021-08-02 19:35:31.000000 microt_prompt-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     7501 2023-02-11 17:20:33.044037 microt_prompt-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     6848 2021-08-03 18:21:32.000000 microt_prompt-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-11 17:20:32.882035 microt_prompt-0.1.8/microt_prompt.egg-info/
--rw-rw-rw-   0        0        0     7501 2023-02-11 17:20:32.000000 microt_prompt-0.1.8/microt_prompt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3275 2023-02-11 17:20:32.000000 microt_prompt-0.1.8/microt_prompt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-11 17:20:32.000000 microt_prompt-0.1.8/microt_prompt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-02-11 17:20:32.000000 microt_prompt-0.1.8/microt_prompt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-11 17:20:32.890021 microt_prompt-0.1.8/microt_prompt_matrix/
--rw-rw-rw-   0        0        0       95 2021-08-03 14:21:25.000000 microt_prompt-0.1.8/microt_prompt_matrix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-11 17:20:32.941038 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/
--rw-rw-rw-   0        0        0      470 2023-01-27 15:43:18.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/__init__.py
--rw-rw-rw-   0        0        0     7614 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/battery_level.py
--rw-rw-rw-   0        0        0      908 2023-01-26 14:17:21.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/compliance.py
--rw-rw-rw-   0        0        0      790 2023-01-26 14:17:38.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/day_of_the_week.py
--rw-rw-rw-   0        0        0     1943 2023-01-26 14:18:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/days_in_study.py
--rw-rw-rw-   0        0        0     1327 2023-01-26 14:18:24.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/home_location.py
--rw-rw-rw-   0        0        0    11103 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/location.py
--rw-rw-rw-   0        0        0     2884 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/location_label.py
--rw-rw-rw-   0        0        0    12601 2023-02-11 16:59:25.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/mims_summary.py
--rw-rw-rw-   0        0        0     1935 2023-01-26 14:20:50.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/parts_of_waking_hour.py
--rw-rw-rw-   0        0        0     7373 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/phone_detected_activity.py
--rw-rw-rw-   0        0        0     8688 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/phone_lock.py
-drwxrwxrwx   0        0        0        0 2023-02-11 17:20:32.950035 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/prompt_response/
--rw-rw-rw-   0        0        0       84 2021-07-29 20:26:38.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/prompt_response/__init__.py
--rw-rw-rw-   0        0        0     1977 2023-01-26 14:15:57.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/prompt_response/combine_appended_response.py
--rw-rw-rw-   0        0        0    10565 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/prompt_response/preprocess_promptResponse_raw.py
--rw-rw-rw-   0        0        0     7666 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/screen_status.py
--rw-rw-rw-   0        0        0      813 2023-01-26 14:21:57.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/study_mode.py
--rw-rw-rw-   0        0        0     1147 2023-01-26 14:22:10.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/time_of_the_day.py
--rw-rw-rw-   0        0        0     5814 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/waking_hours.py
-drwxrwxrwx   0        0        0        0 2023-02-11 17:20:33.001035 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/
--rw-rw-rw-   0        0        0      431 2023-01-26 14:24:13.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/__init__.py
--rw-rw-rw-   0        0        0     7610 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/battery_level.py
--rw-rw-rw-   0        0        0      908 2023-01-26 14:25:11.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/compliance.py
--rw-rw-rw-   0        0        0      790 2023-01-26 14:25:26.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/day_of_the_week.py
--rw-rw-rw-   0        0        0     2113 2023-01-26 14:25:51.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/days_in_study.py
--rw-rw-rw-   0        0        0     1327 2023-01-26 14:26:05.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/home_location.py
--rw-rw-rw-   0        0        0    11122 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/location.py
--rw-rw-rw-   0        0        0     2884 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/location_label.py
--rw-rw-rw-   0        0        0     6456 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/mims_summary.py
--rw-rw-rw-   0        0        0     1935 2023-01-26 14:28:29.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/parts_of_waking_hour.py
--rw-rw-rw-   0        0        0     8687 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/phone_lock.py
-drwxrwxrwx   0        0        0        0 2023-02-11 17:20:33.010038 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/prompt_response/
--rw-rw-rw-   0        0        0       84 2023-01-26 14:23:01.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/prompt_response/__init__.py
--rw-rw-rw-   0        0        0     1977 2023-01-26 14:23:13.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/prompt_response/combine_appended_response.py
--rw-rw-rw-   0        0        0     6606 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/prompt_response/preprocess_promptResponse_raw.py
--rw-rw-rw-   0        0        0     7523 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/screen_status.py
--rw-rw-rw-   0        0        0      815 2023-01-26 14:01:52.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/study_mode.py
--rw-rw-rw-   0        0        0     1147 2023-01-26 14:30:23.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/time_of_the_day.py
--rw-rw-rw-   0        0        0     6547 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/waking_hours.py
--rw-rw-rw-   0        0        0     7008 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/main_ema.py
--rw-rw-rw-   0        0        0     6690 2023-01-27 17:14:07.000000 microt_prompt-0.1.8/microt_prompt_matrix/main_uema.py
-drwxrwxrwx   0        0        0        0 2023-02-11 17:20:33.041002 microt_prompt-0.1.8/microt_prompt_matrix/utils/
--rw-rw-rw-   0        0        0      306 2023-01-26 14:32:19.000000 microt_prompt-0.1.8/microt_prompt_matrix/utils/__init__.py
--rw-rw-rw-   0        0        0     2130 2023-01-26 14:32:27.000000 microt_prompt-0.1.8/microt_prompt_matrix/utils/convert_timestamp.py
--rw-rw-rw-   0        0        0      642 2023-01-26 14:32:36.000000 microt_prompt-0.1.8/microt_prompt_matrix/utils/extract_participant_id.py
--rw-rw-rw-   0        0        0      908 2023-01-26 14:33:03.000000 microt_prompt-0.1.8/microt_prompt_matrix/utils/get_haversine_distance.py
--rw-rw-rw-   0        0        0      154 2023-01-26 14:01:52.000000 microt_prompt-0.1.8/microt_prompt_matrix/utils/get_time_diff.py
--rw-rw-rw-   0        0        0     4105 2023-01-26 14:33:19.000000 microt_prompt-0.1.8/microt_prompt_matrix/utils/home_coordinates.py
--rw-rw-rw-   0        0        0     4964 2023-01-26 14:33:26.000000 microt_prompt-0.1.8/microt_prompt_matrix/utils/load_participant_study_info.py
--rw-rw-rw-   0        0        0     1653 2023-01-26 14:33:34.000000 microt_prompt-0.1.8/microt_prompt_matrix/utils/parse_participants.py
--rw-rw-rw-   0        0        0     1441 2023-01-26 14:33:41.000000 microt_prompt-0.1.8/microt_prompt_matrix/utils/uncompress_file.py
--rw-rw-rw-   0        0        0     1351 2023-01-26 14:33:50.000000 microt_prompt-0.1.8/microt_prompt_matrix/utils/validate_date.py
--rw-rw-rw-   0        0        0     1207 2023-01-26 14:33:59.000000 microt_prompt-0.1.8/microt_prompt_matrix/utils/validate_hours.py
--rw-rw-rw-   0        0        0      108 2021-08-02 19:25:47.000000 microt_prompt-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      731 2023-02-11 17:20:33.046031 microt_prompt-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-02-11 17:19:16.000000 microt_prompt-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-11 18:40:48.577122 microt_prompt-0.1.9/
+-rw-rw-rw-   0        0        0     1108 2021-08-02 19:35:31.000000 microt_prompt-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     7501 2023-02-11 18:40:48.578108 microt_prompt-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6848 2021-08-03 18:21:32.000000 microt_prompt-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-11 18:40:48.420144 microt_prompt-0.1.9/microt_prompt.egg-info/
+-rw-rw-rw-   0        0        0     7501 2023-02-11 18:40:48.000000 microt_prompt-0.1.9/microt_prompt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3275 2023-02-11 18:40:48.000000 microt_prompt-0.1.9/microt_prompt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-11 18:40:48.000000 microt_prompt-0.1.9/microt_prompt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-02-11 18:40:48.000000 microt_prompt-0.1.9/microt_prompt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-11 18:40:48.428112 microt_prompt-0.1.9/microt_prompt_matrix/
+-rw-rw-rw-   0        0        0       95 2021-08-03 14:21:25.000000 microt_prompt-0.1.9/microt_prompt_matrix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-11 18:40:48.477110 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/
+-rw-rw-rw-   0        0        0      470 2023-01-27 15:43:18.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/__init__.py
+-rw-rw-rw-   0        0        0     7614 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/battery_level.py
+-rw-rw-rw-   0        0        0      908 2023-01-26 14:17:21.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/compliance.py
+-rw-rw-rw-   0        0        0      790 2023-01-26 14:17:38.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/day_of_the_week.py
+-rw-rw-rw-   0        0        0     2164 2023-02-11 18:36:31.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/days_in_study.py
+-rw-rw-rw-   0        0        0     1327 2023-01-26 14:18:24.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/home_location.py
+-rw-rw-rw-   0        0        0    11103 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/location.py
+-rw-rw-rw-   0        0        0     2884 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/location_label.py
+-rw-rw-rw-   0        0        0    12601 2023-02-11 16:59:25.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/mims_summary.py
+-rw-rw-rw-   0        0        0     1935 2023-01-26 14:20:50.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/parts_of_waking_hour.py
+-rw-rw-rw-   0        0        0     7570 2023-02-11 18:37:32.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/phone_detected_activity.py
+-rw-rw-rw-   0        0        0     8688 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/phone_lock.py
+drwxrwxrwx   0        0        0        0 2023-02-11 18:40:48.485112 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/prompt_response/
+-rw-rw-rw-   0        0        0       84 2021-07-29 20:26:38.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/prompt_response/__init__.py
+-rw-rw-rw-   0        0        0     1977 2023-01-26 14:15:57.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/prompt_response/combine_appended_response.py
+-rw-rw-rw-   0        0        0    10559 2023-02-11 18:34:04.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/prompt_response/preprocess_promptResponse_raw.py
+-rw-rw-rw-   0        0        0     7666 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/screen_status.py
+-rw-rw-rw-   0        0        0      813 2023-01-26 14:21:57.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/study_mode.py
+-rw-rw-rw-   0        0        0     1147 2023-01-26 14:22:10.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/time_of_the_day.py
+-rw-rw-rw-   0        0        0     5814 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/waking_hours.py
+drwxrwxrwx   0        0        0        0 2023-02-11 18:40:48.533125 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/
+-rw-rw-rw-   0        0        0      431 2023-01-26 14:24:13.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/__init__.py
+-rw-rw-rw-   0        0        0     7610 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/battery_level.py
+-rw-rw-rw-   0        0        0      908 2023-01-26 14:25:11.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/compliance.py
+-rw-rw-rw-   0        0        0      790 2023-01-26 14:25:26.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/day_of_the_week.py
+-rw-rw-rw-   0        0        0     2113 2023-01-26 14:25:51.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/days_in_study.py
+-rw-rw-rw-   0        0        0     1327 2023-01-26 14:26:05.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/home_location.py
+-rw-rw-rw-   0        0        0    11122 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/location.py
+-rw-rw-rw-   0        0        0     2884 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/location_label.py
+-rw-rw-rw-   0        0        0     6456 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/mims_summary.py
+-rw-rw-rw-   0        0        0     1935 2023-01-26 14:28:29.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/parts_of_waking_hour.py
+-rw-rw-rw-   0        0        0     8687 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/phone_lock.py
+drwxrwxrwx   0        0        0        0 2023-02-11 18:40:48.542124 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/prompt_response/
+-rw-rw-rw-   0        0        0       84 2023-01-26 14:23:01.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/prompt_response/__init__.py
+-rw-rw-rw-   0        0        0     1977 2023-01-26 14:23:13.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/prompt_response/combine_appended_response.py
+-rw-rw-rw-   0        0        0     6606 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/prompt_response/preprocess_promptResponse_raw.py
+-rw-rw-rw-   0        0        0     7523 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/screen_status.py
+-rw-rw-rw-   0        0        0      815 2023-01-26 14:01:52.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/study_mode.py
+-rw-rw-rw-   0        0        0     1147 2023-01-26 14:30:23.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/time_of_the_day.py
+-rw-rw-rw-   0        0        0     6547 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/waking_hours.py
+-rw-rw-rw-   0        0        0     7084 2023-02-11 18:39:09.000000 microt_prompt-0.1.9/microt_prompt_matrix/main_ema.py
+-rw-rw-rw-   0        0        0     6690 2023-01-27 17:14:07.000000 microt_prompt-0.1.9/microt_prompt_matrix/main_uema.py
+drwxrwxrwx   0        0        0        0 2023-02-11 18:40:48.575108 microt_prompt-0.1.9/microt_prompt_matrix/utils/
+-rw-rw-rw-   0        0        0      306 2023-01-26 14:32:19.000000 microt_prompt-0.1.9/microt_prompt_matrix/utils/__init__.py
+-rw-rw-rw-   0        0        0     2130 2023-01-26 14:32:27.000000 microt_prompt-0.1.9/microt_prompt_matrix/utils/convert_timestamp.py
+-rw-rw-rw-   0        0        0      642 2023-01-26 14:32:36.000000 microt_prompt-0.1.9/microt_prompt_matrix/utils/extract_participant_id.py
+-rw-rw-rw-   0        0        0      908 2023-01-26 14:33:03.000000 microt_prompt-0.1.9/microt_prompt_matrix/utils/get_haversine_distance.py
+-rw-rw-rw-   0        0        0      154 2023-01-26 14:01:52.000000 microt_prompt-0.1.9/microt_prompt_matrix/utils/get_time_diff.py
+-rw-rw-rw-   0        0        0     4105 2023-01-26 14:33:19.000000 microt_prompt-0.1.9/microt_prompt_matrix/utils/home_coordinates.py
+-rw-rw-rw-   0        0        0     4964 2023-01-26 14:33:26.000000 microt_prompt-0.1.9/microt_prompt_matrix/utils/load_participant_study_info.py
+-rw-rw-rw-   0        0        0     1653 2023-01-26 14:33:34.000000 microt_prompt-0.1.9/microt_prompt_matrix/utils/parse_participants.py
+-rw-rw-rw-   0        0        0     1441 2023-01-26 14:33:41.000000 microt_prompt-0.1.9/microt_prompt_matrix/utils/uncompress_file.py
+-rw-rw-rw-   0        0        0     1351 2023-01-26 14:33:50.000000 microt_prompt-0.1.9/microt_prompt_matrix/utils/validate_date.py
+-rw-rw-rw-   0        0        0     1207 2023-01-26 14:33:59.000000 microt_prompt-0.1.9/microt_prompt_matrix/utils/validate_hours.py
+-rw-rw-rw-   0        0        0      108 2021-08-02 19:25:47.000000 microt_prompt-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      731 2023-02-11 18:40:48.580082 microt_prompt-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-02-11 18:34:21.000000 microt_prompt-0.1.9/setup.py
```

### Comparing `microt_prompt-0.1.8/LICENSE.txt` & `microt_prompt-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/PKG-INFO` & `microt_prompt-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microt_prompt
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package that transform intermediate log files into features of interest for analysis
 Home-page: https://bitbucket.org/mhealthresearchgroup/microt_compliance/src/master/
 Author: Jixin Li, Aditya Ponnada
 Author-email: li.jix@northeastern.edu
 Project-URL: Bug Tracker, https://bitbucket.org/mhealthresearchgroup/microt_compliance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `microt_prompt-0.1.8/README.md` & `microt_prompt-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt.egg-info/PKG-INFO` & `microt_prompt-0.1.9/microt_prompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microt-prompt
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package that transform intermediate log files into features of interest for analysis
 Home-page: https://bitbucket.org/mhealthresearchgroup/microt_compliance/src/master/
 Author: Jixin Li, Aditya Ponnada
 Author-email: li.jix@northeastern.edu
 Project-URL: Bug Tracker, https://bitbucket.org/mhealthresearchgroup/microt_compliance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `microt_prompt-0.1.8/microt_prompt.egg-info/SOURCES.txt` & `microt_prompt-0.1.9/microt_prompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/battery_level.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/battery_level.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/compliance.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/compliance.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/day_of_the_week.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/day_of_the_week.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/days_in_study.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/days_in_study.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,13 +33,15 @@
         if "start_date" in info_dict[participant_id]:
             start_date = info_dict[participant_id]["start_date"]
             start_date_dateobject = datetime.strptime(start_date, "%Y-%m-%d").date()
         else:
             raise Exception(
                 "Don't find this participant in info json. Check if this participant has daily report, and delete Misc and rerun the code. ")
 
-
-    prompt_dateobject_date_series = df_prompt_combined.Actual_Prompt_Local_DateTime.dt.date
+    try:
+        prompt_dateobject_date_series = df_prompt_combined.Actual_Prompt_Local_DateTime.dt.date
+    except AttributeError:
+        raise AttributeError("AttributeError : {} - {}".format(participant_id, df_prompt_combined.Actual_Prompt_Local_DateTime))
 
     days_in_study = prompt_dateobject_date_series.apply(lambda x: calculate_daysInStudy(x, start_date_dateobject))
 
     return days_in_study
```

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/home_location.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/home_location.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/location.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/location.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/location_label.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/location_label.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/mims_summary.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/mims_summary.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/parts_of_waking_hour.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/parts_of_waking_hour.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/phone_detected_activity.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/phone_detected_activity.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 
 def clean_dataframe(df):
     df.reset_index(inplace=True, drop=True)
     dropped_rows = []
     for idx in df.index:
         local_time_str = df["LOG_TIME"][idx]
-        if (local_time_str == "-1") or len(local_time_str.split(' ')) > 3 or len(
+        if (local_time_str == "-1") or ("-1 " in local_time_str) or len(local_time_str.split(' ')) > 3 or len(
                 local_time_str.split('-')[0]) > 4 or len(local_time_str.split(' ')) < 2:
             dropped_rows.append(idx)
     df = df.drop(dropped_rows)
 
     df.reset_index(inplace=True, drop=True)
     return df
 
@@ -125,19 +125,22 @@
             closest_time = "NF"
         else:
             subset_time_list = list(df_logs_combined["Local_Timestamp"])
 
             closest_time = find_closest_time(prompt_time, subset_time_list)
 
             # check if matched time is 5 minutes away from prompt time
-            if get_min_diff(prompt_time, closest_time) < 5:
-                detected_activity = list(df_logs_combined[df_logs_combined['Local_Timestamp'] == closest_time][
-                                             detected_activity_columns].idxmax(axis=1))[0]
-            else:
-                detected_activity = "NF"
+            # if get_min_diff(prompt_time, closest_time) < 5:
+            df_closest = df_logs_combined[df_logs_combined['Local_Timestamp'] == closest_time][
+                detected_activity_columns]
+            #             detected_activity = list(df_closest.idxmax(axis=1))[0]
+            detected_activity = \
+            list(df_closest.eq(df_closest.max(1), axis=0).dot(df_closest.columns + ',').str.rstrip(','))[0]
+            # else:
+            #     detected_activity = "NF"
 
         matched_time_list.append(closest_time)
         detected_activity_list.append(detected_activity)
 
     return detected_activity_list, matched_time_list
```

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/phone_lock.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/phone_lock.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/prompt_response/combine_appended_response.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/prompt_response/combine_appended_response.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/prompt_response/preprocess_promptResponse_raw.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/prompt_response/preprocess_promptResponse_raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import sys
 
 import pandas.errors
 
 from microt_prompt_matrix.utils.convert_timestamp import *
 from glob import glob
 
-columns_list = ["Participant_ID", "Initial_Prompt_Date", "Line", "Prompt_Type", "Study_Mode", "Initial_Prompt_Local_Time", "Initial_Prompt_UnixTime",
+columns_list = ["Participant_ID", "Initial_Prompt_Date", "Prompt_Type", "Study_Mode", "Initial_Prompt_Local_Time", "Initial_Prompt_UnixTime",
                 "Initial_Prompt_UTC_Offset ",
                 "Answer_Status", 'Question_Set_Completion_Local_Time', 'Question_Set_Completion_UnixTime',
                 'Reprompt1_Prompt_Date',
                 'Reprompt1_Prompt_Local_Time', 'Reprompt1_Prompt_UnixTime',
                 'Reprompt2_Prompt_Date', 'Reprompt2_Prompt_Local_Time',
                 'Reprompt2_Prompt_UnixTime ', 'Reprompt3_Prompt_Date',
                 'Reprompt3_Prompt_Local_Time', 'Reprompt3_Prompt_UnixTime',
@@ -179,15 +179,15 @@
     df_reprompt = extract_reprompt(df_raw)
 
     if df_reprompt.shape[0] == 0:
         print("Empty prompt response file after filtering : " + csv_path[0])
         quit()
 
     # add participant id column
-    df_reprompt.insert(loc=0, column='Participant_ID', value=participant_id)
+    # df_reprompt.insert(loc=0, column='Participant_ID', value=participant_id)
 
     # time zone processing
     df_reprompt.reset_index(drop=True, inplace=True)
     Prompt_Local_Time_list = []
     for idx in df_reprompt.index:
         prompt_local_time_timezone = df_reprompt['Actual_Prompt_Local_Time'][idx]
         prompt_local_time_timezone_split = prompt_local_time_timezone.split(" ")
```

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/screen_status.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/screen_status.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/study_mode.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/study_mode.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/time_of_the_day.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/time_of_the_day.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_ema/waking_hours.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/waking_hours.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/battery_level.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/battery_level.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/compliance.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/compliance.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/day_of_the_week.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/day_of_the_week.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/days_in_study.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_ema/days_in_study.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Output: 1) a list of targeted features for the participant 2) print stats of the targeted features for the participant
 """
 
 from datetime import datetime
-
+import numpy as np
 
 
 def calculate_daysInStudy(prompte_date, start_date):
     delta = prompte_date - start_date
     return delta
 
+
 # def get_start_date_dict():
 #     # change to your path of combined_report.csv
 #     combined_report_path = r"E:\compliance_analysis\report\combined_report.csv"
 #     df_report = pd.read_csv(combined_report_path)
 #     participants_list = df_report['participant_ID'].unique()
 #     date_format = '%m/%d/%Y'
 #     start_date_dict = {}
@@ -22,26 +23,25 @@
 #         start_date = datetime.strptime(start_date_str, date_format).date()
 #         start_date_dict[p_id] = start_date
 #     return start_date_dict
 
 def create_column(df_prompt_combined, info_dict, print_stats=True):
     print("\n> start generating the feature: days in study ")
     participant_id = df_prompt_combined['Participant_ID'][0]
+    series_len = len(df_prompt_combined.Actual_Prompt_Local_DateTime)
 
     if participant_id not in info_dict:
-        raise Exception("Don't find this participant in info json. Check if this participant has data, and delete Misc and rerun the code. ")
+        # raise Exception("Don't find this participant in info json. Check if this participant has data, and delete Misc and rerun the code. ")
+        days_in_study = [np.nan] * series_len
     else:
         if "start_date" in info_dict[participant_id]:
             start_date = info_dict[participant_id]["start_date"]
             start_date_dateobject = datetime.strptime(start_date, "%Y-%m-%d").date()
+            prompt_dateobject_date_series = df_prompt_combined.Actual_Prompt_Local_DateTime.dt.date
+            days_in_study = prompt_dateobject_date_series.apply(
+                lambda x: calculate_daysInStudy(x, start_date_dateobject))
         else:
-            raise Exception(
-                "Don't find this participant in info json. Check if this participant has daily report, and delete Misc and rerun the code. ")
-
-    try:
-        prompt_dateobject_date_series = df_prompt_combined.Actual_Prompt_Local_DateTime.dt.date
-    except AttributeError:
-        raise AttributeError("AttributeError : {} - {}".format(participant_id, df_prompt_combined.Actual_Prompt_Local_DateTime))
-
-    days_in_study = prompt_dateobject_date_series.apply(lambda x: calculate_daysInStudy(x, start_date_dateobject))
+            days_in_study = [np.nan] * series_len
+            # raise Exception(
+            # "Don't find this participant in info json. Check if this participant has daily report, and delete Misc and rerun the code. ")
 
-    return days_in_study
+    return days_in_study
```

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/home_location.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/home_location.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/location.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/location.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/location_label.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/location_label.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/mims_summary.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/mims_summary.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/parts_of_waking_hour.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/parts_of_waking_hour.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/phone_lock.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/phone_lock.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/prompt_response/combine_appended_response.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/prompt_response/combine_appended_response.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/prompt_response/preprocess_promptResponse_raw.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/prompt_response/preprocess_promptResponse_raw.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/screen_status.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/screen_status.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/study_mode.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/study_mode.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/time_of_the_day.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/time_of_the_day.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/feature_engineering_uema/waking_hours.py` & `microt_prompt-0.1.9/microt_prompt_matrix/feature_engineering_uema/waking_hours.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/main_ema.py` & `microt_prompt-0.1.9/microt_prompt_matrix/main_ema.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,17 +122,18 @@
 
     # - feature 14: MIMS Summary
     df_mims = feature_engineering_ema.mims_summary.create_column(df_prompt['Actual_Prompt_Local_DateTime'],
                                                                  intermediate_participant_path, date_in_study)
     feature_df = pd.concat([feature_df, df_mims], axis=1)
 
     # - feature 15: Phone Detected Activity
-    feature17 = feature_engineering_ema.phone_detected_activity.create_column(df_prompt['Actual_Prompt_Local_DateTime'],
+    feature17, matchtime = feature_engineering_ema.phone_detected_activity.create_column(df_prompt['Actual_Prompt_Local_DateTime'],
                                                                  intermediate_participant_path, date_in_study)
     feature_df['PHONE_DETECTED_ACTIVITY'] = feature17
+    feature_df['PHONE_DETECTED_ACTIVITY_MATCHTIME'] = matchtime
 
     # save
     feature_df.to_csv(csv_save_path, index=False)
 
     return
```

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/main_uema.py` & `microt_prompt-0.1.9/microt_prompt_matrix/main_uema.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/utils/convert_timestamp.py` & `microt_prompt-0.1.9/microt_prompt_matrix/utils/convert_timestamp.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/utils/extract_participant_id.py` & `microt_prompt-0.1.9/microt_prompt_matrix/utils/extract_participant_id.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/utils/get_haversine_distance.py` & `microt_prompt-0.1.9/microt_prompt_matrix/utils/get_haversine_distance.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/utils/home_coordinates.py` & `microt_prompt-0.1.9/microt_prompt_matrix/utils/home_coordinates.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/utils/load_participant_study_info.py` & `microt_prompt-0.1.9/microt_prompt_matrix/utils/load_participant_study_info.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/utils/parse_participants.py` & `microt_prompt-0.1.9/microt_prompt_matrix/utils/parse_participants.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/utils/uncompress_file.py` & `microt_prompt-0.1.9/microt_prompt_matrix/utils/uncompress_file.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/utils/validate_date.py` & `microt_prompt-0.1.9/microt_prompt_matrix/utils/validate_date.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/microt_prompt_matrix/utils/validate_hours.py` & `microt_prompt-0.1.9/microt_prompt_matrix/utils/validate_hours.py`

 * *Files identical despite different names*

### Comparing `microt_prompt-0.1.8/setup.cfg` & `microt_prompt-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6963 726f 745f 7072 6f6d 7074   = microt_prompt
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
-00000030: 380d 0a61 7574 686f 7220 3d20 4a69 7869  8..author = Jixi
+00000030: 390d 0a61 7574 686f 7220 3d20 4a69 7869  9..author = Jixi
 00000040: 6e20 4c69 2c20 4164 6974 7961 2050 6f6e  n Li, Aditya Pon
 00000050: 6e61 6461 0d0a 6175 7468 6f72 5f65 6d61  nada..author_ema
 00000060: 696c 203d 206c 692e 6a69 7840 6e6f 7274  il = li.jix@nort
 00000070: 6865 6173 7465 726e 2e65 6475 0d0a 6465  heastern.edu..de
 00000080: 7363 7269 7074 696f 6e20 3d20 4120 7061  scription = A pa
 00000090: 636b 6167 6520 7468 6174 2074 7261 6e73  ckage that trans
 000000a0: 666f 726d 2069 6e74 6572 6d65 6469 6174  form intermediat
```

### Comparing `microt_prompt-0.1.8/setup.py` & `microt_prompt-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name='microt_prompt',
-    version="0.1.8",
+    version="0.1.9",
     description='A package that transform intermediate log files into features of interest for analysis',
     url='https://bitbucket.org/mhealthresearchgroup/microt_compliance/src/master/',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Jixin Li, Aditya Ponnada',
     author_email='li.jix@northeastern.edu',
     classifiers=[
```

