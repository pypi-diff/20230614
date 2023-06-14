# Comparing `tmp/projectal-3.1.1.tar.gz` & `tmp/projectal-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectal-3.1.1.tar", last modified: Thu Mar  9 05:04:00 2023, max compression
+gzip compressed data, was "projectal-4.0.1.tar", last modified: Wed Jun 14 06:22:58 2023, max compression
```

## Comparing `projectal-3.1.1.tar` & `projectal-4.0.1.tar`

### file list

```diff
@@ -1,84 +1,88 @@
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-03-09 05:04:00.520494 projectal-3.1.1/
--rw-rw-r--   0 luked     (1003) luked     (1003)     1074 2022-11-17 04:31:31.000000 projectal-3.1.1/LICENSE
--rw-rw-r--   0 luked     (1003) luked     (1003)       30 2022-11-17 04:31:31.000000 projectal-3.1.1/MANIFEST.in
--rw-rw-r--   0 luked     (1003) luked     (1003)      573 2023-03-09 05:04:00.520494 projectal-3.1.1/PKG-INFO
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-03-09 05:04:00.500494 projectal-3.1.1/docs/
--rw-rw-r--   0 luked     (1003) luked     (1003)      140 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/index.html
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-03-09 05:04:00.504494 projectal-3.1.1/docs/projectal/
--rw-rw-r--   0 luked     (1003) luked     (1003)   123963 2023-03-09 05:02:58.000000 projectal-3.1.1/docs/projectal/api.html
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-03-09 05:04:00.512494 projectal-3.1.1/docs/projectal/entities/
--rw-rw-r--   0 luked     (1003) luked     (1003)    44886 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/access_policy.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    76700 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/calendar.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    78998 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/company.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    60445 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/contact.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    47063 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/customer.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    72006 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/department.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   112784 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/file.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    79391 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/folder.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    67125 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/location.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    73862 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/note.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    51453 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/permission.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    76122 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/project.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    53421 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/project_template.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    46200 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/rebate.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    46469 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/resource.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    45789 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/skill.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   138305 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/staff.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    44760 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/stage.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    42248 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/tag.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   167963 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/task.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    81669 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/task_template.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    82639 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/user.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    76578 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities/webhook.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    42087 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entities.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   660878 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/entity.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    81307 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/enums.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   107022 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/errors.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   260261 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/linkers.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    57589 2023-03-09 05:02:59.000000 projectal-3.1.1/docs/projectal/profile.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   111803 2023-03-09 05:02:58.000000 projectal-3.1.1/docs/projectal.html
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-03-09 05:04:00.512494 projectal-3.1.1/examples/
--rw-rw-r--   0 luked     (1003) luked     (1003)     3154 2022-11-17 04:31:31.000000 projectal-3.1.1/examples/linking.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      811 2022-11-17 04:31:31.000000 projectal-3.1.1/examples/task.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1064 2022-12-01 02:53:21.000000 projectal-3.1.1/examples/webhook.py
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-03-09 05:04:00.516494 projectal-3.1.1/projectal/
--rw-rw-r--   0 luked     (1003) luked     (1003)    16944 2023-03-09 04:46:21.000000 projectal-3.1.1/projectal/__init__.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     9133 2023-03-09 04:46:05.000000 projectal-3.1.1/projectal/api.py
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-03-09 05:04:00.520494 projectal-3.1.1/projectal/entities/
--rw-rw-r--   0 luked     (1003) luked     (1003)     1202 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/__init__.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      395 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/access_policy.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     2233 2022-12-21 23:38:50.000000 projectal-3.1.1/projectal/entities/calendar.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1935 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/company.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      982 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/contact.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      460 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/customer.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1855 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/department.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     3171 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/file.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1732 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/folder.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1305 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/location.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1939 2022-12-21 23:38:50.000000 projectal-3.1.1/projectal/entities/note.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      613 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/permission.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1655 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/project.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      709 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/project_template.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      426 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/rebate.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      434 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/resource.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      395 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/skill.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     4678 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/staff.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      344 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/stage.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      230 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/tag.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     6359 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/task.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1833 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/task_template.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1978 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/entities/user.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1668 2022-12-21 23:38:50.000000 projectal-3.1.1/projectal/entities/webhook.py
--rw-rw-r--   0 luked     (1003) luked     (1003)    40482 2023-03-09 04:46:05.000000 projectal-3.1.1/projectal/entity.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     2152 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/enums.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     3564 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/errors.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     8657 2022-12-21 23:38:50.000000 projectal-3.1.1/projectal/linkers.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     2382 2022-11-17 04:31:31.000000 projectal-3.1.1/projectal/profile.py
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-03-09 05:04:00.516494 projectal-3.1.1/projectal.egg-info/
--rw-rw-r--   0 luked     (1003) luked     (1003)      573 2023-03-09 05:04:00.000000 projectal-3.1.1/projectal.egg-info/PKG-INFO
--rw-rw-r--   0 luked     (1003) luked     (1003)     2200 2023-03-09 05:04:00.000000 projectal-3.1.1/projectal.egg-info/SOURCES.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)        1 2023-03-09 05:04:00.000000 projectal-3.1.1/projectal.egg-info/dependency_links.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)       19 2023-03-09 05:04:00.000000 projectal-3.1.1/projectal.egg-info/requires.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)       19 2023-03-09 05:04:00.000000 projectal-3.1.1/projectal.egg-info/top_level.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)       38 2023-03-09 05:04:00.520494 projectal-3.1.1/setup.cfg
--rw-rw-r--   0 luked     (1003) luked     (1003)      757 2023-03-09 04:46:21.000000 projectal-3.1.1/setup.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.541076 projectal-4.0.1/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1074 2022-11-17 04:31:31.000000 projectal-4.0.1/LICENSE
+-rw-rw-r--   0 luked     (1003) luked     (1003)       30 2022-11-17 04:31:31.000000 projectal-4.0.1/MANIFEST.in
+-rw-rw-r--   0 luked     (1003) luked     (1003)      573 2023-06-14 06:22:58.541076 projectal-4.0.1/PKG-INFO
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.533076 projectal-4.0.1/docs/
+-rw-rw-r--   0 luked     (1003) luked     (1003)      140 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/index.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.537076 projectal-4.0.1/docs/projectal/
+-rw-rw-r--   0 luked     (1003) luked     (1003)   123963 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/api.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.537076 projectal-4.0.1/docs/projectal/entities/
+-rw-rw-r--   0 luked     (1003) luked     (1003)    44886 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/access_policy.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    48388 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/activity.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    43819 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/booking.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    76700 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/calendar.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    78998 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/company.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    60445 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/contact.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    47063 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/customer.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    72006 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/department.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   112784 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/file.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    79391 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/folder.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    67125 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/location.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    73862 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/note.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    51453 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/permission.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    76122 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/project.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    53421 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/project_template.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    46200 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/rebate.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    46469 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/resource.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    45789 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/skill.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   138305 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/staff.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    44760 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/stage.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    42248 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/tag.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   167963 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/task.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    81669 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/task_template.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    82639 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/user.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    76578 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/webhook.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    42661 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   660878 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entity.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    81307 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/enums.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   107022 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/errors.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   260261 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/linkers.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    57589 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/profile.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   113364 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.541076 projectal-4.0.1/examples/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3154 2022-11-17 04:31:31.000000 projectal-4.0.1/examples/linking.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      811 2022-11-17 04:31:31.000000 projectal-4.0.1/examples/task.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1064 2022-12-01 02:53:21.000000 projectal-4.0.1/examples/webhook.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.541076 projectal-4.0.1/projectal/
+-rw-rw-r--   0 luked     (1003) luked     (1003)    17172 2023-06-14 06:18:47.000000 projectal-4.0.1/projectal/__init__.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     9133 2023-03-09 04:46:05.000000 projectal-4.0.1/projectal/api.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.541076 projectal-4.0.1/projectal/entities/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1298 2023-05-16 05:22:36.000000 projectal-4.0.1/projectal/entities/__init__.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      395 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/access_policy.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      485 2023-05-16 05:57:07.000000 projectal-4.0.1/projectal/entities/activity.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      303 2023-05-16 05:57:12.000000 projectal-4.0.1/projectal/entities/booking.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2233 2022-12-21 23:38:50.000000 projectal-4.0.1/projectal/entities/calendar.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1935 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/company.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      982 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/contact.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      460 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/customer.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1855 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/department.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3171 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/file.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1732 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/folder.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1305 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/location.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1939 2022-12-21 23:38:50.000000 projectal-4.0.1/projectal/entities/note.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      613 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/permission.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1655 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/project.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      709 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/project_template.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      426 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/rebate.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      434 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/resource.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      395 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/skill.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     4678 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/staff.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      344 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/stage.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      230 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/tag.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     6359 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/task.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1833 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/task_template.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1978 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/user.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1668 2022-12-21 23:38:50.000000 projectal-4.0.1/projectal/entities/webhook.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)    40482 2023-03-09 04:46:05.000000 projectal-4.0.1/projectal/entity.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2152 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/enums.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3564 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/errors.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     8657 2022-12-21 23:38:50.000000 projectal-4.0.1/projectal/linkers.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2382 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/profile.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.541076 projectal-4.0.1/projectal.egg-info/
+-rw-rw-r--   0 luked     (1003) luked     (1003)      573 2023-06-14 06:22:58.000000 projectal-4.0.1/projectal.egg-info/PKG-INFO
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2336 2023-06-14 06:22:58.000000 projectal-4.0.1/projectal.egg-info/SOURCES.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)        1 2023-06-14 06:22:58.000000 projectal-4.0.1/projectal.egg-info/dependency_links.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       19 2023-06-14 06:22:58.000000 projectal-4.0.1/projectal.egg-info/requires.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       19 2023-06-14 06:22:58.000000 projectal-4.0.1/projectal.egg-info/top_level.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       38 2023-06-14 06:22:58.541076 projectal-4.0.1/setup.cfg
+-rw-rw-r--   0 luked     (1003) luked     (1003)      757 2023-06-14 06:15:07.000000 projectal-4.0.1/setup.py
```

### Comparing `projectal-3.1.1/LICENSE` & `projectal-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/PKG-INFO` & `projectal-4.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectal
-Version: 3.1.1
+Version: 4.0.1
 Summary: Python bindings for the Projectal API
 Home-page: https://projectal.com/resources/developer
 Author: Projectal
 Author-email: support@projectal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `projectal-3.1.1/docs/projectal/api.html` & `projectal-4.0.1/docs/projectal/api.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/access_policy.html` & `projectal-4.0.1/docs/projectal/entities/access_policy.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/calendar.html` & `projectal-4.0.1/docs/projectal/entities/calendar.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/company.html` & `projectal-4.0.1/docs/projectal/entities/company.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/contact.html` & `projectal-4.0.1/docs/projectal/entities/contact.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/customer.html` & `projectal-4.0.1/docs/projectal/entities/customer.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/department.html` & `projectal-4.0.1/docs/projectal/entities/department.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/file.html` & `projectal-4.0.1/docs/projectal/entities/file.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/folder.html` & `projectal-4.0.1/docs/projectal/entities/folder.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/location.html` & `projectal-4.0.1/docs/projectal/entities/location.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/note.html` & `projectal-4.0.1/docs/projectal/entities/note.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/permission.html` & `projectal-4.0.1/docs/projectal/entities/permission.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/project.html` & `projectal-4.0.1/docs/projectal/entities/project.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/project_template.html` & `projectal-4.0.1/docs/projectal/entities/project_template.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/rebate.html` & `projectal-4.0.1/docs/projectal/entities/rebate.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/resource.html` & `projectal-4.0.1/docs/projectal/entities/resource.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/skill.html` & `projectal-4.0.1/docs/projectal/entities/skill.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/staff.html` & `projectal-4.0.1/docs/projectal/entities/staff.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/stage.html` & `projectal-4.0.1/docs/projectal/entities/stage.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/tag.html` & `projectal-4.0.1/docs/projectal/entities/tag.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/task.html` & `projectal-4.0.1/docs/projectal/entities/task.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/task_template.html` & `projectal-4.0.1/docs/projectal/entities/task_template.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/user.html` & `projectal-4.0.1/docs/projectal/entities/user.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/webhook.html` & `projectal-4.0.1/docs/projectal/entities/webhook.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities.html` & `projectal-4.0.1/docs/projectal/entities.html`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,16 @@
             <input type="search" placeholder="Search..." role="searchbox" aria-label="search"
                    pattern=".+" required>
 
 
         <h2>Submodules</h2>
         <ul>
                 <li><a href="entities/access_policy.html">access_policy</a></li>
+                <li><a href="entities/activity.html">activity</a></li>
+                <li><a href="entities/booking.html">booking</a></li>
                 <li><a href="entities/calendar.html">calendar</a></li>
                 <li><a href="entities/company.html">company</a></li>
                 <li><a href="entities/contact.html">contact</a></li>
                 <li><a href="entities/customer.html">customer</a></li>
                 <li><a href="entities/department.html">department</a></li>
                 <li><a href="entities/file.html">file</a></li>
                 <li><a href="entities/folder.html">folder</a></li>
