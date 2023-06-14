# Comparing `tmp/nobinobi-staff-0.1.6.7.tar.gz` & `tmp/nobinobi-staff-0.1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nobinobi-staff-0.1.6.7.tar", last modified: Wed Dec 22 14:22:31 2021, max compression
+gzip compressed data, was "dist\nobinobi-staff-0.1.6.8.tar", last modified: Thu Dec 23 10:39:28 2021, max compression
```

## Comparing `nobinobi-staff-0.1.6.7.tar` & `nobinobi-staff-0.1.6.8.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/
--rw-rw-rw-   0        0        0      153 2020-10-29 12:35:37.000000 nobinobi-staff-0.1.6.7/AUTHORS.rst
--rw-rw-rw-   0        0        0     3373 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     2381 2021-12-22 14:21:19.000000 nobinobi-staff-0.1.6.7/HISTORY.rst
--rw-rw-rw-   0        0        0    31774 2020-10-29 12:40:58.000000 nobinobi-staff-0.1.6.7/LICENSE
--rw-rw-rw-   0        0        0      248 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/MANIFEST.in
--rw-rw-rw-   0        0        0     6704 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/README.rst
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/
--rw-rw-rw-   0        0        0      684 2021-12-22 14:21:19.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/__init__.py
--rw-rw-rw-   0        0        0    10338 2021-12-22 14:21:19.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/admin.py
--rw-rw-rw-   0        0        0     1905 2021-09-17 09:46:04.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/apps.py
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/fixtures/
--rw-rw-rw-   0        0        0     1981 2020-09-01 10:41:02.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/fixtures/staff_absence_type_en-US.json
--rw-rw-rw-   0        0        0     2138 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/fixtures/staff_absence_type_fr-CH.json
--rw-rw-rw-   0        0        0     3742 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/forms.py
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/de/
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0      442 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/de/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/en/
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      399 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/en/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/fr/
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     5594 2021-09-17 09:46:04.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/fr/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/fr_CH/
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/fr_CH/LC_MESSAGES/
--rw-rw-rw-   0        0        0     5357 2021-09-17 10:45:02.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/fr_CH/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/it/
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/it/LC_MESSAGES/
--rw-rw-rw-   0        0        0      442 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/locale/it/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/management/
--rw-rw-rw-   0        0        0      748 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/management/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/management/commands/
--rw-rw-rw-   0        0        0      748 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/management/commands/__init__.py
--rw-rw-rw-   0        0        0     3241 2021-09-29 10:43:25.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/management/commands/generate_training.py
--rw-rw-rw-   0        0        0     4647 2021-09-29 10:43:25.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/management/commands/update_training.py
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/
--rw-rw-rw-   0        0        0     5934 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     4150 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0002_auto_20181019_1017.py
--rw-rw-rw-   0        0        0     1602 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0003_auto_20181022_1101.py
--rw-rw-rw-   0        0        0     1201 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0004_team_order.py
--rw-rw-rw-   0        0        0     1553 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0005_auto_20181116_0815.py
--rw-rw-rw-   0        0        0     1194 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0006_staff_working_base.py
--rw-rw-rw-   0        0        0     3775 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0007_auto_20200221_1138.py
--rw-rw-rw-   0        0        0     1349 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0008_add_partial_disability.py
--rw-rw-rw-   0        0        0     1374 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0009_auto_20200805_1143.py
--rw-rw-rw-   0        0        0     2794 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0010_auto_20201029_1500.py
--rw-rw-rw-   0        0        0      593 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/__init__.py
--rw-rw-rw-   0        0        0    12677 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/models.py
--rw-rw-rw-   0        0        0     1067 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/serializers.py
--rw-rw-rw-   0        0        0     4194 2021-09-17 09:46:04.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/signals.py
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/static/
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/static/css/
--rw-rw-rw-   0        0        0      761 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/static/css/nobinobi_staff.css
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/static/js/
--rw-rw-rw-   0        0        0      761 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/static/js/nobinobi_staff.js
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/templates/
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/templates/staff/
--rw-rw-rw-   0        0        0     1530 2020-09-01 10:41:03.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/templates/staff/staff_list_readonly.html
--rw-rw-rw-   0        0        0      777 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/tests.py
--rw-rw-rw-   0        0        0     1784 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/urls.py
--rw-rw-rw-   0        0        0     1796 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.7/nobinobi_staff/views.py
-drwxrwxrwx   0        0        0        0 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff.egg-info/
--rw-rw-rw-   0        0        0     6704 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1864 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      331 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/nobinobi_staff.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      344 2021-12-22 14:21:19.000000 nobinobi-staff-0.1.6.7/requirements.txt
--rw-rw-rw-   0        0        0      789 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.7/requirements_dev.txt
--rw-rw-rw-   0        0        0      132 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.7/requirements_test.txt
--rw-rw-rw-   0        0        0      281 2021-12-22 14:22:31.000000 nobinobi-staff-0.1.6.7/setup.cfg
--rw-rw-rw-   0        0        0     2282 2021-04-13 08:49:29.000000 nobinobi-staff-0.1.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/
+-rw-rw-rw-   0        0        0      153 2020-10-29 12:35:37.000000 nobinobi-staff-0.1.6.8/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3373 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     2543 2021-12-23 10:38:19.000000 nobinobi-staff-0.1.6.8/HISTORY.rst
+-rw-rw-rw-   0        0        0    31774 2020-10-29 12:40:58.000000 nobinobi-staff-0.1.6.8/LICENSE
+-rw-rw-rw-   0        0        0      248 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     6914 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2053 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/README.rst
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/
+-rw-rw-rw-   0        0        0      684 2021-12-23 10:38:19.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/__init__.py
+-rw-rw-rw-   0        0        0    10581 2021-12-23 10:38:17.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/admin.py
+-rw-rw-rw-   0        0        0     1905 2021-09-17 09:46:04.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/apps.py
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/fixtures/
+-rw-rw-rw-   0        0        0     1981 2020-09-01 10:41:02.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/fixtures/staff_absence_type_en-US.json
+-rw-rw-rw-   0        0        0     2138 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/fixtures/staff_absence_type_fr-CH.json
+-rw-rw-rw-   0        0        0     3742 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/forms.py
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/de/
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      442 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/de/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/en/
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      399 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/en/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr/
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     5594 2021-09-17 09:46:04.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr_CH/
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr_CH/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     5357 2021-09-17 10:45:02.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr_CH/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/it/
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      442 2021-03-12 09:31:05.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/locale/it/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/
+-rw-rw-rw-   0        0        0      748 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/__init__.py
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/
+-rw-rw-rw-   0        0        0      748 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     3241 2021-09-29 10:43:25.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/generate_training.py
+-rw-rw-rw-   0        0        0     4647 2021-09-29 10:43:25.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/update_training.py
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/
+-rw-rw-rw-   0        0        0     5934 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     4150 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0002_auto_20181019_1017.py
+-rw-rw-rw-   0        0        0     1602 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0003_auto_20181022_1101.py
+-rw-rw-rw-   0        0        0     1201 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0004_team_order.py
+-rw-rw-rw-   0        0        0     1553 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0005_auto_20181116_0815.py
+-rw-rw-rw-   0        0        0     1194 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0006_staff_working_base.py
+-rw-rw-rw-   0        0        0     3775 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0007_auto_20200221_1138.py
+-rw-rw-rw-   0        0        0     1349 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0008_add_partial_disability.py
+-rw-rw-rw-   0        0        0     1374 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0009_auto_20200805_1143.py
+-rw-rw-rw-   0        0        0     2794 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0010_auto_20201029_1500.py
+-rw-rw-rw-   0        0        0      593 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/__init__.py
+-rw-rw-rw-   0        0        0    12677 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/models.py
+-rw-rw-rw-   0        0        0     1067 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/serializers.py
+-rw-rw-rw-   0        0        0     4305 2021-12-23 10:38:17.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/signals.py
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/static/
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/static/css/
+-rw-rw-rw-   0        0        0      761 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/static/css/nobinobi_staff.css
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/static/js/
+-rw-rw-rw-   0        0        0      761 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/static/js/nobinobi_staff.js
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/templates/
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/templates/staff/
+-rw-rw-rw-   0        0        0     1530 2020-09-01 10:41:03.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/templates/staff/staff_list_readonly.html
+-rw-rw-rw-   0        0        0      777 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/tests.py
+-rw-rw-rw-   0        0        0     1784 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/urls.py
+-rw-rw-rw-   0        0        0     1796 2020-10-29 14:51:49.000000 nobinobi-staff-0.1.6.8/nobinobi_staff/views.py
+drwxrwxrwx   0        0        0        0 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/
+-rw-rw-rw-   0        0        0     6914 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1864 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      331 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      344 2021-12-22 14:21:19.000000 nobinobi-staff-0.1.6.8/requirements.txt
+-rw-rw-rw-   0        0        0      789 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.8/requirements_dev.txt
+-rw-rw-rw-   0        0        0      132 2021-12-14 10:57:24.000000 nobinobi-staff-0.1.6.8/requirements_test.txt
+-rw-rw-rw-   0        0        0      281 2021-12-23 10:39:28.000000 nobinobi-staff-0.1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     2282 2021-04-13 08:49:29.000000 nobinobi-staff-0.1.6.8/setup.py
```

### Comparing `nobinobi-staff-0.1.6.7/CONTRIBUTING.rst` & `nobinobi-staff-0.1.6.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/HISTORY.rst` & `nobinobi-staff-0.1.6.8/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 History
 -------
 
