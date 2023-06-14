# Comparing `tmp/cfl-common-6.8.9.tar.gz` & `tmp/cfl-common-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cfl-common-6.8.9.tar", last modified: Tue Jun 21 09:04:28 2022, max compression
+gzip compressed data, was "dist/cfl-common-6.9.0.tar", last modified: Thu Jun 23 09:40:51 2022, max compression
```

## Comparing `cfl-common-6.8.9.tar` & `cfl-common-6.9.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/
--rw-r--r--   0 runner    (1001) docker     (116)       74 2022-06-21 09:00:15.000000 cfl-common-6.8.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      211 2022-06-21 09:04:28.000000 cfl-common-6.8.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/cfl_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      211 2022-06-21 09:04:28.000000 cfl-common-6.8.9/cfl_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2271 2022-06-21 09:04:28.000000 cfl-common-6.8.9/cfl_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-21 09:04:28.000000 cfl-common-6.8.9/cfl_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       98 2022-06-21 09:04:28.000000 cfl-common-6.8.9/cfl_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-06-21 09:04:28.000000 cfl-common-6.8.9/cfl_common.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/common/
--rw-r--r--   0 runner    (1001) docker     (116)       48 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2521 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (116)      129 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/apps.py
--rw-r--r--   0 runner    (1001) docker     (116)      236 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (116)     6932 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/email_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/common/fixtures/
--rw-r--r--   0 runner    (1001) docker     (116)     1234 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/fixtures/aimmo_characters.json
--rw-r--r--   0 runner    (1001) docker     (116)     1285 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/fixtures/aimmo_characters2.json
--rw-r--r--   0 runner    (1001) docker     (116)     1392 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/fixtures/aimmo_characters3.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1778 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/helpers/data_migration_loader.py
--rw-r--r--   0 runner    (1001) docker     (116)     9620 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/helpers/emails.py
--rw-r--r--   0 runner    (1001) docker     (116)     1505 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/helpers/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/common/migrations/
--rw-r--r--   0 runner    (1001) docker     (116)     9664 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0002_emailverification.py
--rw-r--r--   0 runner    (1001) docker     (116)      922 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0003_aimmocharacter.py
--rw-r--r--   0 runner    (1001) docker     (116)      430 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0004_add_aimmocharacters.py
--rw-r--r--   0 runner    (1001) docker     (116)      412 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0005_add_worksheets.py
--rw-r--r--   0 runner    (1001) docker     (116)      431 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0006_update_aimmo_character_image_path.py
--rw-r--r--   0 runner    (1001) docker     (116)      431 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0007_add_pdf_names_to_first_two_worksheets.py
--rw-r--r--   0 runner    (1001) docker     (116)      381 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0008_unlock_worksheet_3.py
--rw-r--r--   0 runner    (1001) docker     (116)      599 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0009_add_blocked_time_to_teacher_and_student.py
--rw-r--r--   0 runner    (1001) docker     (116)      396 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0010_remove_teacher_title.py
--rw-r--r--   0 runner    (1001) docker     (116)      400 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0011_student_login_id.py
--rw-r--r--   0 runner    (1001) docker     (116)     1135 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0012_usersession.py
--rw-r--r--   0 runner    (1001) docker     (116)     1142 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0013_class_school.py
--rw-r--r--   0 runner    (1001) docker     (116)      817 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0014_login_type.py
--rw-r--r--   0 runner    (1001) docker     (116)      901 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0015_dailyactivity.py
--rw-r--r--   0 runner    (1001) docker     (116)     1208 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0016_joinreleasestudent.py
--rw-r--r--   0 runner    (1001) docker     (116)      637 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0017_copy_email_to_username.py
--rw-r--r--   0 runner    (1001) docker     (116)      387 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0018_update_aimmo_character_image_path.py
--rw-r--r--   0 runner    (1001) docker     (116)      418 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0019_aimmocharacter_alt.py
--rw-r--r--   0 runner    (1001) docker     (116)      555 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0020_class_is_active_and_null_access_code.py
--rw-r--r--   0 runner    (1001) docker     (116)      736 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0021_school_is_active.py
--rw-r--r--   0 runner    (1001) docker     (116)      661 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0022_school_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (116)      515 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/0023_userprofile_aimmo_badges.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11280 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/models.py
--rw-r--r--   0 runner    (1001) docker     (116)     1991 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/common/static/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/common/static/common/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/common/static/common/img/
--rw-r--r--   0 runner    (1001) docker     (116)   557149 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/static/common/img/RR_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/common/templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/common/templates/common/
--rw-r--r--   0 runner    (1001) docker     (116)      336 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/templates/common/freshdesk_widget.html
--rw-r--r--   0 runner    (1001) docker     (116)     1077 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/templates/common/onetrust_cookies_consent_notice.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/common/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1093 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/test_migration_aimmo_characters.py
--rw-r--r--   0 runner    (1001) docker     (116)      652 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/test_migration_blocked_time.py
--rw-r--r--   0 runner    (1001) docker     (116)      536 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/test_migration_remove_teacher_title.py
--rw-r--r--   0 runner    (1001) docker     (116)     2983 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-21 09:04:28.000000 cfl-common-6.8.9/common/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1100 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/utils/classes.py
--rw-r--r--   0 runner    (1001) docker     (116)     2961 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (116)     1123 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/utils/organisation.py
--rw-r--r--   0 runner    (1001) docker     (116)     4290 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/utils/student.py
--rw-r--r--   0 runner    (1001) docker     (116)     2386 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/utils/teacher.py
--rw-r--r--   0 runner    (1001) docker     (116)      941 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/tests/utils/user.py
--rw-r--r--   0 runner    (1001) docker     (116)     1727 2022-06-21 09:00:15.000000 cfl-common-6.8.9/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      100 2022-06-21 09:00:15.000000 cfl-common-6.8.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-06-21 09:04:28.000000 cfl-common-6.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      692 2022-06-21 09:00:15.000000 cfl-common-6.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:51.000000 cfl-common-6.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)       74 2022-06-23 09:37:43.000000 cfl-common-6.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      211 2022-06-23 09:40:51.000000 cfl-common-6.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:50.000000 cfl-common-6.9.0/cfl_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      211 2022-06-23 09:40:50.000000 cfl-common-6.9.0/cfl_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2271 2022-06-23 09:40:50.000000 cfl-common-6.9.0/cfl_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-23 09:40:50.000000 cfl-common-6.9.0/cfl_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       98 2022-06-23 09:40:50.000000 cfl-common-6.9.0/cfl_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2022-06-23 09:40:50.000000 cfl-common-6.9.0/cfl_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:50.000000 cfl-common-6.9.0/common/
+-rw-r--r--   0 runner    (1001) docker     (116)       48 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2521 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)      129 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/apps.py
+-rw-r--r--   0 runner    (1001) docker     (116)      236 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6932 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/email_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:50.000000 cfl-common-6.9.0/common/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (116)     1234 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/fixtures/aimmo_characters.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1285 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/fixtures/aimmo_characters2.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1392 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/fixtures/aimmo_characters3.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:50.000000 cfl-common-6.9.0/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1778 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/helpers/data_migration_loader.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9620 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/helpers/emails.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1505 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/helpers/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:51.000000 cfl-common-6.9.0/common/migrations/
+-rw-r--r--   0 runner    (1001) docker     (116)     9664 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2156 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/migrations/0002_emailverification.py
+-rw-r--r--   0 runner    (1001) docker     (116)      922 2022-06-23 09:37:43.000000 cfl-common-6.9.0/common/migrations/0003_aimmocharacter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      430 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0004_add_aimmocharacters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      412 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0005_add_worksheets.py
+-rw-r--r--   0 runner    (1001) docker     (116)      431 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0006_update_aimmo_character_image_path.py
+-rw-r--r--   0 runner    (1001) docker     (116)      431 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0007_add_pdf_names_to_first_two_worksheets.py
+-rw-r--r--   0 runner    (1001) docker     (116)      381 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0008_unlock_worksheet_3.py
+-rw-r--r--   0 runner    (1001) docker     (116)      599 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0009_add_blocked_time_to_teacher_and_student.py
+-rw-r--r--   0 runner    (1001) docker     (116)      396 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0010_remove_teacher_title.py
+-rw-r--r--   0 runner    (1001) docker     (116)      400 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0011_student_login_id.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1135 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0012_usersession.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1142 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0013_class_school.py
+-rw-r--r--   0 runner    (1001) docker     (116)      817 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0014_login_type.py
+-rw-r--r--   0 runner    (1001) docker     (116)      901 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0015_dailyactivity.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1208 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0016_joinreleasestudent.py
+-rw-r--r--   0 runner    (1001) docker     (116)      637 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0017_copy_email_to_username.py
+-rw-r--r--   0 runner    (1001) docker     (116)      387 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0018_update_aimmo_character_image_path.py
+-rw-r--r--   0 runner    (1001) docker     (116)      418 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0019_aimmocharacter_alt.py
+-rw-r--r--   0 runner    (1001) docker     (116)      555 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0020_class_is_active_and_null_access_code.py
+-rw-r--r--   0 runner    (1001) docker     (116)      736 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0021_school_is_active.py
+-rw-r--r--   0 runner    (1001) docker     (116)      661 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0022_school_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (116)      515 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/0023_userprofile_aimmo_badges.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11280 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1991 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:50.000000 cfl-common-6.9.0/common/static/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:50.000000 cfl-common-6.9.0/common/static/common/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:51.000000 cfl-common-6.9.0/common/static/common/img/
+-rw-r--r--   0 runner    (1001) docker     (116)   557149 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/static/common/img/RR_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:50.000000 cfl-common-6.9.0/common/templates/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:51.000000 cfl-common-6.9.0/common/templates/common/
+-rw-r--r--   0 runner    (1001) docker     (116)      336 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/templates/common/freshdesk_widget.html
+-rw-r--r--   0 runner    (1001) docker     (116)     1077 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/templates/common/onetrust_cookies_consent_notice.html
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:51.000000 cfl-common-6.9.0/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1093 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/test_migration_aimmo_characters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      652 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/test_migration_blocked_time.py
+-rw-r--r--   0 runner    (1001) docker     (116)      536 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/test_migration_remove_teacher_title.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2983 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-23 09:40:51.000000 cfl-common-6.9.0/common/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1100 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/utils/classes.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2961 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1123 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/utils/organisation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4290 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/utils/student.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2386 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/utils/teacher.py
+-rw-r--r--   0 runner    (1001) docker     (116)      941 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/tests/utils/user.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1727 2022-06-23 09:37:44.000000 cfl-common-6.9.0/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      100 2022-06-23 09:37:44.000000 cfl-common-6.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-06-23 09:40:51.000000 cfl-common-6.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      692 2022-06-23 09:37:44.000000 cfl-common-6.9.0/setup.py
```

### Comparing `cfl-common-6.8.9/cfl_common.egg-info/SOURCES.txt` & `cfl-common-6.9.0/cfl_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/app_settings.py` & `cfl-common-6.9.0/common/app_settings.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/email_messages.py` & `cfl-common-6.9.0/common/email_messages.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/fixtures/aimmo_characters.json` & `cfl-common-6.9.0/common/fixtures/aimmo_characters.json`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/fixtures/aimmo_characters2.json` & `cfl-common-6.9.0/common/fixtures/aimmo_characters2.json`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/fixtures/aimmo_characters3.json` & `cfl-common-6.9.0/common/fixtures/aimmo_characters3.json`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/helpers/data_migration_loader.py` & `cfl-common-6.9.0/common/helpers/data_migration_loader.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/helpers/emails.py` & `cfl-common-6.9.0/common/helpers/emails.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/helpers/generators.py` & `cfl-common-6.9.0/common/helpers/generators.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0001_initial.py` & `cfl-common-6.9.0/common/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0002_emailverification.py` & `cfl-common-6.9.0/common/migrations/0002_emailverification.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0003_aimmocharacter.py` & `cfl-common-6.9.0/common/migrations/0003_aimmocharacter.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0009_add_blocked_time_to_teacher_and_student.py` & `cfl-common-6.9.0/common/migrations/0009_add_blocked_time_to_teacher_and_student.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0012_usersession.py` & `cfl-common-6.9.0/common/migrations/0012_usersession.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0013_class_school.py` & `cfl-common-6.9.0/common/migrations/0013_class_school.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0014_login_type.py` & `cfl-common-6.9.0/common/migrations/0014_login_type.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0015_dailyactivity.py` & `cfl-common-6.9.0/common/migrations/0015_dailyactivity.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0016_joinreleasestudent.py` & `cfl-common-6.9.0/common/migrations/0016_joinreleasestudent.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0017_copy_email_to_username.py` & `cfl-common-6.9.0/common/migrations/0017_copy_email_to_username.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0020_class_is_active_and_null_access_code.py` & `cfl-common-6.9.0/common/migrations/0020_class_is_active_and_null_access_code.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0021_school_is_active.py` & `cfl-common-6.9.0/common/migrations/0021_school_is_active.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0022_school_cleanup.py` & `cfl-common-6.9.0/common/migrations/0022_school_cleanup.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/migrations/0023_userprofile_aimmo_badges.py` & `cfl-common-6.9.0/common/migrations/0023_userprofile_aimmo_badges.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/models.py` & `cfl-common-6.9.0/common/models.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/permissions.py` & `cfl-common-6.9.0/common/permissions.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/static/common/img/RR_logo.svg` & `cfl-common-6.9.0/common/static/common/img/RR_logo.svg`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/templates/common/onetrust_cookies_consent_notice.html` & `cfl-common-6.9.0/common/templates/common/onetrust_cookies_consent_notice.html`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/tests/test_migration_aimmo_characters.py` & `cfl-common-6.9.0/common/tests/test_migration_aimmo_characters.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/tests/test_migration_blocked_time.py` & `cfl-common-6.9.0/common/tests/test_migration_blocked_time.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/tests/test_migration_remove_teacher_title.py` & `cfl-common-6.9.0/common/tests/test_migration_remove_teacher_title.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/tests/test_models.py` & `cfl-common-6.9.0/common/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/tests/utils/classes.py` & `cfl-common-6.9.0/common/tests/utils/classes.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/tests/utils/email.py` & `cfl-common-6.9.0/common/tests/utils/email.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/tests/utils/organisation.py` & `cfl-common-6.9.0/common/tests/utils/organisation.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/tests/utils/student.py` & `cfl-common-6.9.0/common/tests/utils/student.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/tests/utils/teacher.py` & `cfl-common-6.9.0/common/tests/utils/teacher.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/tests/utils/user.py` & `cfl-common-6.9.0/common/tests/utils/user.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/common/utils.py` & `cfl-common-6.9.0/common/utils.py`

 * *Files identical despite different names*

### Comparing `cfl-common-6.8.9/setup.py` & `cfl-common-6.9.0/setup.py`

 * *Files identical despite different names*

