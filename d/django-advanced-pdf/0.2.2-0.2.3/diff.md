# Comparing `tmp/django-advanced-pdf-0.2.2.tar.gz` & `tmp/django-advanced-pdf-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-advanced-pdf-0.2.2.tar", last modified: Thu May  4 16:01:40 2023, max compression
+gzip compressed data, was "django-advanced-pdf-0.2.3.tar", last modified: Fri May  5 13:28:27 2023, max compression
```

## Comparing `django-advanced-pdf-0.2.2.tar` & `django-advanced-pdf-0.2.3.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.387322 django-advanced-pdf-0.2.2/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       83 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      629 2023-05-04 16:01:40.387136 django-advanced-pdf-0.2.2/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      158 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.282249 django-advanced-pdf-0.2.2/django_advanced_pdf/
--rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:32.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/.DS_Store
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.286035 django-advanced-pdf-0.2.2/django_advanced_pdf/_trial_temp/
--rwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/_trial_temp/_trial_marker
--rw-r--r--   0 tom        (501) staff       (20)       41 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/_trial_temp/test.log
--rw-r--r--   0 tom        (501) staff       (20)      223 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      207 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/apps.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.288144 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.290195 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_paragraph/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_paragraph/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3083 2023-03-02 10:42:09.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py
--rw-r--r--   0 tom        (501) staff       (20)     2043 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_paragraph/parser.py
--rw-r--r--   0 tom        (501) staff       (20)     4197 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_paragraph/style.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.292107 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_table/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_table/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1281 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_table/data.py
--rw-r--r--   0 tom        (501) staff       (20)     1413 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_table/data_paragraph.py
--rw-r--r--   0 tom        (501) staff       (20)    34502 2023-03-01 15:54:45.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py
--rw-r--r--   0 tom        (501) staff       (20)      712 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/png_images.py
--rw-r--r--   0 tom        (501) staff       (20)    56762 2023-05-03 10:20:01.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/report_xml.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.294029 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/svglib/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/svglib/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    52517 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/svglib/svglib.py
--rw-r--r--   0 tom        (501) staff       (20)     7963 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/svglib/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     9579 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/engine/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.294927 django-advanced-pdf-0.2.2/django_advanced_pdf/migrations/
--rw-r--r--   0 tom        (501) staff       (20)      554 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1176 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/models.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.296495 django-advanced-pdf-0.2.2/django_advanced_pdf/pagers/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/pagers/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     7952 2023-05-03 09:14:16.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/pagers/base.py
--rw-r--r--   0 tom        (501) staff       (20)     5049 2023-05-03 09:07:57.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/pagers/border.py
--rw-r--r--   0 tom        (501) staff       (20)     2432 2023-05-04 16:00:47.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/tasks.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.297010 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/
--rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/.DS_Store
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.297477 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/
--rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/.DS_Store
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.307531 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/abs2/
--rw-r--r--   0 tom        (501) staff       (20)   142408 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/abs2/1.png
--rw-r--r--   0 tom        (501) staff       (20)   194803 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/abs2/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/abs2/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.308452 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/abs3/
--rw-r--r--   0 tom        (501) staff       (20)    49895 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/abs3/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/abs3/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.309347 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/background_colour/
--rw-r--r--   0 tom        (501) staff       (20)    32702 2023-02-23 12:19:01.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/background_colour/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:19:01.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/background_colour/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.315653 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/basic/
--rw-r--r--   0 tom        (501) staff       (20)   142700 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/basic/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/basic/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.316840 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/border/
--rw-r--r--   0 tom        (501) staff       (20)    86430 2023-02-23 12:28:02.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/border/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:28:02.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/border/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.320269 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/change_header/
--rw-r--r--   0 tom        (501) staff       (20)   116046 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/change_header/1.png
--rw-r--r--   0 tom        (501) staff       (20)   135419 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/change_header/2.png
--rw-r--r--   0 tom        (501) staff       (20)   133527 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/change_header/3.png
--rw-r--r--   0 tom        (501) staff       (20)    67070 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/change_header/4.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/change_header/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.322553 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/hidden/
--rw-r--r--   0 tom        (501) staff       (20)   142804 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/hidden/1.png
--rw-r--r--   0 tom        (501) staff       (20)   129438 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/hidden/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-06 08:57:48.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/hidden/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.328039 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/
--rw-r--r--   0 tom        (501) staff       (20)   101102 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/1.png
--rw-r--r--   0 tom        (501) staff       (20)   131206 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/2.png
--rw-r--r--   0 tom        (501) staff       (20)   123455 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/3.png
--rw-r--r--   0 tom        (501) staff       (20)   147016 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/4.png
--rw-r--r--   0 tom        (501) staff       (20)   154909 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/5.png
--rw-r--r--   0 tom        (501) staff       (20)   164056 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/6.png
--rw-r--r--   0 tom        (501) staff       (20)   171134 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/7.png
--rw-r--r--   0 tom        (501) staff       (20)   100782 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/8.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.331373 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/overflow_gt_height/
--rw-r--r--   0 tom        (501) staff       (20)   752024 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/overflow_gt_height/1.png
--rw-r--r--   0 tom        (501) staff       (20)   473318 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/overflow_gt_height/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/overflow_gt_height/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.336043 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/
--rw-r--r--   0 tom        (501) staff       (20)     8996 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/abs2.xml
--rw-r--r--   0 tom        (501) staff       (20)      746 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/abs3.xml
--rw-r--r--   0 tom        (501) staff       (20)      203 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/background_colour.xml
--rw-r--r--   0 tom        (501) staff       (20)    49397 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/basic.xml
--rw-r--r--   0 tom        (501) staff       (20)     1327 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/border.xml
--rw-r--r--   0 tom        (501) staff       (20)     7790 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/change_header.xml
--rw-r--r--   0 tom        (501) staff       (20)     4192 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/hidden.xml
--rw-r--r--   0 tom        (501) staff       (20)    12752 2023-02-23 11:40:06.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/keep_with_next.xml
--rw-r--r--   0 tom        (501) staff       (20)     7691 2023-03-02 10:18:57.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/overflow_gt_height.xml
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.274311 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.338113 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/abs2/
--rw-r--r--   0 tom        (501) staff       (20)   142408 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/abs2/1.png
--rw-r--r--   0 tom        (501) staff       (20)   194803 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/abs2/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/abs2/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.339437 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/abs3/
--rw-r--r--   0 tom        (501) staff       (20)    49895 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/abs3/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/abs3/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.340355 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/background_colour/
--rw-r--r--   0 tom        (501) staff       (20)    32702 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/background_colour/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/background_colour/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.341420 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/basic/
--rw-r--r--   0 tom        (501) staff       (20)   142700 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/basic/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/basic/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.342153 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/border/
--rw-r--r--   0 tom        (501) staff       (20)    86430 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/border/1.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/border/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.345865 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/change_header/
--rw-r--r--   0 tom        (501) staff       (20)   116046 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/change_header/1.png
--rw-r--r--   0 tom        (501) staff       (20)   135419 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/change_header/2.png
--rw-r--r--   0 tom        (501) staff       (20)   133527 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/change_header/3.png
--rw-r--r--   0 tom        (501) staff       (20)    67070 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/change_header/4.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/change_header/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.347619 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/hidden/
--rw-r--r--   0 tom        (501) staff       (20)   142804 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/hidden/1.png
--rw-r--r--   0 tom        (501) staff       (20)   129438 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/hidden/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/hidden/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.377925 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/
--rw-r--r--   0 tom        (501) staff       (20)   101102 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/1.png
--rw-r--r--   0 tom        (501) staff       (20)   131206 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/2.png
--rw-r--r--   0 tom        (501) staff       (20)   123455 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/3.png
--rw-r--r--   0 tom        (501) staff       (20)   147016 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/4.png
--rw-r--r--   0 tom        (501) staff       (20)   154909 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/5.png
--rw-r--r--   0 tom        (501) staff       (20)   164056 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/6.png
--rw-r--r--   0 tom        (501) staff       (20)   171134 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/7.png
--rw-r--r--   0 tom        (501) staff       (20)   100782 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/8.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/page_count.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.385082 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/overflow_gt_height/
--rw-r--r--   0 tom        (501) staff       (20)   752024 2023-03-20 15:08:05.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png
--rw-r--r--   0 tom        (501) staff       (20)   473318 2023-03-20 15:08:05.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:05.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/overflow_gt_height/page_count.txt
--rw-r--r--   0 tom        (501) staff       (20)     4852 2023-03-06 08:57:48.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/tests.py
--rw-r--r--   0 tom        (501) staff       (20)      336 2023-05-04 10:30:08.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/urls.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.386243 django-advanced-pdf-0.2.2/django_advanced_pdf/views/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-05-03 10:37:37.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/views/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      499 2023-05-04 09:14:22.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/views/standard.py
--rw-r--r--   0 tom        (501) staff       (20)     1387 2023-05-04 10:54:47.000000 django-advanced-pdf-0.2.2/django_advanced_pdf/views/tasks.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-04 16:01:40.285327 django-advanced-pdf-0.2.2/django_advanced_pdf.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      629 2023-05-04 16:01:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     5599 2023-05-04 16:01:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-04 16:01:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       20 2023-05-04 16:01:40.000000 django-advanced-pdf-0.2.2/django_advanced_pdf.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-05-04 16:01:40.387364 django-advanced-pdf-0.2.2/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      672 2023-05-04 16:00:57.000000 django-advanced-pdf-0.2.2/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.069733 django-advanced-pdf-0.2.3/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       83 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      629 2023-05-05 13:28:27.069482 django-advanced-pdf-0.2.3/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      158 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.933133 django-advanced-pdf-0.2.3/django_advanced_pdf/
+-rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:32.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/.DS_Store
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.939435 django-advanced-pdf-0.2.3/django_advanced_pdf/_trial_temp/
+-rwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/_trial_temp/_trial_marker
+-rw-r--r--   0 tom        (501) staff       (20)       41 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/_trial_temp/test.log
+-rw-r--r--   0 tom        (501) staff       (20)      223 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      207 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/apps.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.947583 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.949815 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_paragraph/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_paragraph/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3083 2023-03-02 10:42:09.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py
+-rw-r--r--   0 tom        (501) staff       (20)     2043 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_paragraph/parser.py
+-rw-r--r--   0 tom        (501) staff       (20)     4197 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_paragraph/style.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.953082 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_table/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_table/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1281 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_table/data.py
+-rw-r--r--   0 tom        (501) staff       (20)     1413 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_table/data_paragraph.py
+-rw-r--r--   0 tom        (501) staff       (20)    34502 2023-03-01 15:54:45.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py
+-rw-r--r--   0 tom        (501) staff       (20)      712 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/png_images.py
+-rw-r--r--   0 tom        (501) staff       (20)    56762 2023-05-03 10:20:01.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/report_xml.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.956379 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/svglib/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/svglib/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    52517 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/svglib/svglib.py
+-rw-r--r--   0 tom        (501) staff       (20)     7963 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/svglib/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     9579 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/engine/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.957248 django-advanced-pdf-0.2.3/django_advanced_pdf/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)      554 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1176 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/models.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.964510 django-advanced-pdf-0.2.3/django_advanced_pdf/pagers/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/pagers/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     7952 2023-05-03 09:14:16.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/pagers/base.py
+-rw-r--r--   0 tom        (501) staff       (20)     5049 2023-05-03 09:07:57.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/pagers/border.py
+-rw-r--r--   0 tom        (501) staff       (20)     2432 2023-05-04 16:00:47.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/tasks.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.965319 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/
+-rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/.DS_Store
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.966801 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/
+-rw-r--r--   0 tom        (501) staff       (20)     6148 2023-02-23 15:49:37.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/.DS_Store
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.969053 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/abs2/
+-rw-r--r--   0 tom        (501) staff       (20)   142408 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/abs2/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   194803 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/abs2/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/abs2/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.969952 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/abs3/
+-rw-r--r--   0 tom        (501) staff       (20)    49895 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/abs3/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:20:55.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/abs3/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.970967 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/background_colour/
+-rw-r--r--   0 tom        (501) staff       (20)    32702 2023-02-23 12:19:01.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/background_colour/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:19:01.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/background_colour/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.972145 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/basic/
+-rw-r--r--   0 tom        (501) staff       (20)   142700 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/basic/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/basic/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.973419 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/border/
+-rw-r--r--   0 tom        (501) staff       (20)    86430 2023-02-23 12:28:02.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/border/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 12:28:02.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/border/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.976167 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/change_header/
+-rw-r--r--   0 tom        (501) staff       (20)   116046 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/change_header/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   135419 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/change_header/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   133527 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/change_header/3.png
+-rw-r--r--   0 tom        (501) staff       (20)    67070 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/change_header/4.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 11:51:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/change_header/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.978169 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/hidden/
+-rw-r--r--   0 tom        (501) staff       (20)   142804 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/hidden/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   129438 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/hidden/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-06 08:57:48.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/hidden/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.019044 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/
+-rw-r--r--   0 tom        (501) staff       (20)   101102 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   131206 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   123455 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/3.png
+-rw-r--r--   0 tom        (501) staff       (20)   147016 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/4.png
+-rw-r--r--   0 tom        (501) staff       (20)   154909 2023-02-23 10:44:40.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/5.png
+-rw-r--r--   0 tom        (501) staff       (20)   164056 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/6.png
+-rw-r--r--   0 tom        (501) staff       (20)   171134 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/7.png
+-rw-r--r--   0 tom        (501) staff       (20)   100782 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/8.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-02-23 10:44:41.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.024479 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/overflow_gt_height/
+-rw-r--r--   0 tom        (501) staff       (20)   752024 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/overflow_gt_height/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   473318 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/overflow_gt_height/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-02 10:39:31.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/overflow_gt_height/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.029629 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/
+-rw-r--r--   0 tom        (501) staff       (20)     8996 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/abs2.xml
+-rw-r--r--   0 tom        (501) staff       (20)      746 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/abs3.xml
+-rw-r--r--   0 tom        (501) staff       (20)      203 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/background_colour.xml
+-rw-r--r--   0 tom        (501) staff       (20)    49397 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/basic.xml
+-rw-r--r--   0 tom        (501) staff       (20)     1327 2023-01-16 11:14:24.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/border.xml
+-rw-r--r--   0 tom        (501) staff       (20)     7790 2023-02-22 15:48:40.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/change_header.xml
+-rw-r--r--   0 tom        (501) staff       (20)     4192 2023-03-14 12:55:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/hidden.xml
+-rw-r--r--   0 tom        (501) staff       (20)    12752 2023-02-23 11:40:06.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/keep_with_next.xml
+-rw-r--r--   0 tom        (501) staff       (20)     7691 2023-03-02 10:18:57.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/overflow_gt_height.xml
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.917546 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.031778 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/abs2/
+-rw-r--r--   0 tom        (501) staff       (20)   142408 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/abs2/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   194803 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/abs2/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:58.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/abs2/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.032992 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/abs3/
+-rw-r--r--   0 tom        (501) staff       (20)    49895 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/abs3/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/abs3/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.033910 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/background_colour/
+-rw-r--r--   0 tom        (501) staff       (20)    32702 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/background_colour/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:07:59.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/background_colour/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.035029 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/basic/
+-rw-r--r--   0 tom        (501) staff       (20)   142700 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/basic/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/basic/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.035824 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/border/
+-rw-r--r--   0 tom        (501) staff       (20)    86430 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/border/1.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/border/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.038940 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/change_header/
+-rw-r--r--   0 tom        (501) staff       (20)   116046 2023-03-20 15:08:00.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/change_header/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   135419 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/change_header/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   133527 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/change_header/3.png
+-rw-r--r--   0 tom        (501) staff       (20)    67070 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/change_header/4.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/change_header/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.040717 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/hidden/
+-rw-r--r--   0 tom        (501) staff       (20)   142804 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/hidden/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   129438 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/hidden/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:01.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/hidden/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.052822 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/
+-rw-r--r--   0 tom        (501) staff       (20)   101102 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   131206 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/2.png
+-rw-r--r--   0 tom        (501) staff       (20)   123455 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/3.png
+-rw-r--r--   0 tom        (501) staff       (20)   147016 2023-03-20 15:08:02.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/4.png
+-rw-r--r--   0 tom        (501) staff       (20)   154909 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/5.png
+-rw-r--r--   0 tom        (501) staff       (20)   164056 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/6.png
+-rw-r--r--   0 tom        (501) staff       (20)   171134 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/7.png
+-rw-r--r--   0 tom        (501) staff       (20)   100782 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/8.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:03.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/page_count.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.059920 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/overflow_gt_height/
+-rw-r--r--   0 tom        (501) staff       (20)   752024 2023-03-20 15:08:05.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png
+-rw-r--r--   0 tom        (501) staff       (20)   473318 2023-03-20 15:08:05.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-20 15:08:05.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/overflow_gt_height/page_count.txt
+-rw-r--r--   0 tom        (501) staff       (20)     4852 2023-03-06 08:57:48.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/tests.py
+-rw-r--r--   0 tom        (501) staff       (20)      336 2023-05-04 10:30:08.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/urls.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:27.068994 django-advanced-pdf-0.2.3/django_advanced_pdf/views/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-05-03 10:37:37.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/views/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      499 2023-05-04 09:14:22.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/views/standard.py
+-rw-r--r--   0 tom        (501) staff       (20)     1471 2023-05-05 13:22:57.000000 django-advanced-pdf-0.2.3/django_advanced_pdf/views/tasks.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-05 13:28:26.938315 django-advanced-pdf-0.2.3/django_advanced_pdf.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      629 2023-05-05 13:28:26.000000 django-advanced-pdf-0.2.3/django_advanced_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     5599 2023-05-05 13:28:26.000000 django-advanced-pdf-0.2.3/django_advanced_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-05 13:28:26.000000 django-advanced-pdf-0.2.3/django_advanced_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       20 2023-05-05 13:28:26.000000 django-advanced-pdf-0.2.3/django_advanced_pdf.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-05-05 13:28:27.069805 django-advanced-pdf-0.2.3/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      672 2023-05-05 13:27:37.000000 django-advanced-pdf-0.2.3/setup.py
```

### Comparing `django-advanced-pdf-0.2.2/LICENSE` & `django-advanced-pdf-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/PKG-INFO` & `django-advanced-pdf-0.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-pdf
-Version: 0.2.2
+Version: 0.2.3
 Summary: Django app that helps one create pdf
 Home-page: https://github.com/django-advance-utils/django-advanced-pdf
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/.DS_Store` & `django-advanced-pdf-0.2.3/django_advanced_pdf/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_paragraph/enhanced_paragraph.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_paragraph/parser.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_paragraph/parser.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_paragraph/style.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_paragraph/style.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_table/data.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_table/data.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_table/data_paragraph.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_table/data_paragraph.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/engine/enhanced_table/enhanced_tables.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/engine/png_images.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/engine/png_images.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/engine/report_xml.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/engine/report_xml.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/engine/svglib/svglib.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/engine/svglib/svglib.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/engine/svglib/utils.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/engine/svglib/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/engine/utils.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/engine/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/migrations/0001_initial.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/models.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/models.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/pagers/base.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/pagers/base.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/pagers/border.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/pagers/border.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/tasks.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/tasks.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/.DS_Store` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/.DS_Store` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/abs2/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/abs2/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/abs2/2.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/abs2/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/abs3/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/abs3/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/background_colour/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/background_colour/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/basic/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/basic/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/border/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/border/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/change_header/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/change_header/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/change_header/2.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/change_header/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/change_header/3.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/change_header/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/change_header/4.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/change_header/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/hidden/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/hidden/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/hidden/2.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/hidden/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/2.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/3.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/4.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/5.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/5.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/6.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/6.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/7.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/7.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/keep_with_next/8.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/keep_with_next/8.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/overflow_gt_height/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/overflow_gt_height/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/held/overflow_gt_height/2.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/held/overflow_gt_height/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/abs2.xml` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/abs2.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/abs3.xml` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/abs3.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/basic.xml` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/basic.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/border.xml` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/border.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/change_header.xml` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/change_header.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/hidden.xml` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/hidden.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/keep_with_next.xml` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/keep_with_next.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/reports/overflow_gt_height.xml` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/reports/overflow_gt_height.xml`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/abs2/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/abs2/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/abs2/2.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/abs2/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/abs3/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/abs3/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/background_colour/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/background_colour/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/basic/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/basic/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/border/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/border/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/change_header/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/change_header/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/change_header/2.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/change_header/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/change_header/3.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/change_header/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/change_header/4.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/change_header/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/hidden/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/hidden/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/hidden/2.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/hidden/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/2.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/3.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/3.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/4.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/4.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/5.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/5.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/6.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/6.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/7.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/7.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/keep_with_next/8.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/keep_with_next/8.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/overflow_gt_height/1.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png` & `django-advanced-pdf-0.2.3/django_advanced_pdf/test_data/temp/overflow_gt_height/2.png`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/tests.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/tests.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf/views/tasks.py` & `django-advanced-pdf-0.2.3/django_advanced_pdf/views/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from django.core.cache import caches
 from django.core.files.base import ContentFile
 from django.http import FileResponse, Http404
 from django.urls import reverse