+0.1.6.8 (2021-12-23)
+++++++++++++++++++++++
+
+* 879490a - filter on choice staff absence only active staff
+* d04ba24 - Fix bug when save staff for training
+
 0.1.6.7 (2021-12-22)
 ++++++++++++++++++++++
 
 * c19f6cb - Filter by default to staff active in list admin
 * dd97bda - Fix requirements
 
 0.1.6.6 (2021-12-14)
```

### Comparing `nobinobi-staff-0.1.6.7/LICENSE` & `nobinobi-staff-0.1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/PKG-INFO` & `nobinobi-staff-0.1.6.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nobinobi-staff
-Version: 0.1.6.7
+Version: 0.1.6.8
 Summary: Application staff for nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-staff
 Author: Florian Alu
 Author-email: alu@prolibre.com
 License: UNKNOWN
 Description: =============================
         Nobinobi Staff
@@ -103,14 +103,20 @@
         
         
         
         
         History
         -------
         
+        0.1.6.8 (2021-12-23)
+        ++++++++++++++++++++++
+        
+        * 879490a - filter on choice staff absence only active staff
+        * d04ba24 - Fix bug when save staff for training
+        
         0.1.6.7 (2021-12-22)
         ++++++++++++++++++++++
         
         * c19f6cb - Filter by default to staff active in list admin
         * dd97bda - Fix requirements
         
         0.1.6.6 (2021-12-14)