@@ -81,36 +83,38 @@
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="sd">Implementations of all Projectal entities.</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
 </span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="sd">All classes here inherit from `projectal.entity.Entity`.</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>
 </span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="kn">from</span> <span class="nn">projectal.entities.access_policy</span> <span class="kn">import</span> <span class="n">AccessPolicy</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="kn">from</span> <span class="nn">projectal.entities.calendar</span> <span class="kn">import</span> <span class="n">Calendar</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a><span class="kn">from</span> <span class="nn">projectal.entities.company</span> <span class="kn">import</span> <span class="n">Company</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a><span class="kn">from</span> <span class="nn">projectal.entities.contact</span> <span class="kn">import</span> <span class="n">Contact</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="kn">from</span> <span class="nn">projectal.entities.customer</span> <span class="kn">import</span> <span class="n">Customer</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a><span class="kn">from</span> <span class="nn">projectal.entities.department</span> <span class="kn">import</span> <span class="n">Department</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a><span class="kn">from</span> <span class="nn">projectal.entities.file</span> <span class="kn">import</span> <span class="n">File</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="kn">from</span> <span class="nn">projectal.entities.folder</span> <span class="kn">import</span> <span class="n">Folder</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="kn">from</span> <span class="nn">projectal.entities.location</span> <span class="kn">import</span> <span class="n">Location</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a><span class="kn">from</span> <span class="nn">projectal.entities.note</span> <span class="kn">import</span> <span class="n">Note</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="kn">from</span> <span class="nn">projectal.entities.permission</span> <span class="kn">import</span> <span class="n">Permission</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a><span class="kn">from</span> <span class="nn">projectal.entities.project</span> <span class="kn">import</span> <span class="n">Project</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a><span class="kn">from</span> <span class="nn">projectal.entities.project_template</span> <span class="kn">import</span> <span class="n">ProjectTemplate</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a><span class="kn">from</span> <span class="nn">projectal.entities.rebate</span> <span class="kn">import</span> <span class="n">Rebate</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a><span class="kn">from</span> <span class="nn">projectal.entities.resource</span> <span class="kn">import</span> <span class="n">Resource</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a><span class="kn">from</span> <span class="nn">projectal.entities.skill</span> <span class="kn">import</span> <span class="n">Skill</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a><span class="kn">from</span> <span class="nn">projectal.entities.staff</span> <span class="kn">import</span> <span class="n">Staff</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a><span class="kn">from</span> <span class="nn">projectal.entities.stage</span> <span class="kn">import</span> <span class="n">Stage</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a><span class="kn">from</span> <span class="nn">projectal.entities.tag</span> <span class="kn">import</span> <span class="n">Tag</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a><span class="kn">from</span> <span class="nn">projectal.entities.task</span> <span class="kn">import</span> <span class="n">Task</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a><span class="kn">from</span> <span class="nn">projectal.entities.task_template</span> <span class="kn">import</span> <span class="n">TaskTemplate</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a><span class="kn">from</span> <span class="nn">projectal.entities.user</span> <span class="kn">import</span> <span class="n">User</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a><span class="kn">from</span> <span class="nn">projectal.entities.webhook</span> <span class="kn">import</span> <span class="n">Webhook</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="kn">from</span> <span class="nn">projectal.entities.activity</span> <span class="kn">import</span> <span class="n">Activity</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a><span class="kn">from</span> <span class="nn">projectal.entities.booking</span> <span class="kn">import</span> <span class="n">Booking</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a><span class="kn">from</span> <span class="nn">projectal.entities.calendar</span> <span class="kn">import</span> <span class="n">Calendar</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="kn">from</span> <span class="nn">projectal.entities.company</span> <span class="kn">import</span> <span class="n">Company</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a><span class="kn">from</span> <span class="nn">projectal.entities.contact</span> <span class="kn">import</span> <span class="n">Contact</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a><span class="kn">from</span> <span class="nn">projectal.entities.customer</span> <span class="kn">import</span> <span class="n">Customer</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="kn">from</span> <span class="nn">projectal.entities.department</span> <span class="kn">import</span> <span class="n">Department</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="kn">from</span> <span class="nn">projectal.entities.file</span> <span class="kn">import</span> <span class="n">File</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a><span class="kn">from</span> <span class="nn">projectal.entities.folder</span> <span class="kn">import</span> <span class="n">Folder</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="kn">from</span> <span class="nn">projectal.entities.location</span> <span class="kn">import</span> <span class="n">Location</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a><span class="kn">from</span> <span class="nn">projectal.entities.note</span> <span class="kn">import</span> <span class="n">Note</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a><span class="kn">from</span> <span class="nn">projectal.entities.permission</span> <span class="kn">import</span> <span class="n">Permission</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a><span class="kn">from</span> <span class="nn">projectal.entities.project</span> <span class="kn">import</span> <span class="n">Project</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a><span class="kn">from</span> <span class="nn">projectal.entities.project_template</span> <span class="kn">import</span> <span class="n">ProjectTemplate</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a><span class="kn">from</span> <span class="nn">projectal.entities.rebate</span> <span class="kn">import</span> <span class="n">Rebate</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a><span class="kn">from</span> <span class="nn">projectal.entities.resource</span> <span class="kn">import</span> <span class="n">Resource</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a><span class="kn">from</span> <span class="nn">projectal.entities.skill</span> <span class="kn">import</span> <span class="n">Skill</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a><span class="kn">from</span> <span class="nn">projectal.entities.staff</span> <span class="kn">import</span> <span class="n">Staff</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a><span class="kn">from</span> <span class="nn">projectal.entities.stage</span> <span class="kn">import</span> <span class="n">Stage</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a><span class="kn">from</span> <span class="nn">projectal.entities.tag</span> <span class="kn">import</span> <span class="n">Tag</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a><span class="kn">from</span> <span class="nn">projectal.entities.task</span> <span class="kn">import</span> <span class="n">Task</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a><span class="kn">from</span> <span class="nn">projectal.entities.task_template</span> <span class="kn">import</span> <span class="n">TaskTemplate</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a><span class="kn">from</span> <span class="nn">projectal.entities.user</span> <span class="kn">import</span> <span class="n">User</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a><span class="kn">from</span> <span class="nn">projectal.entities.webhook</span> <span class="kn">import</span> <span class="n">Webhook</span>
 </span></pre></div>
 
 
             </section>
     </main>
 <script>
     function escapeHTML(html) {
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 
 
   ⁰
 ____ projectal [project logo] [Unknown INPUT type]
 ***** Submodules *****
     * access_policy
+    * activity
+    * booking
     * calendar
     * company
     * contact
     * customer
     * department
     * file
     * folder
@@ -35,30 +37,32 @@
 _1"""
 _2Implementations of all Projectal entities.
 _3
 _4All classes here inherit from `projectal.entity.Entity`.
 _5"""
 _6
 _7from projectal.entities.access_policy import AccessPolicy
-_8from projectal.entities.calendar import Calendar
-_9from projectal.entities.company import Company
-10from projectal.entities.contact import Contact
-11from projectal.entities.customer import Customer
-12from projectal.entities.department import Department
-13from projectal.entities.file import File
-14from projectal.entities.folder import Folder
-15from projectal.entities.location import Location
-16from projectal.entities.note import Note
-17from projectal.entities.permission import Permission
-18from projectal.entities.project import Project
-19from projectal.entities.project_template import ProjectTemplate
-20from projectal.entities.rebate import Rebate
-21from projectal.entities.resource import Resource
-22from projectal.entities.skill import Skill
-23from projectal.entities.staff import Staff
-24from projectal.entities.stage import Stage
-25from projectal.entities.tag import Tag
-26from projectal.entities.task import Task
-27from projectal.entities.task_template import TaskTemplate
-28from projectal.entities.user import User
-29from projectal.entities.webhook import Webhook
+_8from projectal.entities.activity import Activity
+_9from projectal.entities.booking import Booking
+10from projectal.entities.calendar import Calendar
+11from projectal.entities.company import Company
+12from projectal.entities.contact import Contact
+13from projectal.entities.customer import Customer
+14from projectal.entities.department import Department
+15from projectal.entities.file import File
+16from projectal.entities.folder import Folder
+17from projectal.entities.location import Location
+18from projectal.entities.note import Note
+19from projectal.entities.permission import Permission
+20from projectal.entities.project import Project
+21from projectal.entities.project_template import ProjectTemplate
+22from projectal.entities.rebate import Rebate
+23from projectal.entities.resource import Resource
+24from projectal.entities.skill import Skill
+25from projectal.entities.staff import Staff
+26from projectal.entities.stage import Stage
+27from projectal.entities.tag import Tag
+28from projectal.entities.task import Task
+29from projectal.entities.task_template import TaskTemplate
+30from projectal.entities.user import User
+31from projectal.entities.webhook import Webhook
```

### Comparing `projectal-3.1.1/docs/projectal/entity.html` & `projectal-4.0.1/docs/projectal/entity.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/enums.html` & `projectal-4.0.1/docs/projectal/enums.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/errors.html` & `projectal-4.0.1/docs/projectal/errors.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/linkers.html` & `projectal-4.0.1/docs/projectal/linkers.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/profile.html` & `projectal-4.0.1/docs/projectal/profile.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal.html` & `projectal-4.0.1/docs/projectal.html`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,29 @@
 details = projectal.auth_details()
 </code></pre>
 
 <hr />
 
 <h2 id="changelog">Changelog</h2>
 
+<h3 id="401">4.0.1</h3>
+
+<ul>
+<li>Minimum Projectal version is now 4.0.0.</li>
+</ul>
+
+<h3 id="400">4.0.0</h3>
+
+<p>Version 4.0.0 accompanies the release of Projectal 4.0.</p>
+
+<ul>
+<li><p>Added the <code>Activity</code> entity, new in Projectal 4.0.</p></li>
+<li><p>Added the <code>Booking</code> entity, new in Projectal 4.0.</p></li>
+</ul>
+
 <h3 id="311">3.1.1</h3>
 
 <ul>
 <li>Link requests generated by 'projectal.Entity.create()' and 'projectal.Entity.update()' are now
 executed in batches. This is enabled by default with the 'batch_linking=True' parameter and can
 be disabled to execute each link request individually. It is recommended to leave this parameter
 enabled as this can greatly reduce the number of network requests.</li>
@@ -511,403 +526,414 @@
 </span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a><span class="sd">details = projectal.auth_details()</span>
 </span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a><span class="sd">```</span>
 </span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>
 </span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="sd">----</span>
 </span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
 </span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a><span class="sd">## Changelog</span>
 </span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a><span class="sd">### 3.1.1</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="sd">- Link requests generated by &#39;projectal.Entity.create()&#39; and &#39;projectal.Entity.update()&#39; are now</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a><span class="sd">  executed in batches. This is enabled by default with the &#39;batch_linking=True&#39; parameter and can</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a><span class="sd">  be disabled to execute each link request individually. It is recommended to leave this parameter</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a><span class="sd">  enabled as this can greatly reduce the number of network requests.</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="sd">### 3.1.0</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="sd">- Minimum Projectal version is now 3.1.5.</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a><span class="sd">### 4.0.1</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="sd">- Minimum Projectal version is now 4.0.0.</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a><span class="sd">### 4.0.0</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a><span class="sd">Version 4.0.0 accompanies the release of Projectal 4.0.</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="sd">- Added the `Activity` entity, new in Projectal 4.0.</span>
 </span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="sd">- Added `projectal.Webhook.list_events()`. See API doc for details on how to use.</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="sd">- Added the `Booking` entity, new in Projectal 4.0.</span>
 </span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">- Added `deleted_at` parameter to `projectal.Entity.get()`. This value should be a UTC timestamp</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="sd">  from a webhook delete event.</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD service configured in</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a><span class="sd">  the Projectal server settings.</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">### 3.1.1</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="sd">- Link requests generated by &#39;projectal.Entity.create()&#39; and &#39;projectal.Entity.update()&#39; are now</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="sd">  executed in batches. This is enabled by default with the &#39;batch_linking=True&#39; parameter and can</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">  be disabled to execute each link request individually. It is recommended to leave this parameter</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a><span class="sd">  enabled as this can greatly reduce the number of network requests.</span>
 </span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="sd">- Enhanced output of `projectal.Entity.changes()` function when reporting link changes.</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="sd">  It no longer dumps the entire before-and-after list with the full content of each linked entity.</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a><span class="sd">  Now reports three lists: `added`, `updated`, `removed`. Entities within the `updated` list</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a><span class="sd">  follow the same `old` vs `new` dictionary model for the data attributes within them. E.g:</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="sd">### 3.1.0</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="sd">- Minimum Projectal version is now 3.1.5.</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a><span class="sd">- Added `projectal.Webhook.list_events()`. See API doc for details on how to use.</span>
 </span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a><span class="sd">    ```</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="sd">    resourceList: [</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="sd">        &#39;added&#39;: [],</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="sd">        &#39;updated&#39;: [</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="sd">            {&#39;uuId&#39;: &#39;14eb4c31-0f92-49d1-8b4d-507ab939003e&#39;, &#39;resourceLink&#39;: {&#39;utilization&#39;: {&#39;old&#39;: 0.1, &#39;new&#39;: 0.9}}},</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="sd">        ],</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a><span class="sd">        &#39;removed&#39;: []</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="sd">    ]</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="sd">    ```</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="sd">  This should result in slimmer logs that are much easier to understand as the changes are</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="sd">  clearly indicated.</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">### 3.0.2</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="sd">- Added `projectal.Entity.get_link_definitions()`. Exposes entity link definition dictionary.</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">  Consumers can inspect which links an Entity knows about and their internal settings.</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="sd">  Link definitions that appear here are the links valid for `links=[]` parameters.</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="sd">### 3.0.1</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">- Fixed fetching project with links=[&#39;task&#39;] not being available.</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a><span class="sd">- Improved Permission.list(). Now returns a dict with the permission name as</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a><span class="sd">  key with Permission objects as the value (instead of list of uuIds).</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a><span class="sd">- Added `deleted_at` parameter to `projectal.Entity.get()`. This value should be a UTC timestamp</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="sd">  from a webhook delete event.</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="sd">- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD service configured in</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="sd">  the Projectal server settings.</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a><span class="sd">- Enhanced output of `projectal.Entity.changes()` function when reporting link changes.</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="sd">  It no longer dumps the entire before-and-after list with the full content of each linked entity.</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="sd">  Now reports three lists: `added`, `updated`, `removed`. Entities within the `updated` list</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="sd">  follow the same `old` vs `new` dictionary model for the data attributes within them. E.g:</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="sd">    ```</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">    resourceList: [</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="sd">        &#39;added&#39;: [],</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">        &#39;updated&#39;: [</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="sd">            {&#39;uuId&#39;: &#39;14eb4c31-0f92-49d1-8b4d-507ab939003e&#39;, &#39;resourceLink&#39;: {&#39;utilization&#39;: {&#39;old&#39;: 0.1, &#39;new&#39;: 0.9}}},</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">        ],</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="sd">        &#39;removed&#39;: []</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">    ]</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">    ```</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a><span class="sd">  This should result in slimmer logs that are much easier to understand as the changes are</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a><span class="sd">  clearly indicated.</span>
 </span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="sd">- Added a way to use the aliasing feature of the API (new in Projectal 3.0).</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="sd">Set `projectal.api_alias = &#39;uuid&#39;` to the UUID of a User object and all</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="sd">requests made will be done as that user. Restore this value to None to resume</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="sd">normal operation. (Some rules and limitations apply. See API for more details.)</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="sd">### 3.0.2</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="sd">- Added `projectal.Entity.get_link_definitions()`. Exposes entity link definition dictionary.</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="sd">  Consumers can inspect which links an Entity knows about and their internal settings.</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="sd">  Link definitions that appear here are the links valid for `links=[]` parameters.</span>
 </span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">- Added complete support for the Tags entity (including linkers).</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">### 3.0</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">Version 3.0 accompanies the release of Projectal 3.0.</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">### 3.0.1</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="sd">- Fixed fetching project with links=[&#39;task&#39;] not being available.</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="sd">- Improved Permission.list(). Now returns a dict with the permission name as</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">  key with Permission objects as the value (instead of list of uuIds).</span>
 </span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">**Breaking changes**:</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">- The `links` parameter on `Entity` functions now consumes a list of entity</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a><span class="sd">  names instead of a comma-separated string. For example:</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">- Added a way to use the aliasing feature of the API (new in Projectal 3.0).</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="sd">Set `projectal.api_alias = &#39;uuid&#39;` to the UUID of a User object and all</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">requests made will be done as that user. Restore this value to None to resume</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a><span class="sd">normal operation. (Some rules and limitations apply. See API for more details.)</span>
 </span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a><span class="sd">    ```</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="sd">    # Before:</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=&#39;skill,location&#39;)  # No longer valid</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="sd">    # Now:</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;, &#39;location&#39;])</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="sd">    ```</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="sd">- The `projectal.enums.SkillLevel` enum has had all values renamed to match the new values</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="sd">  used in Projectal (Junior, Mid, Senior). This includes the properties on</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">  Skill entities indicating work time for auto-scheduling (now `juniorLevel`,</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="sd">  `midLevel`, `seniorLevel`).</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a><span class="sd">- Working with entity links has changed in this release. The previous methods</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a><span class="sd">  are still available and continue to work as before, but there is no need</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="sd">  to interact with the `projectal.linkers` methods yourself anymore.</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a><span class="sd">- Added complete support for the Tags entity (including linkers).</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a><span class="sd">### 3.0</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="sd">Version 3.0 accompanies the release of Projectal 3.0.</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="sd">**Breaking changes**:</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="sd">- The `links` parameter on `Entity` functions now consumes a list of entity</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">  names instead of a comma-separated string. For example:</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="sd">    ```</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a><span class="sd">    # Before:</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=&#39;skill,location&#39;)  # No longer valid</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a><span class="sd">    # Now:</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;, &#39;location&#39;])</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="sd">    ```</span>
 </span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="sd">  You can now modify the list of links within an entity and save the entity</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">  directly. The library will automatically determine how the links have been</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">  modified and issue the correct linker methods on your behalf. E.g.,</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">  you can now do:</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="sd">- The `projectal.enums.SkillLevel` enum has had all values renamed to match the new values</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">  used in Projectal (Junior, Mid, Senior). This includes the properties on</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">  Skill entities indicating work time for auto-scheduling (now `juniorLevel`,</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">  `midLevel`, `seniorLevel`).</span>
 </span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="sd">    ```</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="sd">    staff = projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;])</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">    staff[&#39;firstName&#39;] = &quot;New name&quot;  # Field update</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">    staff[&#39;skillList&#39;] = [skill1, skill2, skill3]  # Link update</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="sd">    staff.save()  # Both changes are saved</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="sd">**Other changes**:</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">- Working with entity links has changed in this release. The previous methods</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">  are still available and continue to work as before, but there is no need</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="sd">  to interact with the `projectal.linkers` methods yourself anymore.</span>
 </span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">    task = projectal.Task.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;stage&#39;])</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a><span class="sd">    task[&#39;stage&#39;] = stage1  # Uses a single object instead of list</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="sd">    task.save()</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="sd">    ```</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">  You can now modify the list of links within an entity and save the entity</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a><span class="sd">  directly. The library will automatically determine how the links have been</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="sd">  modified and issue the correct linker methods on your behalf. E.g.,</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="sd">  you can now do:</span>
 </span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="sd">  See `examples/linking.py` for a more complete demonstration of linking</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a><span class="sd">  capabilities and limitations.</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a><span class="sd">- Linkers (`projectal.linkers`) can now be given a list of Entities (of one</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd"> type) to link/unlink/relink in bulk. E.g:</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">    ```</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">    staff.unlink_skill(skill1)  # Before</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">    staff.unlink_skill([skill1, skill2, skill3])  # This works now too</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">    ```</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">- Linkers now strip the payload to only the required fields instead of passing</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">  on the entire Entity object. This cuts down on network traffic significantly.</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">- Linkers now also work in reverse. The Projectal server currently only supports</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="sd">  linking entities in one direction (e.g., Company to Staff), which often means</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a><span class="sd">  writing something like:</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="sd">    ```</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a><span class="sd">    staff = projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;])</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="sd">    staff[&#39;firstName&#39;] = &quot;New name&quot;  # Field update</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a><span class="sd">    staff[&#39;skillList&#39;] = [skill1, skill2, skill3]  # Link update</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd">    staff.save()  # Both changes are saved</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">    task = projectal.Task.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;stage&#39;])</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">    task[&#39;stage&#39;] = stage1  # Uses a single object instead of list</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">    task.save()</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">    ```</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">  See `examples/linking.py` for a more complete demonstration of linking</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">  capabilities and limitations.</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="sd">- Linkers (`projectal.linkers`) can now be given a list of Entities (of one</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a><span class="sd"> type) to link/unlink/relink in bulk. E.g:</span>
 </span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a><span class="sd">    ```</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a><span class="sd">    staff.link_location(location)</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a><span class="sd">    company.link_staff(staff)</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a><span class="sd">    staff.unlink_skill(skill1)  # Before</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a><span class="sd">    staff.unlink_skill([skill1, skill2, skill3])  # This works now too</span>
 </span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a><span class="sd">    ```</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a><span class="sd">  The change in direction is not very intuitive and would require you to constantly</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a><span class="sd">  verify which direction is the one available to you in the documentation.</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a><span class="sd">  Reverse linkers hide this from you and figure out the direction of the relationship</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a><span class="sd">  for you behind the scenes. So now this is possible, even though the API doesn&#39;t</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a><span class="sd">  strictly support it:</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a><span class="sd">    ```</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a><span class="sd">    staff.link_location(location)</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">    staff.link_company(company)</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a><span class="sd">    ```</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a><span class="sd">    Caveat: the documentation for Staff will not list Company links. You will still</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a><span class="sd">    have to look up the Company documentation for the link description.</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a><span class="sd">- Requesting entity links with the `links=` parameter will now always ensure the</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a><span class="sd">  link field (e.g., `taskList`) exists in the result, even if there are no links.</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a><span class="sd">  The server may not always return a value, but we can use a default value ([] for</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a><span class="sd">  lists, None for dicts).</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a><span class="sd">- Added a `Permission` entity to correctly type Permissions in responses.</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">- Added a `Tag` entity, new in Projectal 3.0.</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="sd">- Added `links` parameter to `Company.get_primary_company()`</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a><span class="sd">- Linkers now strip the payload to only the required fields instead of passing</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a><span class="sd">  on the entire Entity object. This cuts down on network traffic significantly.</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a><span class="sd">- Linkers now also work in reverse. The Projectal server currently only supports</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a><span class="sd">  linking entities in one direction (e.g., Company to Staff), which often means</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a><span class="sd">  writing something like:</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a><span class="sd">    ```</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">    staff.link_location(location)</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a><span class="sd">    company.link_staff(staff)</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a><span class="sd">    ```</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a><span class="sd">  The change in direction is not very intuitive and would require you to constantly</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="sd">  verify which direction is the one available to you in the documentation.</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a><span class="sd">  Reverse linkers hide this from you and figure out the direction of the relationship</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a><span class="sd">  for you behind the scenes. So now this is possible, even though the API doesn&#39;t</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a><span class="sd">  strictly support it:</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a><span class="sd">    ```</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a><span class="sd">    staff.link_location(location)</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">    staff.link_company(company)</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">    ```</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a><span class="sd">    Caveat: the documentation for Staff will not list Company links. You will still</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="sd">    have to look up the Company documentation for the link description.</span>
 </span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a><span class="sd">- `Department.tree()`: now consumes a `holder` Entity object instead</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">  of a uuId.</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a><span class="sd">- `Department.tree()`: added `generic_staff` parameter, new in</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a><span class="sd">  Projectal 3.0.</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a><span class="sd">- Don&#39;t break on trailing slash in Projectal URL</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">- When creating tasks, populate the `projectRef` and `parent` fields in the</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a><span class="sd">  returned Task object.</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a><span class="sd">- Requesting entity links with the `links=` parameter will now always ensure the</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">  link field (e.g., `taskList`) exists in the result, even if there are no links.</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a><span class="sd">  The server may not always return a value, but we can use a default value ([] for</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a><span class="sd">  lists, None for dicts).</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a><span class="sd">- Added a `Permission` entity to correctly type Permissions in responses.</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a><span class="sd">- Added a `Tag` entity, new in Projectal 3.0.</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a><span class="sd">- Added `links` parameter to `Company.get_primary_company()`</span>
 </span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">- Added convenience functions for matching on fields where you only want</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">  one result (e.g match_one()) which return the first match found.</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">- `Department.tree()`: now consumes a `holder` Entity object instead</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">  of a uuId.</span>
 </span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">- Update the entity `history()` method for Projectal 3.0. Some new parameters</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a><span class="sd">  allow you to restrict the history to a particular range or to get only the</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a><span class="sd">  changes for a webhook timestamp.</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a><span class="sd">- Entity objects can call `.history()` on themselves.</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="sd">- The library now keeps a reference to the User account that is currently logged</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">  in and using the API: `projectal.api_auth_details`.</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a><span class="sd">**Known issues**:</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">- You cannot save changes to Notes or Calendars via their holding entity. You</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="sd">  must save the changes on the Note or Calendar directly. To illustrate:</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">  ```</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a><span class="sd">  staff = projectal.Staff.get(&lt;uuid&gt;, links=[&#39;calendar&#39;])</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a><span class="sd">  calendar = staff[&#39;calendarList&#39;][0]</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="sd">  calendar[&#39;name&#39;] = &#39;Calendar 2&#39;</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">- `Department.tree()`: added `generic_staff` parameter, new in</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a><span class="sd">  Projectal 3.0.</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a><span class="sd">- Don&#39;t break on trailing slash in Projectal URL</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">- When creating tasks, populate the `projectRef` and `parent` fields in the</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="sd">  returned Task object.</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">- Added convenience functions for matching on fields where you only want</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a><span class="sd">  one result (e.g match_one()) which return the first match found.</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="sd">- Update the entity `history()` method for Projectal 3.0. Some new parameters</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">  allow you to restrict the history to a particular range or to get only the</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a><span class="sd">  changes for a webhook timestamp.</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="sd">- Entity objects can call `.history()` on themselves.</span>
 </span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="sd">  # Cannot do this - will not pick up the changes</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">  staff.save()</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="sd">- The library now keeps a reference to the User account that is currently logged</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">  in and using the API: `projectal.api_auth_details`.</span>
 </span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a><span class="sd">  # You must do this for now</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">  calendar.save()</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="sd">  ```</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">  This will be resolved in a future release.</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="sd">- When creating Notes, the `created` and `modified` values may differ by</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a><span class="sd">  1ms in the object you have a reference to compared to what is actually</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="sd">  stored in the database.</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="sd">- Duration calculation is not precise yet (mentioned in 2.1.0)</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a><span class="sd">**Known issues**:</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">- You cannot save changes to Notes or Calendars via their holding entity. You</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="sd">  must save the changes on the Note or Calendar directly. To illustrate:</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">  ```</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a><span class="sd">  staff = projectal.Staff.get(&lt;uuid&gt;, links=[&#39;calendar&#39;])</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="sd">  calendar = staff[&#39;calendarList&#39;][0]</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a><span class="sd">  calendar[&#39;name&#39;] = &#39;Calendar 2&#39;</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">  # Cannot do this - will not pick up the changes</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="sd">  staff.save()</span>
 </span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">### 2.1.0</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">**Breaking changes**:</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">- Getting location calendar is now done on an instance instead of class. So</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">- The `CompanyType.Master` enum has been replaced with `CompanyType.Primary`.</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">  This was a leftover reference to the Master Company which was renamed in</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">  Projectal several versions ago.</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">- Date conversion functions return None when given None or empty string</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">- Added `Task.reset_duration()` as a basic duration calculator for tasks.</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a><span class="sd">  This is a work-in-progress and will be gradually improved. The duration</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">  calculator takes into consideration the location to remove non-work</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">  days from the estimate of working duration. It currently does not work</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">  for the time component or `isWorking=True` exceptions.</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="sd">- Change detection in `Entity.changes()` now excludes cases where the</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a><span class="sd">  server has no value and the new value is None. Saving this change has</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">  no effect and would always detect a change until a non-None value is</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="sd">  set, which is noisy and generates more network activity.</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a><span class="sd">### 2.0.3</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a><span class="sd">- Better support for calendars.</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a><span class="sd">  - Distinguish between calendar containers (&quot;Calendar&quot;) and the</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="sd">    calendar items within them (&quot;CalendarItem&quot;).</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a><span class="sd">  - Allow CalendarItems to be saved directly. E.G item.save()</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a><span class="sd">- Fix &#39;holder&#39; parameter in contact/staff/location/task_template not</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a><span class="sd">  permitting object type. Now consumes uuId or object to match rest of</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="sd">  the library.</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a><span class="sd">- `Entity.changes()` has been extended with an `old=True` flag. When</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="sd">  this flag is true, the set of changes will now return both the original</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a><span class="sd">  and the new values. E.g.</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a><span class="sd">```</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a><span class="sd">task.changes()</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a><span class="sd"># {&#39;name&#39;: &#39;current&#39;}</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a><span class="sd">task.changes(old=True)</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a><span class="sd"># {&#39;name&#39;: {&#39;old&#39;: &#39;original&#39;, &#39;new&#39;: &#39;current&#39;}}</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a><span class="sd">```</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a><span class="sd">- Fixed entity link cache causing errors when deleting a link from an entity</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a><span class="sd">  which has not been fetched with links (deleting from empty list).</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a><span class="sd">### 2.0.2</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a><span class="sd">- Fixed updating Webhook entities</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a><span class="sd">### 2.0.1</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a><span class="sd">- Fixed application ID not being used correctly.</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a><span class="sd">### 2.0.0</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="sd">- Version 2.0 accompanies the release of Projectal 2.0. There are no major changes</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a><span class="sd">  since the previous release.</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a><span class="sd">- Expose `Entity.changes()` function. It returns a list of fields on an entity that</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a><span class="sd">  have changed since fetching it. These are the changes that will be sent over to the</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a><span class="sd">  server when an update request is made.</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a><span class="sd">- Added missing &#39;packaging&#39; dependency to requirements.</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">  # You must do this for now</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">  calendar.save()</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">  ```</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">  This will be resolved in a future release.</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">- When creating Notes, the `created` and `modified` values may differ by</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">  1ms in the object you have a reference to compared to what is actually</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">  stored in the database.</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">- Duration calculation is not precise yet (mentioned in 2.1.0)</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a><span class="sd">### 2.1.0</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">**Breaking changes**:</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">- Getting location calendar is now done on an instance instead of class. So</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="sd">- The `CompanyType.Master` enum has been replaced with `CompanyType.Primary`.</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a><span class="sd">  This was a leftover reference to the Master Company which was renamed in</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">  Projectal several versions ago.</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a><span class="sd">**Other changes**:</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a><span class="sd">- Date conversion functions return None when given None or empty string</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a><span class="sd">- Added `Task.reset_duration()` as a basic duration calculator for tasks.</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a><span class="sd">  This is a work-in-progress and will be gradually improved. The duration</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="sd">  calculator takes into consideration the location to remove non-work</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a><span class="sd">  days from the estimate of working duration. It currently does not work</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a><span class="sd">  for the time component or `isWorking=True` exceptions.</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a><span class="sd">- Change detection in `Entity.changes()` now excludes cases where the</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="sd">  server has no value and the new value is None. Saving this change has</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a><span class="sd">  no effect and would always detect a change until a non-None value is</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="sd">  set, which is noisy and generates more network activity.</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a><span class="sd">### 2.0.3</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a><span class="sd">- Better support for calendars.</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a><span class="sd">  - Distinguish between calendar containers (&quot;Calendar&quot;) and the</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a><span class="sd">    calendar items within them (&quot;CalendarItem&quot;).</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a><span class="sd">  - Allow CalendarItems to be saved directly. E.G item.save()</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a><span class="sd">- Fix &#39;holder&#39; parameter in contact/staff/location/task_template not</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a><span class="sd">  permitting object type. Now consumes uuId or object to match rest of</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a><span class="sd">  the library.</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a><span class="sd">- `Entity.changes()` has been extended with an `old=True` flag. When</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a><span class="sd">  this flag is true, the set of changes will now return both the original</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a><span class="sd">  and the new values. E.g.</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a><span class="sd">```</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a><span class="sd">task.changes()</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a><span class="sd"># {&#39;name&#39;: &#39;current&#39;}</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a><span class="sd">task.changes(old=True)</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a><span class="sd"># {&#39;name&#39;: {&#39;old&#39;: &#39;original&#39;, &#39;new&#39;: &#39;current&#39;}}</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="sd">```</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a><span class="sd">- Fixed entity link cache causing errors when deleting a link from an entity</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a><span class="sd">  which has not been fetched with links (deleting from empty list).</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a><span class="sd">### 2.0.2</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a><span class="sd">- Fixed updating Webhook entities</span>
 </span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a><span class="sd">### 1.2.0</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="sd">**Breaking changes**:</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a><span class="sd">- Renamed `request_timestamp` to `response_timestamp` to better reflect its purpose.</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a><span class="sd">- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been reverted.</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a><span class="sd">  All date fields returned from the server remain as UTC timestamps.</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a><span class="sd">  The reason is that date fields on tasks contain a time component and converting them</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a><span class="sd">  into date strings was erasing the time, resulting in a value that does not match</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a><span class="sd">  the database.</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a><span class="sd">  Note: the server supports setting date fields using a date string like `2022-04-05`.</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">  You may use this if you prefer but the server will always return a timestamp.</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a><span class="sd">### 2.0.1</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a><span class="sd">- Fixed application ID not being used correctly.</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a><span class="sd">### 2.0.0</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a><span class="sd">- Version 2.0 accompanies the release of Projectal 2.0. There are no major changes</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a><span class="sd">  since the previous release.</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a><span class="sd">- Expose `Entity.changes()` function. It returns a list of fields on an entity that</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a><span class="sd">  have changed since fetching it. These are the changes that will be sent over to the</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a><span class="sd">  server when an update request is made.</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a><span class="sd">- Added missing &#39;packaging&#39; dependency to requirements.</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a><span class="sd">### 1.2.0</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">**Breaking changes**:</span>
 </span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">  Note: we provide utility functions for easily converting dates from/to</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a><span class="sd">  timestamps expected by the Projectal server. See:</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and</span>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a><span class="sd">  `projectal.timestamp_from_datetime()`.</span>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a><span class="sd">- Implement request chunking - for methods that consume a list of entities, we now</span>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a><span class="sd">  automatically batch them up into multiple requests to prevent timeouts on really</span>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">  large request. Values are configurable through</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a><span class="sd">  `projectal.chunk_size_read` and `projectal.chunk_size_write`.</span>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a><span class="sd">  Default values: Read: 1000 items. Write: 200 items.</span>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="sd">- Added profile get/set functions on entities for easier use. Now you only need to supply</span>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="sd">  the key and the data. E.g:</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a><span class="sd">```</span>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a><span class="sd">key = &#39;hr_connector&#39;</span>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a><span class="sd">data = {&#39;staff_source&#39;: &#39;company_z&#39;}</span>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a><span class="sd">task.profile_set(key, data)</span>
-</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a><span class="sd">```</span>
-</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>
-</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a><span class="sd">- Entity link methods now automatically update the entity&#39;s cached list of links. E.g:</span>
-</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a><span class="sd">  a task fetched with staff links will have `task[&#39;staffList&#39;] = [Staff1,Staff2]`.</span>
-</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="sd">  Before, doing a `task.link_staff(staff)` did not modify the list to reflect the</span>
-</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a><span class="sd">  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same applies for update</span>
-</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a><span class="sd">  and delete.</span>
-</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>
-</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a><span class="sd">  This allows you to modify links and continue working with that object without having</span>
-</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a><span class="sd">  to fetch it again to obtain the most recent link data. Be aware that if you acquire</span>
-</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="sd">  the object without requesting the link data as well</span>
-</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a><span class="sd">  (e.g: `projectal.Task.get(id, links=&#39;STAFF&#39;)`),</span>
-</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a><span class="sd">  these lists will not accurately reflect what&#39;s in the database, only the changes made</span>
-</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a><span class="sd">  while the object is held.</span>
-</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a>
-</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a><span class="sd">- Support new `applicationId` property on login. Set with: `projectal.api_application_id`.</span>
-</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a><span class="sd">  The application ID is sent back to you in webhooks so you know which application was</span>
-</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a><span class="sd">  the source of the event (and you can choose to filter them accordingly).</span>
-</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a><span class="sd">- Added `Entity.set_readonly()` to allow setting values on entities that will not</span>
-</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a><span class="sd">  be sent over to the server when updating/saving the entity.</span>
-</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a>
-</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a><span class="sd">  The main use case for this is to populate cached entities which you have just created</span>
-</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a><span class="sd">  with values you already know about. This is mainly a workaround for the limitation of</span>
-</span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a><span class="sd">  the server not sending the full object back after creating it, resulting in the client</span>
-</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a><span class="sd">  needing to fetch the object in full again if it needs some of the fields set by the</span>
-</span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a><span class="sd">  server after creation.</span>
-</span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a>
-</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a><span class="sd">  Additionally, some read-only fields will generate an error on the server if</span>
-</span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a><span class="sd">  included in the update request. This method lets you set these values on newly</span>
-</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a><span class="sd">  created objects without triggering this error.</span>
-</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a>
-</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a><span class="sd">  A common example is setting the `projectRef` of a task you just created.</span>
-</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a>
-</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a>
-</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a><span class="sd">### 1.1.1</span>
-</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a><span class="sd">- Add support for &#39;profiles&#39; API. Profiles are a type of key-value storage that target</span>
-</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a><span class="sd">  any entity. Not currently documented.</span>
-</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a><span class="sd">- Fix handling error message parsing in ProjectalException for batch create operation</span>
-</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a><span class="sd">- Add `Task.update_order()` to set task order</span>
-</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a><span class="sd">- Return empty list when GETing empty list instead of failing (no request to server)</span>
-</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a><span class="sd">- Expose the timestamp returned by requests that modify the database. Use</span>
-</span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a><span class="sd">  `projectal.request_timestamp` to get the value of the most recent request (None</span>
-</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a><span class="sd">  if no timestamp in response)</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">- Renamed `request_timestamp` to `response_timestamp` to better reflect its purpose.</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a><span class="sd">- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been reverted.</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">  All date fields returned from the server remain as UTC timestamps.</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">  The reason is that date fields on tasks contain a time component and converting them</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a><span class="sd">  into date strings was erasing the time, resulting in a value that does not match</span>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a><span class="sd">  the database.</span>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">  Note: the server supports setting date fields using a date string like `2022-04-05`.</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a><span class="sd">  You may use this if you prefer but the server will always return a timestamp.</span>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="sd">  Note: we provide utility functions for easily converting dates from/to</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="sd">  timestamps expected by the Projectal server. See:</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a><span class="sd">  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a><span class="sd">  `projectal.timestamp_from_datetime()`.</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a><span class="sd">**Other changes**:</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a><span class="sd">- Implement request chunking - for methods that consume a list of entities, we now</span>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a><span class="sd">  automatically batch them up into multiple requests to prevent timeouts on really</span>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a><span class="sd">  large request. Values are configurable through</span>
+</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a><span class="sd">  `projectal.chunk_size_read` and `projectal.chunk_size_write`.</span>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a><span class="sd">  Default values: Read: 1000 items. Write: 200 items.</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="sd">- Added profile get/set functions on entities for easier use. Now you only need to supply</span>
+</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a><span class="sd">  the key and the data. E.g:</span>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a><span class="sd">```</span>
+</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a><span class="sd">key = &#39;hr_connector&#39;</span>
+</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a><span class="sd">data = {&#39;staff_source&#39;: &#39;company_z&#39;}</span>
+</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="sd">task.profile_set(key, data)</span>
+</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a><span class="sd">```</span>
+</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a>
+</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a><span class="sd">- Entity link methods now automatically update the entity&#39;s cached list of links. E.g:</span>
+</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a><span class="sd">  a task fetched with staff links will have `task[&#39;staffList&#39;] = [Staff1,Staff2]`.</span>
+</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a><span class="sd">  Before, doing a `task.link_staff(staff)` did not modify the list to reflect the</span>
+</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a><span class="sd">  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same applies for update</span>
+</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a><span class="sd">  and delete.</span>
+</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a>
+</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a><span class="sd">  This allows you to modify links and continue working with that object without having</span>
+</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a><span class="sd">  to fetch it again to obtain the most recent link data. Be aware that if you acquire</span>
+</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a><span class="sd">  the object without requesting the link data as well</span>
+</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a><span class="sd">  (e.g: `projectal.Task.get(id, links=&#39;STAFF&#39;)`),</span>
+</span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a><span class="sd">  these lists will not accurately reflect what&#39;s in the database, only the changes made</span>
+</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a><span class="sd">  while the object is held.</span>
+</span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a>
+</span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a><span class="sd">- Support new `applicationId` property on login. Set with: `projectal.api_application_id`.</span>
+</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a><span class="sd">  The application ID is sent back to you in webhooks so you know which application was</span>
+</span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a><span class="sd">  the source of the event (and you can choose to filter them accordingly).</span>
+</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a><span class="sd">- Added `Entity.set_readonly()` to allow setting values on entities that will not</span>
+</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a><span class="sd">  be sent over to the server when updating/saving the entity.</span>
+</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a>
+</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a><span class="sd">  The main use case for this is to populate cached entities which you have just created</span>
+</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a><span class="sd">  with values you already know about. This is mainly a workaround for the limitation of</span>
+</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a><span class="sd">  the server not sending the full object back after creating it, resulting in the client</span>
+</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a><span class="sd">  needing to fetch the object in full again if it needs some of the fields set by the</span>
+</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a><span class="sd">  server after creation.</span>
+</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a>
+</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a><span class="sd">  Additionally, some read-only fields will generate an error on the server if</span>
+</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a><span class="sd">  included in the update request. This method lets you set these values on newly</span>
+</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a><span class="sd">  created objects without triggering this error.</span>
+</span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a>
+</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a><span class="sd">  A common example is setting the `projectRef` of a task you just created.</span>
 </span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a>
-</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a><span class="sd">### 1.1.0</span>
-</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a><span class="sd">- Minimum Projectal version is now 1.9.4.</span>
-</span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a>
-</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a><span class="sd">**Breaking changes**:</span>
-</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a><span class="sd">- Entity `list()` now returns a list of UUIDs instead of full objects. You may provide</span>
-</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a><span class="sd">  an `expand` parameter to restore the previous behavior: `Entity.list(expand=True)`.</span>
-</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a><span class="sd">  This change is made for performance reasons where you may have thousands of tasks</span>
-</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a><span class="sd">  and getting them all may time out. For those cases, we suggest writing a query to filter</span>
-</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a><span class="sd">  down to only the tasks and fields you need.</span>
-</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a><span class="sd">- `Company.get_master_company()` has been renamed to `Company.get_primary_company()`</span>
-</span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a><span class="sd">  to match the server.</span>
-</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a><span class="sd">- The following date fields are converted into date strings upon fetch:</span>
-</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a><span class="sd">  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.</span>
-</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a><span class="sd">  These fields are added or updated using date strings (like `2022-03-02`), but the</span>
-</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a><span class="sd">  server returns timestamps (e.g: 1646006400000) upon fetch, which is confusing. This</span>
-</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a><span class="sd">  change ensures they are always date strings for consistency.</span>
-</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a>
-</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a><span class="sd">- When updating an entity, only the fields that have changed are sent to the server. When</span>
-</span><span id="L-361"><a href="#L-361"><span class="linenos">361</span></a><span class="sd">  updating a list of entities, unmodified entities are not sent to the server at all. This</span>
-</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a><span class="sd">  dramatically reduces the payload size and should speed things up.</span>
-</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a><span class="sd">- When fetching entities, entity links are now typed as well. E.g. `project[&#39;rebateList&#39;]`</span>
-</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a><span class="sd">  contains a list of `Rebate` instead of `dict`.</span>
-</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a><span class="sd">- Added `date_from_timestamp()` and `timestamp_from_date()` functions to help with</span>
-</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a><span class="sd">  converting to/from dates and Projectal timestamps.</span>
-</span><span id="L-367"><a href="#L-367"><span class="linenos">367</span></a><span class="sd">- Entity history now uses `desc` by default (index 0 is newest)</span>
-</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a><span class="sd">- Added `Project.tasks()` to list all task UUIDs within a project.</span>
+</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a>
+</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a><span class="sd">### 1.1.1</span>
+</span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a><span class="sd">- Add support for &#39;profiles&#39; API. Profiles are a type of key-value storage that target</span>
+</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a><span class="sd">  any entity. Not currently documented.</span>
+</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a><span class="sd">- Fix handling error message parsing in ProjectalException for batch create operation</span>
+</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a><span class="sd">- Add `Task.update_order()` to set task order</span>
+</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a><span class="sd">- Return empty list when GETing empty list instead of failing (no request to server)</span>
+</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a><span class="sd">- Expose the timestamp returned by requests that modify the database. Use</span>
+</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a><span class="sd">  `projectal.request_timestamp` to get the value of the most recent request (None</span>
+</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a><span class="sd">  if no timestamp in response)</span>
+</span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a>
+</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a><span class="sd">### 1.1.0</span>
+</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a><span class="sd">- Minimum Projectal version is now 1.9.4.</span>
+</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a>
+</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a><span class="sd">**Breaking changes**:</span>
+</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a><span class="sd">- Entity `list()` now returns a list of UUIDs instead of full objects. You may provide</span>
+</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a><span class="sd">  an `expand` parameter to restore the previous behavior: `Entity.list(expand=True)`.</span>
+</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a><span class="sd">  This change is made for performance reasons where you may have thousands of tasks</span>
+</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a><span class="sd">  and getting them all may time out. For those cases, we suggest writing a query to filter</span>
+</span><span id="L-361"><a href="#L-361"><span class="linenos">361</span></a><span class="sd">  down to only the tasks and fields you need.</span>
+</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a><span class="sd">- `Company.get_master_company()` has been renamed to `Company.get_primary_company()`</span>
+</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a><span class="sd">  to match the server.</span>
+</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a><span class="sd">- The following date fields are converted into date strings upon fetch:</span>
+</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a><span class="sd">  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.</span>
+</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a><span class="sd">  These fields are added or updated using date strings (like `2022-03-02`), but the</span>
+</span><span id="L-367"><a href="#L-367"><span class="linenos">367</span></a><span class="sd">  server returns timestamps (e.g: 1646006400000) upon fetch, which is confusing. This</span>
+</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a><span class="sd">  change ensures they are always date strings for consistency.</span>
 </span><span id="L-369"><a href="#L-369"><span class="linenos">369</span></a>
-</span><span id="L-370"><a href="#L-370"><span class="linenos">370</span></a><span class="sd">### 1.0.3</span>
-</span><span id="L-371"><a href="#L-371"><span class="linenos">371</span></a><span class="sd">- Fix another case of automatic JWT refresh not working</span>
-</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a>
-</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a><span class="sd">### 1.0.2</span>
-</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a><span class="sd">- Entity instances can `save()` or `delete()` on themselves</span>
-</span><span id="L-375"><a href="#L-375"><span class="linenos">375</span></a><span class="sd">- Fix broken `dict` methods (`get()` and `update()`) when called from Entity instances</span>
-</span><span id="L-376"><a href="#L-376"><span class="linenos">376</span></a><span class="sd">- Fix automatic JWT refresh only working in some cases</span>
-</span><span id="L-377"><a href="#L-377"><span class="linenos">377</span></a>
-</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a><span class="sd">### 1.0.1</span>
-</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a><span class="sd">- Added `list()` function for all entities</span>
-</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a><span class="sd">- Added search functions for all entities (match-, search, query)</span>
-</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a><span class="sd">- Added `Company.get_master_company()`</span>
-</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a><span class="sd">- Fixed adding template tasks</span>
+</span><span id="L-370"><a href="#L-370"><span class="linenos">370</span></a><span class="sd">**Other changes**:</span>
+</span><span id="L-371"><a href="#L-371"><span class="linenos">371</span></a><span class="sd">- When updating an entity, only the fields that have changed are sent to the server. When</span>
+</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a><span class="sd">  updating a list of entities, unmodified entities are not sent to the server at all. This</span>
+</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a><span class="sd">  dramatically reduces the payload size and should speed things up.</span>
+</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a><span class="sd">- When fetching entities, entity links are now typed as well. E.g. `project[&#39;rebateList&#39;]`</span>
+</span><span id="L-375"><a href="#L-375"><span class="linenos">375</span></a><span class="sd">  contains a list of `Rebate` instead of `dict`.</span>
+</span><span id="L-376"><a href="#L-376"><span class="linenos">376</span></a><span class="sd">- Added `date_from_timestamp()` and `timestamp_from_date()` functions to help with</span>
+</span><span id="L-377"><a href="#L-377"><span class="linenos">377</span></a><span class="sd">  converting to/from dates and Projectal timestamps.</span>
+</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a><span class="sd">- Entity history now uses `desc` by default (index 0 is newest)</span>
+</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a><span class="sd">- Added `Project.tasks()` to list all task UUIDs within a project.</span>
+</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a>
+</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a><span class="sd">### 1.0.3</span>
+</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a><span class="sd">- Fix another case of automatic JWT refresh not working</span>
 </span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a>
-</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a><span class="kn">import</span> <span class="nn">logging</span>
-</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a><span class="kn">import</span> <span class="nn">os</span>
-</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a>
-</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a><span class="kn">from</span> <span class="nn">projectal.entities</span> <span class="kn">import</span> <span class="o">*</span>
-</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a><span class="kn">from</span> <span class="nn">.api</span> <span class="kn">import</span> <span class="o">*</span>
-</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a><span class="kn">from</span> <span class="nn">.</span> <span class="kn">import</span> <span class="n">profile</span>
-</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a>
-</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a><span class="n">api_base</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_URL&#39;</span><span class="p">)</span>
-</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a><span class="n">api_username</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_USERNAME&#39;</span><span class="p">)</span>
-</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a><span class="n">api_password</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_PASSWORD&#39;</span><span class="p">)</span>
-</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a><span class="n">api_application_id</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a><span class="n">api_auth_details</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a><span class="n">api_alias</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-398"><a href="#L-398"><span class="linenos">398</span></a><span class="n">cookies</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a><span class="n">chunk_size_read</span> <span class="o">=</span> <span class="mi">1000</span>
-</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a><span class="n">chunk_size_write</span> <span class="o">=</span> <span class="mi">200</span>
-</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a>
-</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a><span class="c1"># Records the timestamp generated by the last request (database</span>
-</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a><span class="c1"># event time). These are reported on add or updates; if there is</span>
-</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a><span class="c1"># no timestamp in the response, this is set to None.</span>
-</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a><span class="n">response_timestamp</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a>
-</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a>
-</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a><span class="c1"># The minimum version number of the Projectal instance that this</span>
-</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a><span class="c1"># API client targets. Lower versions are not supported and will</span>
-</span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a><span class="c1"># raise an exception.</span>
-</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a><span class="n">MIN_PROJECTAL_VERSION</span> <span class="o">=</span> <span class="s2">&quot;3.1.5&quot;</span>
+</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a><span class="sd">### 1.0.2</span>
+</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a><span class="sd">- Entity instances can `save()` or `delete()` on themselves</span>
+</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a><span class="sd">- Fix broken `dict` methods (`get()` and `update()`) when called from Entity instances</span>
+</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a><span class="sd">- Fix automatic JWT refresh only working in some cases</span>
+</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a>
+</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a><span class="sd">### 1.0.1</span>
+</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a><span class="sd">- Added `list()` function for all entities</span>
+</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a><span class="sd">- Added search functions for all entities (match-, search, query)</span>
+</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a><span class="sd">- Added `Company.get_master_company()`</span>
+</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a><span class="sd">- Fixed adding template tasks</span>
+</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a>
+</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a><span class="kn">import</span> <span class="nn">logging</span>
+</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a><span class="kn">import</span> <span class="nn">os</span>
+</span><span id="L-398"><a href="#L-398"><span class="linenos">398</span></a>
+</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a><span class="kn">from</span> <span class="nn">projectal.entities</span> <span class="kn">import</span> <span class="o">*</span>
+</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a><span class="kn">from</span> <span class="nn">.api</span> <span class="kn">import</span> <span class="o">*</span>
+</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a><span class="kn">from</span> <span class="nn">.</span> <span class="kn">import</span> <span class="n">profile</span>
+</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a>
+</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a><span class="n">api_base</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_URL&#39;</span><span class="p">)</span>
+</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a><span class="n">api_username</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_USERNAME&#39;</span><span class="p">)</span>
+</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a><span class="n">api_password</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_PASSWORD&#39;</span><span class="p">)</span>
+</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a><span class="n">api_application_id</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a><span class="n">api_auth_details</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a><span class="n">api_alias</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a><span class="n">cookies</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a><span class="n">chunk_size_read</span> <span class="o">=</span> <span class="mi">1000</span>
+</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a><span class="n">chunk_size_write</span> <span class="o">=</span> <span class="mi">200</span>
 </span><span id="L-412"><a href="#L-412"><span class="linenos">412</span></a>
-</span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a><span class="n">__verify</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a>
-</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a><span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s1">&#39;projectal-api-client&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">NullHandler</span><span class="p">())</span>
+</span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a><span class="c1"># Records the timestamp generated by the last request (database</span>
+</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a><span class="c1"># event time). These are reported on add or updates; if there is</span>
+</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a><span class="c1"># no timestamp in the response, this is set to None.</span>
+</span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a><span class="n">response_timestamp</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a>
+</span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a>
+</span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a><span class="c1"># The minimum version number of the Projectal instance that this</span>
+</span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a><span class="c1"># API client targets. Lower versions are not supported and will</span>
+</span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a><span class="c1"># raise an exception.</span>
+</span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a><span class="n">MIN_PROJECTAL_VERSION</span> <span class="o">=</span> <span class="s2">&quot;4.0.0&quot;</span>
+</span><span id="L-423"><a href="#L-423"><span class="linenos">423</span></a>
+</span><span id="L-424"><a href="#L-424"><span class="linenos">424</span></a><span class="n">__verify</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-425"><a href="#L-425"><span class="linenos">425</span></a>
+</span><span id="L-426"><a href="#L-426"><span class="linenos">426</span></a><span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s1">&#39;projectal-api-client&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">NullHandler</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
     </main>
 <script>
     function escapeHTML(html) {
```

#### html2text {}

```diff
@@ -31,14 +31,20 @@
 status = projectal.status()
 
 # Test account credentials
 projectal.login()
 details = projectal.auth_details()
 ===============================================================================
 ***** Changelog *****
+**** 4.0.1 ****
+    * Minimum Projectal version is now 4.0.0.
+**** 4.0.0 ****
+Version 4.0.0 accompanies the release of Projectal 4.0.
+    * Added the Activity entity, new in Projectal 4.0.
+    * Added the Booking entity, new in Projectal 4.0.
 **** 3.1.1 ****
     * Link requests generated by 'projectal.Entity.create()' and
       'projectal.Entity.update()' are now executed in batches. This is enabled
       by default with the 'batch_linking=True' parameter and can be disabled to
       execute each link request individually. It is recommended to leave this
       parameter enabled as this can greatly reduce the number of network
       requests.
@@ -345,476 +351,487 @@
 _20details = projectal.auth_details()
 _21```
 _22
 _23----
 _24
 _25## Changelog
 _26
-_27### 3.1.1
-_28- Link requests generated by 'projectal.Entity.create()' and
+_27### 4.0.1
+_28- Minimum Projectal version is now 4.0.0.
+_29
+_30### 4.0.0
+_31
+_32Version 4.0.0 accompanies the release of Projectal 4.0.
+_33
+_34- Added the `Activity` entity, new in Projectal 4.0.
+_35
+_36- Added the `Booking` entity, new in Projectal 4.0.
+_37
+_38### 3.1.1
+_39- Link requests generated by 'projectal.Entity.create()' and
 'projectal.Entity.update()' are now
-_29  executed in batches. This is enabled by default with the
+_40  executed in batches. This is enabled by default with the
 'batch_linking=True' parameter and can
-_30  be disabled to execute each link request individually. It is recommended
+_41  be disabled to execute each link request individually. It is recommended
 to leave this parameter
-_31  enabled as this can greatly reduce the number of network requests.
-_32
-_33### 3.1.0
-_34- Minimum Projectal version is now 3.1.5.
-_35
-_36- Added `projectal.Webhook.list_events()`. See API doc for details on how to
+_42  enabled as this can greatly reduce the number of network requests.
+_43
+_44### 3.1.0
+_45- Minimum Projectal version is now 3.1.5.
+_46
+_47- Added `projectal.Webhook.list_events()`. See API doc for details on how to
 use.
-_37
-_38- Added `deleted_at` parameter to `projectal.Entity.get()`. This value
+_48
+_49- Added `deleted_at` parameter to `projectal.Entity.get()`. This value
 should be a UTC timestamp
-_39  from a webhook delete event.
-_40
-_41- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD
+_50  from a webhook delete event.
+_51
+_52- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD
 service configured in
-_42  the Projectal server settings.
-_43
-_44- Enhanced output of `projectal.Entity.changes()` function when reporting
+_53  the Projectal server settings.
+_54
+_55- Enhanced output of `projectal.Entity.changes()` function when reporting
 link changes.
-_45  It no longer dumps the entire before-and-after list with the full content
+_56  It no longer dumps the entire before-and-after list with the full content
 of each linked entity.
-_46  Now reports three lists: `added`, `updated`, `removed`. Entities within
+_57  Now reports three lists: `added`, `updated`, `removed`. Entities within
 the `updated` list
-_47  follow the same `old` vs `new` dictionary model for the data attributes
+_58  follow the same `old` vs `new` dictionary model for the data attributes
 within them. E.g:
-_48
-_49    ```
-_50    resourceList: [
-_51        'added': [],
-_52        'updated': [
-_53            {'uuId': '14eb4c31-0f92-49d1-8b4d-507ab939003e', 'resourceLink':
+_59
+_60    ```
+_61    resourceList: [
+_62        'added': [],
+_63        'updated': [
+_64            {'uuId': '14eb4c31-0f92-49d1-8b4d-507ab939003e', 'resourceLink':
 {'utilization': {'old': 0.1, 'new': 0.9}}},
-_54        ],
-_55        'removed': []
-_56    ]
-_57    ```
-_58  This should result in slimmer logs that are much easier to understand as
+_65        ],
+_66        'removed': []
+_67    ]
+_68    ```
+_69  This should result in slimmer logs that are much easier to understand as
 the changes are
-_59  clearly indicated.
-_60
-_61### 3.0.2
-_62- Added `projectal.Entity.get_link_definitions()`. Exposes entity link
+_70  clearly indicated.
+_71
+_72### 3.0.2
+_73- Added `projectal.Entity.get_link_definitions()`. Exposes entity link
 definition dictionary.
-_63  Consumers can inspect which links an Entity knows about and their internal
+_74  Consumers can inspect which links an Entity knows about and their internal
 settings.
-_64  Link definitions that appear here are the links valid for `links=[]`
+_75  Link definitions that appear here are the links valid for `links=[]`
 parameters.
-_65
-_66### 3.0.1
-_67- Fixed fetching project with links=['task'] not being available.
-_68
-_69- Improved Permission.list(). Now returns a dict with the permission name as
-_70  key with Permission objects as the value (instead of list of uuIds).
-_71
-_72- Added a way to use the aliasing feature of the API (new in Projectal 3.0).
-_73Set `projectal.api_alias = 'uuid'` to the UUID of a User object and all
-_74requests made will be done as that user. Restore this value to None to
-resume
-_75normal operation. (Some rules and limitations apply. See API for more
-details.)
 _76
-_77- Added complete support for the Tags entity (including linkers).
-_78
-_79### 3.0
-_80
-_81Version 3.0 accompanies the release of Projectal 3.0.
+_77### 3.0.1
+_78- Fixed fetching project with links=['task'] not being available.
+_79
+_80- Improved Permission.list(). Now returns a dict with the permission name as
+_81  key with Permission objects as the value (instead of list of uuIds).
 _82
-_83**Breaking changes**:
-_84
-_85- The `links` parameter on `Entity` functions now consumes a list of entity
-_86  names instead of a comma-separated string. For example:
+_83- Added a way to use the aliasing feature of the API (new in Projectal 3.0).
+_84Set `projectal.api_alias = 'uuid'` to the UUID of a User object and all
+_85requests made will be done as that user. Restore this value to None to
+resume
+_86normal operation. (Some rules and limitations apply. See API for more
+details.)
 _87
-_88    ```
-_89    # Before:
-_90    projectal.Staff.get('<uuid>', links='skill,location')  # No longer valid
-_91    # Now:
-_92    projectal.Staff.get('<uuid>', links=['skill', 'location'])
-_93    ```
-_94
-_95- The `projectal.enums.SkillLevel` enum has had all values renamed to match
+_88- Added complete support for the Tags entity (including linkers).
+_89
+_90### 3.0
+_91
+_92Version 3.0 accompanies the release of Projectal 3.0.
+_93
+_94**Breaking changes**:
+_95
+_96- The `links` parameter on `Entity` functions now consumes a list of entity
+_97  names instead of a comma-separated string. For example:
+_98
+_99    ```
+100    # Before:
+101    projectal.Staff.get('<uuid>', links='skill,location')  # No longer valid
+102    # Now:
+103    projectal.Staff.get('<uuid>', links=['skill', 'location'])
+104    ```
+105
+106- The `projectal.enums.SkillLevel` enum has had all values renamed to match
 the new values
-_96  used in Projectal (Junior, Mid, Senior). This includes the properties on
-_97  Skill entities indicating work time for auto-scheduling (now
+107  used in Projectal (Junior, Mid, Senior). This includes the properties on
+108  Skill entities indicating work time for auto-scheduling (now
 `juniorLevel`,
-_98  `midLevel`, `seniorLevel`).
-_99
-100**Other changes**:
-101
-102- Working with entity links has changed in this release. The previous
-methods
-103  are still available and continue to work as before, but there is no need
-104  to interact with the `projectal.linkers` methods yourself anymore.
-105
-106  You can now modify the list of links within an entity and save the entity
-107  directly. The library will automatically determine how the links have been
-108  modified and issue the correct linker methods on your behalf. E.g.,
-109  you can now do:
+109  `midLevel`, `seniorLevel`).
 110
-111    ```
-112    staff = projectal.Staff.get('<uuid>', links=['skill'])
-113    staff['firstName'] = "New name"  # Field update
-114    staff['skillList'] = [skill1, skill2, skill3]  # Link update
-115    staff.save()  # Both changes are saved
+111**Other changes**:
+112
+113- Working with entity links has changed in this release. The previous
+methods
+114  are still available and continue to work as before, but there is no need
+115  to interact with the `projectal.linkers` methods yourself anymore.
 116
-117    task = projectal.Task.get('<uuid>', links=['stage'])
-118    task['stage'] = stage1  # Uses a single object instead of list
-119    task.save()
-120    ```
+117  You can now modify the list of links within an entity and save the entity
+118  directly. The library will automatically determine how the links have been
+119  modified and issue the correct linker methods on your behalf. E.g.,
+120  you can now do:
 121
-122  See `examples/linking.py` for a more complete demonstration of linking
-123  capabilities and limitations.
-124
-125- Linkers (`projectal.linkers`) can now be given a list of Entities (of one
-126 type) to link/unlink/relink in bulk. E.g:
-127    ```
-128    staff.unlink_skill(skill1)  # Before
-129    staff.unlink_skill([skill1, skill2, skill3])  # This works now too
-130    ```
-131
-132- Linkers now strip the payload to only the required fields instead of
+122    ```
+123    staff = projectal.Staff.get('<uuid>', links=['skill'])
+124    staff['firstName'] = "New name"  # Field update
+125    staff['skillList'] = [skill1, skill2, skill3]  # Link update
+126    staff.save()  # Both changes are saved
+127
+128    task = projectal.Task.get('<uuid>', links=['stage'])
+129    task['stage'] = stage1  # Uses a single object instead of list
+130    task.save()
+131    ```
+132
+133  See `examples/linking.py` for a more complete demonstration of linking
+134  capabilities and limitations.
+135
+136- Linkers (`projectal.linkers`) can now be given a list of Entities (of one
+137 type) to link/unlink/relink in bulk. E.g:
+138    ```
+139    staff.unlink_skill(skill1)  # Before
+140    staff.unlink_skill([skill1, skill2, skill3])  # This works now too
+141    ```
+142
+143- Linkers now strip the payload to only the required fields instead of
 passing
-133  on the entire Entity object. This cuts down on network traffic
+144  on the entire Entity object. This cuts down on network traffic
 significantly.
-134
-135- Linkers now also work in reverse. The Projectal server currently only
+145
+146- Linkers now also work in reverse. The Projectal server currently only
 supports
-136  linking entities in one direction (e.g., Company to Staff), which often
+147  linking entities in one direction (e.g., Company to Staff), which often
 means
-137  writing something like:
-138    ```
-139    staff.link_location(location)
-140    company.link_staff(staff)
-141    ```
-142  The change in direction is not very intuitive and would require you to
+148  writing something like:
+149    ```
+150    staff.link_location(location)
+151    company.link_staff(staff)
+152    ```
+153  The change in direction is not very intuitive and would require you to
 constantly
-143  verify which direction is the one available to you in the documentation.
-144
-145  Reverse linkers hide this from you and figure out the direction of the
+154  verify which direction is the one available to you in the documentation.
+155
+156  Reverse linkers hide this from you and figure out the direction of the
 relationship
-146  for you behind the scenes. So now this is possible, even though the API
+157  for you behind the scenes. So now this is possible, even though the API
 doesn't
-147  strictly support it:
-148    ```
-149    staff.link_location(location)
-150    staff.link_company(company)
-151    ```
-152    Caveat: the documentation for Staff will not list Company links. You
+158  strictly support it:
+159    ```
+160    staff.link_location(location)
+161    staff.link_company(company)
+162    ```
+163    Caveat: the documentation for Staff will not list Company links. You
 will still
-153    have to look up the Company documentation for the link description.
-154
-155- Requesting entity links with the `links=` parameter will now always ensure
+164    have to look up the Company documentation for the link description.
+165
+166- Requesting entity links with the `links=` parameter will now always ensure
 the
-156  link field (e.g., `taskList`) exists in the result, even if there are no
+167  link field (e.g., `taskList`) exists in the result, even if there are no
 links.
-157  The server may not always return a value, but we can use a default value (
+168  The server may not always return a value, but we can use a default value (
 [] for
-158  lists, None for dicts).
-159
-160- Added a `Permission` entity to correctly type Permissions in responses.
-161
-162- Added a `Tag` entity, new in Projectal 3.0.
-163
-164- Added `links` parameter to `Company.get_primary_company()`
-165
-166- `Department.tree()`: now consumes a `holder` Entity object instead
-167  of a uuId.
-168
-169- `Department.tree()`: added `generic_staff` parameter, new in
-170  Projectal 3.0.
-171
-172- Don't break on trailing slash in Projectal URL
-173
-174- When creating tasks, populate the `projectRef` and `parent` fields in the
-175  returned Task object.
+169  lists, None for dicts).
+170
+171- Added a `Permission` entity to correctly type Permissions in responses.
+172
+173- Added a `Tag` entity, new in Projectal 3.0.
+174
+175- Added `links` parameter to `Company.get_primary_company()`
 176
-177- Added convenience functions for matching on fields where you only want
-178  one result (e.g match_one()) which return the first match found.
+177- `Department.tree()`: now consumes a `holder` Entity object instead
+178  of a uuId.
 179
-180- Update the entity `history()` method for Projectal 3.0. Some new
+180- `Department.tree()`: added `generic_staff` parameter, new in
+181  Projectal 3.0.
+182
+183- Don't break on trailing slash in Projectal URL
+184
+185- When creating tasks, populate the `projectRef` and `parent` fields in the
+186  returned Task object.
+187
+188- Added convenience functions for matching on fields where you only want
+189  one result (e.g match_one()) which return the first match found.
+190
+191- Update the entity `history()` method for Projectal 3.0. Some new
 parameters
-181  allow you to restrict the history to a particular range or to get only the
-182  changes for a webhook timestamp.
-183
-184- Entity objects can call `.history()` on themselves.
-185
-186- The library now keeps a reference to the User account that is currently
-logged
-187  in and using the API: `projectal.api_auth_details`.
-188
-189**Known issues**:
-190- You cannot save changes to Notes or Calendars via their holding entity.
-You
-191  must save the changes on the Note or Calendar directly. To illustrate:
-192  ```
-193  staff = projectal.Staff.get(<uuid>, links=['calendar'])
-194  calendar = staff['calendarList'][0]
-195  calendar['name'] = 'Calendar 2'
+192  allow you to restrict the history to a particular range or to get only the
+193  changes for a webhook timestamp.
+194
+195- Entity objects can call `.history()` on themselves.
 196
-197  # Cannot do this - will not pick up the changes
-198  staff.save()
+197- The library now keeps a reference to the User account that is currently
+logged
+198  in and using the API: `projectal.api_auth_details`.
 199
-200  # You must do this for now
-201  calendar.save()
-202  ```
-203  This will be resolved in a future release.
-204
-205- When creating Notes, the `created` and `modified` values may differ by
-206  1ms in the object you have a reference to compared to what is actually
-207  stored in the database.
-208
-209- Duration calculation is not precise yet (mentioned in 2.1.0)
+200**Known issues**:
+201- You cannot save changes to Notes or Calendars via their holding entity.
+You
+202  must save the changes on the Note or Calendar directly. To illustrate:
+203  ```
+204  staff = projectal.Staff.get(<uuid>, links=['calendar'])
+205  calendar = staff['calendarList'][0]
+206  calendar['name'] = 'Calendar 2'
+207
+208  # Cannot do this - will not pick up the changes
+209  staff.save()
 210
-211### 2.1.0
-212**Breaking changes**:
-213- Getting location calendar is now done on an instance instead of class. So
-214  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`
-215- The `CompanyType.Master` enum has been replaced with
+211  # You must do this for now
+212  calendar.save()
+213  ```
+214  This will be resolved in a future release.
+215
+216- When creating Notes, the `created` and `modified` values may differ by
+217  1ms in the object you have a reference to compared to what is actually
+218  stored in the database.
+219
+220- Duration calculation is not precise yet (mentioned in 2.1.0)
+221
+222### 2.1.0
+223**Breaking changes**:
+224- Getting location calendar is now done on an instance instead of class. So
+225  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`
+226- The `CompanyType.Master` enum has been replaced with
 `CompanyType.Primary`.
-216  This was a leftover reference to the Master Company which was renamed in
-217  Projectal several versions ago.
-218
-219**Other changes**:
-220- Date conversion functions return None when given None or empty string
-221- Added `Task.reset_duration()` as a basic duration calculator for tasks.
-222  This is a work-in-progress and will be gradually improved. The duration
-223  calculator takes into consideration the location to remove non-work
-224  days from the estimate of working duration. It currently does not work
-225  for the time component or `isWorking=True` exceptions.
-226- Change detection in `Entity.changes()` now excludes cases where the
-227  server has no value and the new value is None. Saving this change has
-228  no effect and would always detect a change until a non-None value is
-229  set, which is noisy and generates more network activity.
-230
-231### 2.0.3
-232- Better support for calendars.
-233  - Distinguish between calendar containers ("Calendar") and the
-234    calendar items within them ("CalendarItem").
-235  - Allow CalendarItems to be saved directly. E.G item.save()
-236- Fix 'holder' parameter in contact/staff/location/task_template not
-237  permitting object type. Now consumes uuId or object to match rest of
-238  the library.
-239- `Entity.changes()` has been extended with an `old=True` flag. When
-240  this flag is true, the set of changes will now return both the original
-241  and the new values. E.g.
-242```
-243task.changes()
-244# {'name': 'current'}
-245task.changes(old=True)
-246# {'name': {'old': 'original', 'new': 'current'}}
-247```
-248- Fixed entity link cache causing errors when deleting a link from an entity
-249  which has not been fetched with links (deleting from empty list).
-250
-251### 2.0.2
-252- Fixed updating Webhook entities
-253
-254### 2.0.1
-255- Fixed application ID not being used correctly.
-256
-257### 2.0.0
-258- Version 2.0 accompanies the release of Projectal 2.0. There are no major
+227  This was a leftover reference to the Master Company which was renamed in
+228  Projectal several versions ago.
+229
+230**Other changes**:
+231- Date conversion functions return None when given None or empty string
+232- Added `Task.reset_duration()` as a basic duration calculator for tasks.
+233  This is a work-in-progress and will be gradually improved. The duration
+234  calculator takes into consideration the location to remove non-work
+235  days from the estimate of working duration. It currently does not work
+236  for the time component or `isWorking=True` exceptions.
+237- Change detection in `Entity.changes()` now excludes cases where the
+238  server has no value and the new value is None. Saving this change has
+239  no effect and would always detect a change until a non-None value is
+240  set, which is noisy and generates more network activity.
+241
+242### 2.0.3
+243- Better support for calendars.
+244  - Distinguish between calendar containers ("Calendar") and the
+245    calendar items within them ("CalendarItem").
+246  - Allow CalendarItems to be saved directly. E.G item.save()
+247- Fix 'holder' parameter in contact/staff/location/task_template not
+248  permitting object type. Now consumes uuId or object to match rest of
+249  the library.
+250- `Entity.changes()` has been extended with an `old=True` flag. When
+251  this flag is true, the set of changes will now return both the original
+252  and the new values. E.g.
+253```
+254task.changes()
+255# {'name': 'current'}
+256task.changes(old=True)
+257# {'name': {'old': 'original', 'new': 'current'}}
+258```
+259- Fixed entity link cache causing errors when deleting a link from an entity
+260  which has not been fetched with links (deleting from empty list).
+261
+262### 2.0.2
+263- Fixed updating Webhook entities
+264
+265### 2.0.1
+266- Fixed application ID not being used correctly.
+267
+268### 2.0.0
+269- Version 2.0 accompanies the release of Projectal 2.0. There are no major
 changes
-259  since the previous release.
-260- Expose `Entity.changes()` function. It returns a list of fields on an
+270  since the previous release.
+271- Expose `Entity.changes()` function. It returns a list of fields on an
 entity that
-261  have changed since fetching it. These are the changes that will be sent
+272  have changed since fetching it. These are the changes that will be sent
 over to the
-262  server when an update request is made.
-263- Added missing 'packaging' dependency to requirements.
-264
-265### 1.2.0
-266
-267**Breaking changes**:
-268
-269- Renamed `request_timestamp` to `response_timestamp` to better reflect its
+273  server when an update request is made.
+274- Added missing 'packaging' dependency to requirements.
+275
+276### 1.2.0
+277
+278**Breaking changes**:
+279
+280- Renamed `request_timestamp` to `response_timestamp` to better reflect its
 purpose.
-270- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been
+281- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been
 reverted.
-271  All date fields returned from the server remain as UTC timestamps.
-272
-273  The reason is that date fields on tasks contain a time component and
+282  All date fields returned from the server remain as UTC timestamps.
+283
+284  The reason is that date fields on tasks contain a time component and
 converting them
-274  into date strings was erasing the time, resulting in a value that does not
+285  into date strings was erasing the time, resulting in a value that does not
 match
-275  the database.
-276
-277  Note: the server supports setting date fields using a date string like
+286  the database.
+287
+288  Note: the server supports setting date fields using a date string like
 `2022-04-05`.
-278  You may use this if you prefer but the server will always return a
+289  You may use this if you prefer but the server will always return a
 timestamp.
-279
-280  Note: we provide utility functions for easily converting dates from/to
-281  timestamps expected by the Projectal server. See:
-282  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and
-283  `projectal.timestamp_from_datetime()`.
-284
-285**Other changes**:
-286- Implement request chunking - for methods that consume a list of entities,
+290
+291  Note: we provide utility functions for easily converting dates from/to
+292  timestamps expected by the Projectal server. See:
+293  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and
+294  `projectal.timestamp_from_datetime()`.
+295
+296**Other changes**:
+297- Implement request chunking - for methods that consume a list of entities,
 we now
-287  automatically batch them up into multiple requests to prevent timeouts on
+298  automatically batch them up into multiple requests to prevent timeouts on
 really
-288  large request. Values are configurable through
-289  `projectal.chunk_size_read` and `projectal.chunk_size_write`.
-290  Default values: Read: 1000 items. Write: 200 items.
-291- Added profile get/set functions on entities for easier use. Now you only
+299  large request. Values are configurable through
+300  `projectal.chunk_size_read` and `projectal.chunk_size_write`.
+301  Default values: Read: 1000 items. Write: 200 items.
+302- Added profile get/set functions on entities for easier use. Now you only
 need to supply
-292  the key and the data. E.g:
-293
-294```
-295key = 'hr_connector'
-296data = {'staff_source': 'company_z'}
-297task.profile_set(key, data)
-298```
-299
-300- Entity link methods now automatically update the entity's cached list of
+303  the key and the data. E.g:
+304
+305```
+306key = 'hr_connector'
+307data = {'staff_source': 'company_z'}
+308task.profile_set(key, data)
+309```
+310
+311- Entity link methods now automatically update the entity's cached list of
 links. E.g:
-301  a task fetched with staff links will have `task['staffList'] =
+312  a task fetched with staff links will have `task['staffList'] =
 [Staff1,Staff2]`.
-302  Before, doing a `task.link_staff(staff)` did not modify the list to
+313  Before, doing a `task.link_staff(staff)` did not modify the list to
 reflect the
-303  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same
+314  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same
 applies for update
-304  and delete.
-305
-306  This allows you to modify links and continue working with that object
+315  and delete.
+316
+317  This allows you to modify links and continue working with that object
 without having
-307  to fetch it again to obtain the most recent link data. Be aware that if
+318  to fetch it again to obtain the most recent link data. Be aware that if
 you acquire
-308  the object without requesting the link data as well
-309  (e.g: `projectal.Task.get(id, links='STAFF')`),
-310  these lists will not accurately reflect what's in the database, only the
+319  the object without requesting the link data as well
+320  (e.g: `projectal.Task.get(id, links='STAFF')`),
+321  these lists will not accurately reflect what's in the database, only the
 changes made
-311  while the object is held.
-312
-313- Support new `applicationId` property on login. Set with:
+322  while the object is held.
+323
+324- Support new `applicationId` property on login. Set with:
 `projectal.api_application_id`.
-314  The application ID is sent back to you in webhooks so you know which
+325  The application ID is sent back to you in webhooks so you know which
 application was
-315  the source of the event (and you can choose to filter them accordingly).
-316- Added `Entity.set_readonly()` to allow setting values on entities that
+326  the source of the event (and you can choose to filter them accordingly).
+327- Added `Entity.set_readonly()` to allow setting values on entities that
 will not
-317  be sent over to the server when updating/saving the entity.
-318
-319  The main use case for this is to populate cached entities which you have
+328  be sent over to the server when updating/saving the entity.
+329
+330  The main use case for this is to populate cached entities which you have
 just created
-320  with values you already know about. This is mainly a workaround for the
+331  with values you already know about. This is mainly a workaround for the
 limitation of
-321  the server not sending the full object back after creating it, resulting
+332  the server not sending the full object back after creating it, resulting
 in the client
-322  needing to fetch the object in full again if it needs some of the fields
+333  needing to fetch the object in full again if it needs some of the fields
 set by the
-323  server after creation.
-324
-325  Additionally, some read-only fields will generate an error on the server
+334  server after creation.
+335
+336  Additionally, some read-only fields will generate an error on the server
 if
-326  included in the update request. This method lets you set these values on
+337  included in the update request. This method lets you set these values on
 newly
-327  created objects without triggering this error.
-328
-329  A common example is setting the `projectRef` of a task you just created.
-330
-331
-332### 1.1.1
-333- Add support for 'profiles' API. Profiles are a type of key-value storage
+338  created objects without triggering this error.
+339
+340  A common example is setting the `projectRef` of a task you just created.
+341
+342
+343### 1.1.1
+344- Add support for 'profiles' API. Profiles are a type of key-value storage
 that target
-334  any entity. Not currently documented.
-335- Fix handling error message parsing in ProjectalException for batch create
+345  any entity. Not currently documented.
+346- Fix handling error message parsing in ProjectalException for batch create
 operation
-336- Add `Task.update_order()` to set task order
-337- Return empty list when GETing empty list instead of failing (no request to
+347- Add `Task.update_order()` to set task order
+348- Return empty list when GETing empty list instead of failing (no request to
 server)
-338- Expose the timestamp returned by requests that modify the database. Use
-339  `projectal.request_timestamp` to get the value of the most recent request
+349- Expose the timestamp returned by requests that modify the database. Use
+350  `projectal.request_timestamp` to get the value of the most recent request
 (None
-340  if no timestamp in response)
-341
-342### 1.1.0
-343- Minimum Projectal version is now 1.9.4.
-344
-345**Breaking changes**:
-346- Entity `list()` now returns a list of UUIDs instead of full objects. You
+351  if no timestamp in response)
+352
+353### 1.1.0
+354- Minimum Projectal version is now 1.9.4.
+355
+356**Breaking changes**:
+357- Entity `list()` now returns a list of UUIDs instead of full objects. You
 may provide
-347  an `expand` parameter to restore the previous behavior: `Entity.list
+358  an `expand` parameter to restore the previous behavior: `Entity.list
 (expand=True)`.
-348  This change is made for performance reasons where you may have thousands
+359  This change is made for performance reasons where you may have thousands
 of tasks
-349  and getting them all may time out. For those cases, we suggest writing a
+360  and getting them all may time out. For those cases, we suggest writing a
 query to filter
-350  down to only the tasks and fields you need.
-351- `Company.get_master_company()` has been renamed to
+361  down to only the tasks and fields you need.
+362- `Company.get_master_company()` has been renamed to
 `Company.get_primary_company()`
-352  to match the server.
-353- The following date fields are converted into date strings upon fetch:
-354  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.
-355  These fields are added or updated using date strings (like `2022-03-02`),
+363  to match the server.
+364- The following date fields are converted into date strings upon fetch:
+365  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.
+366  These fields are added or updated using date strings (like `2022-03-02`),
 but the
-356  server returns timestamps (e.g: 1646006400000) upon fetch, which is
+367  server returns timestamps (e.g: 1646006400000) upon fetch, which is
 confusing. This
-357  change ensures they are always date strings for consistency.
-358
-359**Other changes**:
-360- When updating an entity, only the fields that have changed are sent to the
+368  change ensures they are always date strings for consistency.
+369
+370**Other changes**:
+371- When updating an entity, only the fields that have changed are sent to the
 server. When
-361  updating a list of entities, unmodified entities are not sent to the
+372  updating a list of entities, unmodified entities are not sent to the
 server at all. This
-362  dramatically reduces the payload size and should speed things up.
-363- When fetching entities, entity links are now typed as well. E.g. `project
+373  dramatically reduces the payload size and should speed things up.
+374- When fetching entities, entity links are now typed as well. E.g. `project
 ['rebateList']`
-364  contains a list of `Rebate` instead of `dict`.
-365- Added `date_from_timestamp()` and `timestamp_from_date()` functions to
+375  contains a list of `Rebate` instead of `dict`.
+376- Added `date_from_timestamp()` and `timestamp_from_date()` functions to
 help with
-366  converting to/from dates and Projectal timestamps.
-367- Entity history now uses `desc` by default (index 0 is newest)
-368- Added `Project.tasks()` to list all task UUIDs within a project.
-369
-370### 1.0.3
-371- Fix another case of automatic JWT refresh not working
-372
-373### 1.0.2
-374- Entity instances can `save()` or `delete()` on themselves
-375- Fix broken `dict` methods (`get()` and `update()`) when called from Entity
-instances
-376- Fix automatic JWT refresh only working in some cases
-377
-378### 1.0.1
-379- Added `list()` function for all entities
-380- Added search functions for all entities (match-, search, query)
-381- Added `Company.get_master_company()`
-382- Fixed adding template tasks
+377  converting to/from dates and Projectal timestamps.
+378- Entity history now uses `desc` by default (index 0 is newest)
+379- Added `Project.tasks()` to list all task UUIDs within a project.
+380
+381### 1.0.3
+382- Fix another case of automatic JWT refresh not working
 383
-384"""
-385import logging
-386import os
-387
-388from projectal.entities import *
-389from .api import *
-390from . import profile
-391
-392api_base = os.getenv('PROJECTAL_URL')
-393api_username = os.getenv('PROJECTAL_USERNAME')
-394api_password = os.getenv('PROJECTAL_PASSWORD')
-395api_application_id = None
-396api_auth_details = None
-397api_alias = None
-398cookies = None
-399chunk_size_read = 1000
-400chunk_size_write = 200
-401
-402# Records the timestamp generated by the last request (database
-403# event time). These are reported on add or updates; if there is
-404# no timestamp in the response, this is set to None.
-405response_timestamp = None
-406
-407
-408# The minimum version number of the Projectal instance that this
-409# API client targets. Lower versions are not supported and will
-410# raise an exception.
-411MIN_PROJECTAL_VERSION = "3.1.5"
+384### 1.0.2
+385- Entity instances can `save()` or `delete()` on themselves
+386- Fix broken `dict` methods (`get()` and `update()`) when called from Entity
+instances
+387- Fix automatic JWT refresh only working in some cases
+388
+389### 1.0.1
+390- Added `list()` function for all entities
+391- Added search functions for all entities (match-, search, query)
+392- Added `Company.get_master_company()`
+393- Fixed adding template tasks
+394
+395"""
+396import logging
+397import os
+398
+399from projectal.entities import *
+400from .api import *
+401from . import profile
+402
+403api_base = os.getenv('PROJECTAL_URL')
+404api_username = os.getenv('PROJECTAL_USERNAME')
+405api_password = os.getenv('PROJECTAL_PASSWORD')
+406api_application_id = None
+407api_auth_details = None
+408api_alias = None
+409cookies = None
+410chunk_size_read = 1000
+411chunk_size_write = 200
 412
-413__verify = True
-414
-415logging.getLogger('projectal-api-client').addHandler(logging.NullHandler())
+413# Records the timestamp generated by the last request (database
+414# event time). These are reported on add or updates; if there is
+415# no timestamp in the response, this is set to None.
+416response_timestamp = None
+417
+418
+419# The minimum version number of the Projectal instance that this
+420# API client targets. Lower versions are not supported and will
+421# raise an exception.
+422MIN_PROJECTAL_VERSION = "4.0.0"
+423
+424__verify = True
+425
+426logging.getLogger('projectal-api-client').addHandler(logging.NullHandler())
```

### Comparing `projectal-3.1.1/examples/linking.py` & `projectal-4.0.1/examples/linking.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/examples/task.py` & `projectal-4.0.1/examples/task.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/examples/webhook.py` & `projectal-4.0.1/examples/webhook.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/__init__.py` & `projectal-4.0.1/projectal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,25 @@
 details = projectal.auth_details()
 ```
 
 ----
 
 ## Changelog
 
+### 4.0.1
+- Minimum Projectal version is now 4.0.0.
+
+### 4.0.0
+
+Version 4.0.0 accompanies the release of Projectal 4.0.
+
+- Added the `Activity` entity, new in Projectal 4.0.
+
+- Added the `Booking` entity, new in Projectal 4.0.
+
 ### 3.1.1
 - Link requests generated by 'projectal.Entity.create()' and 'projectal.Entity.update()' are now
   executed in batches. This is enabled by default with the 'batch_linking=True' parameter and can
   be disabled to execute each link request individually. It is recommended to leave this parameter
   enabled as this can greatly reduce the number of network requests.
 
 ### 3.1.0
@@ -404,12 +415,12 @@
 # no timestamp in the response, this is set to None.
 response_timestamp = None
 
 
 # The minimum version number of the Projectal instance that this
 # API client targets. Lower versions are not supported and will
 # raise an exception.
-MIN_PROJECTAL_VERSION = "3.1.5"
+MIN_PROJECTAL_VERSION = "4.0.0"
 
 __verify = True
 
 logging.getLogger('projectal-api-client').addHandler(logging.NullHandler())
```

### Comparing `projectal-3.1.1/projectal/api.py` & `projectal-4.0.1/projectal/api.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/__init__.py` & `projectal-4.0.1/projectal/entities/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Implementations of all Projectal entities.
 
 All classes here inherit from `projectal.entity.Entity`.
 """
 
 from projectal.entities.access_policy import AccessPolicy
+from projectal.entities.activity import Activity
+from projectal.entities.booking import Booking
 from projectal.entities.calendar import Calendar
 from projectal.entities.company import Company
 from projectal.entities.contact import Contact
 from projectal.entities.customer import Customer
 from projectal.entities.department import Department
 from projectal.entities.file import File
 from projectal.entities.folder import Folder
```

### Comparing `projectal-3.1.1/projectal/entities/calendar.py` & `projectal-4.0.1/projectal/entities/calendar.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/company.py` & `projectal-4.0.1/projectal/entities/company.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/contact.py` & `projectal-4.0.1/projectal/entities/contact.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/department.py` & `projectal-4.0.1/projectal/entities/department.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/file.py` & `projectal-4.0.1/projectal/entities/file.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/folder.py` & `projectal-4.0.1/projectal/entities/folder.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/location.py` & `projectal-4.0.1/projectal/entities/location.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/note.py` & `projectal-4.0.1/projectal/entities/note.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/permission.py` & `projectal-4.0.1/projectal/entities/permission.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/project.py` & `projectal-4.0.1/projectal/entities/project.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/project_template.py` & `projectal-4.0.1/projectal/entities/project_template.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/staff.py` & `projectal-4.0.1/projectal/entities/staff.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/task.py` & `projectal-4.0.1/projectal/entities/task.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/task_template.py` & `projectal-4.0.1/projectal/entities/task_template.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/user.py` & `projectal-4.0.1/projectal/entities/user.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/webhook.py` & `projectal-4.0.1/projectal/entities/webhook.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entity.py` & `projectal-4.0.1/projectal/entity.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/enums.py` & `projectal-4.0.1/projectal/enums.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/errors.py` & `projectal-4.0.1/projectal/errors.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/linkers.py` & `projectal-4.0.1/projectal/linkers.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/profile.py` & `projectal-4.0.1/projectal/profile.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal.egg-info/PKG-INFO` & `projectal-4.0.1/projectal.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectal
-Version: 3.1.1
+Version: 4.0.1
 Summary: Python bindings for the Projectal API
 Home-page: https://projectal.com/resources/developer
 Author: Projectal
 Author-email: support@projectal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `projectal-3.1.1/projectal.egg-info/SOURCES.txt` & `projectal-4.0.1/projectal.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 docs/projectal/entities.html
 docs/projectal/entity.html
 docs/projectal/enums.html
 docs/projectal/errors.html
 docs/projectal/linkers.html
 docs/projectal/profile.html
 docs/projectal/entities/access_policy.html
+docs/projectal/entities/activity.html
+docs/projectal/entities/booking.html
 docs/projectal/entities/calendar.html
 docs/projectal/entities/company.html
 docs/projectal/entities/contact.html
 docs/projectal/entities/customer.html
 docs/projectal/entities/department.html
 docs/projectal/entities/file.html
 docs/projectal/entities/folder.html
@@ -46,14 +48,16 @@
 projectal.egg-info/PKG-INFO
 projectal.egg-info/SOURCES.txt
 projectal.egg-info/dependency_links.txt
 projectal.egg-info/requires.txt
 projectal.egg-info/top_level.txt
 projectal/entities/__init__.py
 projectal/entities/access_policy.py
+projectal/entities/activity.py
+projectal/entities/booking.py
 projectal/entities/calendar.py
 projectal/entities/company.py
 projectal/entities/contact.py
 projectal/entities/customer.py
 projectal/entities/department.py
 projectal/entities/file.py
 projectal/entities/folder.py
```

### Comparing `projectal-3.1.1/setup.py` & `projectal-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='projectal',
-    version='3.1.1',
+    version='4.0.1',
     description='Python bindings for the Projectal API',
     long_description="The Python library allows developers to write Python-based apps that talk directly with Projectal. This gives developers immense freedom to access all data points in Projectal and to integrate Projectal with their workflow.",
     long_description_content_type="text/plain",
     url='https://projectal.com/resources/developer',
     author='Projectal',
     author_email='support@projectal.com',
     license='MIT',
```