+from django.utils.decorators import method_decorator
 from django.utils.safestring import mark_safe
 from django.views import View
 from django.views.decorators.clickjacking import xframe_options_exempt
 from django_modals.modals import Modal
 
 
+@method_decorator(xframe_options_exempt, name='dispatch')
 class ViewTaskPDF(View):
     cache_key = 'default'
 
-    @xframe_options_exempt
     def get(self, request, file_key):
         cache_data = caches[self.cache_key].get(file_key)
         if cache_data is not None:
             response = FileResponse(ContentFile(cache_data['file']), content_type="application/pdf")
             filename = cache_data['filename']
             response['Content-Disposition'] = f'filename={filename}'
             response['Content-Length'] = len(cache_data['file'])
```

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf.egg-info/PKG-INFO` & `django-advanced-pdf-0.2.3/django_advanced_pdf.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-pdf
-Version: 0.2.2
+Version: 0.2.3
 Summary: Django app that helps one create pdf
 Home-page: https://github.com/django-advance-utils/django-advanced-pdf
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-pdf-0.2.2/django_advanced_pdf.egg-info/SOURCES.txt` & `django-advanced-pdf-0.2.3/django_advanced_pdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-advanced-pdf-0.2.2/setup.py` & `django-advanced-pdf-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-advanced-pdf",
-    version="0.2.2",
+    version="0.2.3",
     author="Thomas Turner",
     description="Django app that helps one create pdf",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-advanced-pdf",
     include_package_data=True,
     packages=['django_advanced_pdf'],
```