```

### Comparing `nobinobi-staff-0.1.6.7/README.rst` & `nobinobi-staff-0.1.6.8/README.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/__init__.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 #  License, or (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Affero General Public License for more details.
 
-__version__ = "0.1.6.7"
+__version__ = "0.1.6.8"
 default_app_config = 'nobinobi_staff.apps.NobinobiStaffConfig'
```

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/admin.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,19 @@
          }),
         (_('Comment'),
          {
              'fields': ['comment'],
          }),
     ]
 
+    def get_form(self, request, obj=None, **kwargs):
+        form = super(AbsenceAdmin, self).get_form(request, obj, **kwargs)
+        form.base_fields['staff'].queryset = Staff.objects.filter(status__exact='active')
+        return form
+
 
 @admin.register(AbsenceType)
 class AbsenceTypeAdmin(admin.ModelAdmin):
     list_filter = ('reason', 'abbr',)
     ordering = ('reason',)
     search_fields = ('reason', 'abbr',)
```

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/apps.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/apps.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/fixtures/staff_absence_type_en-US.json` & `nobinobi-staff-0.1.6.8/nobinobi_staff/fixtures/staff_absence_type_en-US.json`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/fixtures/staff_absence_type_fr-CH.json` & `nobinobi-staff-0.1.6.8/nobinobi_staff/fixtures/staff_absence_type_fr-CH.json`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/forms.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/forms.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/locale/fr/LC_MESSAGES/django.mo` & `nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/locale/fr_CH/LC_MESSAGES/django.mo` & `nobinobi-staff-0.1.6.8/nobinobi_staff/locale/fr_CH/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/management/__init__.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/management/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/management/commands/__init__.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/management/commands/generate_training.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/generate_training.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/management/commands/update_training.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/management/commands/update_training.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0001_initial.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0002_auto_20181019_1017.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0002_auto_20181019_1017.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0003_auto_20181022_1101.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0003_auto_20181022_1101.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0004_team_order.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0004_team_order.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0005_auto_20181116_0815.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0005_auto_20181116_0815.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0006_staff_working_base.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0006_staff_working_base.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0007_auto_20200221_1138.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0007_auto_20200221_1138.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0008_add_partial_disability.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0008_add_partial_disability.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0009_auto_20200805_1143.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0009_auto_20200805_1143.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/0010_auto_20201029_1500.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/0010_auto_20201029_1500.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/migrations/__init__.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/models.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/models.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/serializers.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/serializers.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/signals.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/signals.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,16 @@
                 training.default_number_days = (rt.number_days * ta) / 100
                 training.save()
 
 
 @receiver(post_save, sender=Staff)
 def update_training_for_staff(sender, instance, created, raw, using, **kwargs):
     create_training_for_staff(instance)
