# Comparing `tmp/projectal-3.1.1.tar.gz` & `tmp/projectal-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectal-3.1.1.tar", last modified: Thu Mar  9 05:04:00 2023, max compression
+gzip compressed data, was "projectal-4.0.0.tar", last modified: Wed Jun 14 05:42:55 2023, max compression
```

## Comparing `projectal-3.1.1.tar` & `projectal-4.0.0.tar`

### file list

```diff
@@ -1,84 +1,86 @@
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
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 05:42:55.449802 projectal-4.0.0/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1074 2022-11-17 04:31:31.000000 projectal-4.0.0/LICENSE
+-rw-rw-r--   0 luked     (1003) luked     (1003)       30 2022-11-17 04:31:31.000000 projectal-4.0.0/MANIFEST.in
+-rw-rw-r--   0 luked     (1003) luked     (1003)      573 2023-06-14 05:42:55.449802 projectal-4.0.0/PKG-INFO
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 05:42:55.445803 projectal-4.0.0/docs/
+-rw-rw-r--   0 luked     (1003) luked     (1003)      140 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/index.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 05:42:55.445803 projectal-4.0.0/docs/projectal/
+-rw-rw-r--   0 luked     (1003) luked     (1003)   123963 2023-03-09 05:02:58.000000 projectal-4.0.0/docs/projectal/api.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 05:42:55.449802 projectal-4.0.0/docs/projectal/entities/
+-rw-rw-r--   0 luked     (1003) luked     (1003)    44886 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/access_policy.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    76700 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/calendar.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    78998 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/company.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    60445 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/contact.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    47063 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/customer.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    72006 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/department.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   112784 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/file.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    79391 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/folder.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    67125 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/location.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    73862 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/note.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    51453 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/permission.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    76122 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/project.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    53421 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/project_template.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    46200 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/rebate.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    46469 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/resource.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    45789 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/skill.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   138305 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/staff.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    44760 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/stage.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    42248 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/tag.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   167963 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/task.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    81669 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/task_template.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    82639 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/user.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    76578 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities/webhook.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    42087 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entities.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   660878 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/entity.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    81307 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/enums.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   107022 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/errors.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   260261 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/linkers.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    57589 2023-03-09 05:02:59.000000 projectal-4.0.0/docs/projectal/profile.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   111803 2023-03-09 05:02:58.000000 projectal-4.0.0/docs/projectal.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 05:42:55.449802 projectal-4.0.0/examples/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3154 2022-11-17 04:31:31.000000 projectal-4.0.0/examples/linking.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      811 2022-11-17 04:31:31.000000 projectal-4.0.0/examples/task.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1064 2022-12-01 02:53:21.000000 projectal-4.0.0/examples/webhook.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 05:42:55.449802 projectal-4.0.0/projectal/
+-rw-rw-r--   0 luked     (1003) luked     (1003)    17119 2023-06-14 04:33:19.000000 projectal-4.0.0/projectal/__init__.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     9133 2023-03-09 04:46:05.000000 projectal-4.0.0/projectal/api.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 05:42:55.449802 projectal-4.0.0/projectal/entities/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1298 2023-05-16 05:22:36.000000 projectal-4.0.0/projectal/entities/__init__.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      395 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/access_policy.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      485 2023-05-16 05:57:07.000000 projectal-4.0.0/projectal/entities/activity.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      303 2023-05-16 05:57:12.000000 projectal-4.0.0/projectal/entities/booking.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2233 2022-12-21 23:38:50.000000 projectal-4.0.0/projectal/entities/calendar.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1935 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/company.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      982 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/contact.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      460 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/customer.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1855 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/department.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3171 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/file.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1732 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/folder.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1305 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/location.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1939 2022-12-21 23:38:50.000000 projectal-4.0.0/projectal/entities/note.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      613 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/permission.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1655 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/project.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      709 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/project_template.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      426 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/rebate.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      434 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/resource.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      395 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/skill.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     4678 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/staff.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      344 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/stage.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      230 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/tag.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     6359 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/task.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1833 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/task_template.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1978 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/entities/user.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1668 2022-12-21 23:38:50.000000 projectal-4.0.0/projectal/entities/webhook.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)    40482 2023-03-09 04:46:05.000000 projectal-4.0.0/projectal/entity.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2152 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/enums.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3564 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/errors.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     8657 2022-12-21 23:38:50.000000 projectal-4.0.0/projectal/linkers.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2382 2022-11-17 04:31:31.000000 projectal-4.0.0/projectal/profile.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 05:42:55.449802 projectal-4.0.0/projectal.egg-info/
+-rw-rw-r--   0 luked     (1003) luked     (1003)      573 2023-06-14 05:42:55.000000 projectal-4.0.0/projectal.egg-info/PKG-INFO
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2261 2023-06-14 05:42:55.000000 projectal-4.0.0/projectal.egg-info/SOURCES.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)        1 2023-06-14 05:42:55.000000 projectal-4.0.0/projectal.egg-info/dependency_links.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       19 2023-06-14 05:42:55.000000 projectal-4.0.0/projectal.egg-info/requires.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       19 2023-06-14 05:42:55.000000 projectal-4.0.0/projectal.egg-info/top_level.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       38 2023-06-14 05:42:55.449802 projectal-4.0.0/setup.cfg
+-rw-rw-r--   0 luked     (1003) luked     (1003)      757 2023-06-14 05:16:16.000000 projectal-4.0.0/setup.py
```

### Comparing `projectal-3.1.1/LICENSE` & `projectal-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/PKG-INFO` & `projectal-4.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectal
-Version: 3.1.1
+Version: 4.0.0
 Summary: Python bindings for the Projectal API
 Home-page: https://projectal.com/resources/developer
 Author: Projectal
 Author-email: support@projectal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `projectal-3.1.1/docs/projectal/api.html` & `projectal-4.0.0/docs/projectal/api.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/access_policy.html` & `projectal-4.0.0/docs/projectal/entities/access_policy.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/calendar.html` & `projectal-4.0.0/docs/projectal/entities/calendar.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/company.html` & `projectal-4.0.0/docs/projectal/entities/company.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/contact.html` & `projectal-4.0.0/docs/projectal/entities/contact.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/customer.html` & `projectal-4.0.0/docs/projectal/entities/customer.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/department.html` & `projectal-4.0.0/docs/projectal/entities/department.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/file.html` & `projectal-4.0.0/docs/projectal/entities/file.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/folder.html` & `projectal-4.0.0/docs/projectal/entities/folder.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/location.html` & `projectal-4.0.0/docs/projectal/entities/location.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/note.html` & `projectal-4.0.0/docs/projectal/entities/note.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/permission.html` & `projectal-4.0.0/docs/projectal/entities/permission.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/project.html` & `projectal-4.0.0/docs/projectal/entities/project.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/project_template.html` & `projectal-4.0.0/docs/projectal/entities/project_template.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/rebate.html` & `projectal-4.0.0/docs/projectal/entities/rebate.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/resource.html` & `projectal-4.0.0/docs/projectal/entities/resource.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/skill.html` & `projectal-4.0.0/docs/projectal/entities/skill.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/staff.html` & `projectal-4.0.0/docs/projectal/entities/staff.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/stage.html` & `projectal-4.0.0/docs/projectal/entities/stage.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/tag.html` & `projectal-4.0.0/docs/projectal/entities/tag.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/task.html` & `projectal-4.0.0/docs/projectal/entities/task.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/task_template.html` & `projectal-4.0.0/docs/projectal/entities/task_template.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/user.html` & `projectal-4.0.0/docs/projectal/entities/user.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities/webhook.html` & `projectal-4.0.0/docs/projectal/entities/webhook.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entities.html` & `projectal-4.0.0/docs/projectal/entities.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/entity.html` & `projectal-4.0.0/docs/projectal/entity.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/enums.html` & `projectal-4.0.0/docs/projectal/enums.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/errors.html` & `projectal-4.0.0/docs/projectal/errors.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/linkers.html` & `projectal-4.0.0/docs/projectal/linkers.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal/profile.html` & `projectal-4.0.0/docs/projectal/profile.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/docs/projectal.html` & `projectal-4.0.0/docs/projectal.html`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/examples/linking.py` & `projectal-4.0.0/examples/linking.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/examples/task.py` & `projectal-4.0.0/examples/task.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/examples/webhook.py` & `projectal-4.0.0/examples/webhook.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/__init__.py` & `projectal-4.0.0/projectal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,22 @@
 details = projectal.auth_details()
 ```
 
 ----
 
 ## Changelog
 
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
@@ -404,12 +412,12 @@
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

### Comparing `projectal-3.1.1/projectal/api.py` & `projectal-4.0.0/projectal/api.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/__init__.py` & `projectal-4.0.0/projectal/entities/__init__.py`

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

### Comparing `projectal-3.1.1/projectal/entities/calendar.py` & `projectal-4.0.0/projectal/entities/calendar.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/company.py` & `projectal-4.0.0/projectal/entities/company.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/contact.py` & `projectal-4.0.0/projectal/entities/contact.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/department.py` & `projectal-4.0.0/projectal/entities/department.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/file.py` & `projectal-4.0.0/projectal/entities/file.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/folder.py` & `projectal-4.0.0/projectal/entities/folder.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/location.py` & `projectal-4.0.0/projectal/entities/location.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/note.py` & `projectal-4.0.0/projectal/entities/note.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/permission.py` & `projectal-4.0.0/projectal/entities/permission.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/project.py` & `projectal-4.0.0/projectal/entities/project.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/project_template.py` & `projectal-4.0.0/projectal/entities/project_template.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/staff.py` & `projectal-4.0.0/projectal/entities/staff.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/task.py` & `projectal-4.0.0/projectal/entities/task.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/task_template.py` & `projectal-4.0.0/projectal/entities/task_template.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/user.py` & `projectal-4.0.0/projectal/entities/user.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entities/webhook.py` & `projectal-4.0.0/projectal/entities/webhook.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/entity.py` & `projectal-4.0.0/projectal/entity.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/enums.py` & `projectal-4.0.0/projectal/enums.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/errors.py` & `projectal-4.0.0/projectal/errors.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/linkers.py` & `projectal-4.0.0/projectal/linkers.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal/profile.py` & `projectal-4.0.0/projectal/profile.py`

 * *Files identical despite different names*

### Comparing `projectal-3.1.1/projectal.egg-info/PKG-INFO` & `projectal-4.0.0/projectal.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectal
-Version: 3.1.1
+Version: 4.0.0
 Summary: Python bindings for the Projectal API
 Home-page: https://projectal.com/resources/developer
 Author: Projectal
 Author-email: support@projectal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `projectal-3.1.1/projectal.egg-info/SOURCES.txt` & `projectal-4.0.0/projectal.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,16 @@
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

### Comparing `projectal-3.1.1/setup.py` & `projectal-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='projectal',
-    version='3.1.1',
+    version='4.0.0',
     description='Python bindings for the Projectal API',
     long_description="The Python library allows developers to write Python-based apps that talk directly with Projectal. This gives developers immense freedom to access all data points in Projectal and to integrate Projectal with their workflow.",
     long_description_content_type="text/plain",
     url='https://projectal.com/resources/developer',
     author='Projectal',
     author_email='support@projectal.com',
     license='MIT',
```