+    year = timezone.localdate().year
+    call_command('update_training', years=[year], staffs=[instance.id])
 
 
 @receiver(post_save, sender=Absence)
 def create_training_for_staff_after_absence(sender, instance, created, raw, using, **kwargs):
     create_training_for_staff(instance.staff, instance)
```

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/static/css/nobinobi_staff.css` & `nobinobi-staff-0.1.6.8/nobinobi_staff/static/css/nobinobi_staff.css`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/static/js/nobinobi_staff.js` & `nobinobi-staff-0.1.6.8/nobinobi_staff/static/js/nobinobi_staff.js`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/templates/staff/staff_list_readonly.html` & `nobinobi-staff-0.1.6.8/nobinobi_staff/templates/staff/staff_list_readonly.html`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/tests.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/tests.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/urls.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/urls.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff/views.py` & `nobinobi-staff-0.1.6.8/nobinobi_staff/views.py`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff.egg-info/PKG-INFO` & `nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nobinobi-staff
-Version: 0.1.6.7
+Version: 0.1.6.8
 Summary: Application staff for nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-staff
 Author: Florian Alu
 Author-email: alu@prolibre.com
 License: UNKNOWN
 Description: =============================
         Nobinobi Staff
@@ -103,14 +103,20 @@
         
         
         
         
         History
         -------
         
+        0.1.6.8 (2021-12-23)
+        ++++++++++++++++++++++
+        
+        * 879490a - filter on choice staff absence only active staff
+        * d04ba24 - Fix bug when save staff for training
+        
         0.1.6.7 (2021-12-22)
         ++++++++++++++++++++++
         
         * c19f6cb - Filter by default to staff active in list admin
         * dd97bda - Fix requirements
         
         0.1.6.6 (2021-12-14)
```

### Comparing `nobinobi-staff-0.1.6.7/nobinobi_staff.egg-info/SOURCES.txt` & `nobinobi-staff-0.1.6.8/nobinobi_staff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/requirements_dev.txt` & `nobinobi-staff-0.1.6.8/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `nobinobi-staff-0.1.6.7/setup.py` & `nobinobi-staff-0.1.6.8/setup.py`

 * *Files identical despite different names*

