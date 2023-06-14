# Comparing `tmp/python-gerrit-api-2.1.6.tar.gz` & `tmp/python-gerrit-api-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gerrit-api-2.1.6.tar", last modified: Thu Dec  8 08:53:47 2022, max compression
+gzip compressed data, was "python-gerrit-api-2.1.7.tar", last modified: Wed Jun 14 04:48:27 2023, max compression
```

## Comparing `python-gerrit-api-2.1.6.tar` & `python-gerrit-api-2.1.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.330272 python-gerrit-api-2.1.6/
--rw-r--r--   0 shijialiang   (501) staff       (20)     1069 2022-07-25 01:29:00.000000 python-gerrit-api-2.1.6/LICENSE
--rw-r--r--   0 shijialiang   (501) staff       (20)       34 2022-07-25 01:29:00.000000 python-gerrit-api-2.1.6/MANIFEST.in
--rw-r--r--   0 shijialiang   (501) staff       (20)    10732 2022-12-08 08:53:47.329842 python-gerrit-api-2.1.6/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     9853 2022-10-19 05:47:23.000000 python-gerrit-api-2.1.6/README.rst
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.296268 python-gerrit-api-2.1.6/gerrit/
--rw-r--r--   0 shijialiang   (501) staff       (20)     6052 2022-12-08 08:53:18.000000 python-gerrit-api-2.1.6/gerrit/__init__.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.302063 python-gerrit-api-2.1.6/gerrit/accounts/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-07-25 01:29:00.000000 python-gerrit-api-2.1.6/gerrit/accounts/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    18170 2022-10-13 01:47:09.000000 python-gerrit-api-2.1.6/gerrit/accounts/account.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3295 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/accounts/accounts.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2085 2022-08-17 13:53:30.000000 python-gerrit-api-2.1.6/gerrit/accounts/emails.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4544 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/accounts/gpg_keys.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1890 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/accounts/ssh_keys.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.304937 python-gerrit-api-2.1.6/gerrit/changes/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-07-25 01:29:00.000000 python-gerrit-api-2.1.6/gerrit/changes/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    27580 2022-10-19 07:11:30.000000 python-gerrit-api-2.1.6/gerrit/changes/change.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2876 2022-12-08 08:53:18.000000 python-gerrit-api-2.1.6/gerrit/changes/changes.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4583 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/changes/edit.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2266 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/changes/messages.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4522 2022-08-17 13:53:30.000000 python-gerrit-api-2.1.6/gerrit/changes/reviewers.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.308281 python-gerrit-api-2.1.6/gerrit/changes/revision/
--rw-r--r--   0 shijialiang   (501) staff       (20)    13137 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/changes/revision/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2713 2022-11-25 02:07:31.000000 python-gerrit-api-2.1.6/gerrit/changes/revision/comments.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3916 2022-11-25 02:07:31.000000 python-gerrit-api-2.1.6/gerrit/changes/revision/drafts.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4630 2022-11-25 02:07:31.000000 python-gerrit-api-2.1.6/gerrit/changes/revision/files.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.311180 python-gerrit-api-2.1.6/gerrit/config/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-07-25 01:29:00.000000 python-gerrit-api-2.1.6/gerrit/config/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1958 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/config/caches.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     7218 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/config/config.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1621 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/config/tasks.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.311549 python-gerrit-api-2.1.6/gerrit/gitiles/
--rw-r--r--   0 shijialiang   (501) staff       (20)      691 2022-12-08 08:53:18.000000 python-gerrit-api-2.1.6/gerrit/gitiles/__init__.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.314446 python-gerrit-api-2.1.6/gerrit/groups/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-07-25 01:29:00.000000 python-gerrit-api-2.1.6/gerrit/groups/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5230 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/groups/group.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4033 2022-08-17 10:34:58.000000 python-gerrit-api-2.1.6/gerrit/groups/groups.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2153 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/groups/members.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2165 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/groups/subgroups.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.315543 python-gerrit-api-2.1.6/gerrit/plugins/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-07-25 01:29:00.000000 python-gerrit-api-2.1.6/gerrit/plugins/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3085 2022-08-17 13:53:30.000000 python-gerrit-api-2.1.6/gerrit/plugins/plugins.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.320262 python-gerrit-api-2.1.6/gerrit/projects/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-07-25 01:29:00.000000 python-gerrit-api-2.1.6/gerrit/projects/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3877 2022-08-17 13:53:30.000000 python-gerrit-api-2.1.6/gerrit/projects/branches.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1845 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/projects/commit.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2319 2022-08-17 13:53:30.000000 python-gerrit-api-2.1.6/gerrit/projects/dashboards.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4067 2022-08-17 13:53:30.000000 python-gerrit-api-2.1.6/gerrit/projects/labels.py
--rw-r--r--   0 shijialiang   (501) staff       (20)    13866 2022-10-13 01:47:09.000000 python-gerrit-api-2.1.6/gerrit/projects/project.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     5080 2022-08-17 13:53:30.000000 python-gerrit-api-2.1.6/gerrit/projects/projects.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2785 2022-08-17 13:53:30.000000 python-gerrit-api-2.1.6/gerrit/projects/tags.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2471 2022-08-17 13:53:30.000000 python-gerrit-api-2.1.6/gerrit/projects/webhooks.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.325502 python-gerrit-api-2.1.6/gerrit/utils/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2022-07-25 01:29:00.000000 python-gerrit-api-2.1.6/gerrit/utils/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2157 2022-08-17 10:34:58.000000 python-gerrit-api-2.1.6/gerrit/utils/common.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1275 2022-08-09 05:24:31.000000 python-gerrit-api-2.1.6/gerrit/utils/entity.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1851 2022-10-13 01:47:09.000000 python-gerrit-api-2.1.6/gerrit/utils/exceptions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1749 2022-10-13 02:13:54.000000 python-gerrit-api-2.1.6/gerrit/utils/models.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     7978 2022-10-13 02:51:00.000000 python-gerrit-api-2.1.6/gerrit/utils/requester.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2022-12-08 08:53:47.329529 python-gerrit-api-2.1.6/python_gerrit_api.egg-info/
--rw-r--r--   0 shijialiang   (501) staff       (20)    10732 2022-12-08 08:53:47.000000 python-gerrit-api-2.1.6/python_gerrit_api.egg-info/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     1433 2022-12-08 08:53:47.000000 python-gerrit-api-2.1.6/python_gerrit_api.egg-info/SOURCES.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        1 2022-12-08 08:53:47.000000 python-gerrit-api-2.1.6/python_gerrit_api.egg-info/dependency_links.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       31 2022-12-08 08:53:47.000000 python-gerrit-api-2.1.6/python_gerrit_api.egg-info/requires.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        7 2022-12-08 08:53:47.000000 python-gerrit-api-2.1.6/python_gerrit_api.egg-info/top_level.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       31 2022-10-13 02:51:00.000000 python-gerrit-api-2.1.6/requirements.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       38 2022-12-08 08:53:47.330317 python-gerrit-api-2.1.6/setup.cfg
--rw-r--r--   0 shijialiang   (501) staff       (20)     2028 2022-12-08 08:53:18.000000 python-gerrit-api-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.730738 python-gerrit-api-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-14 04:48:27.730738 python-gerrit-api-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.718738 python-gerrit-api-2.1.7/gerrit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.718738 python-gerrit-api-2.1.7/gerrit/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/gpg_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.722738 python-gerrit-api-2.1.7/gerrit/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27580 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/reviewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.722738 python-gerrit-api-2.1.7/gerrit/changes/revision/
+-rw-r--r--   0 runner    (1001) docker     (123)    13137 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/revision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/revision/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/revision/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/revision/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.722738 python-gerrit-api-2.1.7/gerrit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/config/caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/config/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.722738 python-gerrit-api-2.1.7/gerrit/gitiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/gitiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.722738 python-gerrit-api-2.1.7/gerrit/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/groups/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/groups/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/groups/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/groups/subgroups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.726739 python-gerrit-api-2.1.7/gerrit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.726739 python-gerrit-api-2.1.7/gerrit/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.730738 python-gerrit-api-2.1.7/gerrit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.730738 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-14 04:48:27.000000 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-14 04:48:27.000000 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:48:27.000000 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 04:48:27.000000 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 04:48:27.000000 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:48:27.730738 python-gerrit-api-2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/setup.py
```

### Comparing `python-gerrit-api-2.1.6/LICENSE` & `python-gerrit-api-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/PKG-INFO` & `python-gerrit-api-2.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -64,42 +64,27 @@
 
 .. code-block:: bash
 
     git clone https://github.com/shijl0925/python-gerrit-api.git
     cd python-gerrit-api
     python setup.py install
 
-Donate
-------
-
-donations are not mandatory but very welcomed
-If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
-
-Paypal
-------
-.. image:: https://raw.githubusercontent.com/andreostrovsky/donate-with-paypal/master/blue.svg
-    :target: https://paypal.me/shijialiang0925
-
-Wechat Pay
-----------
-.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/wechat.jpg
-
-Alipay
-------
-.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/alipay.jpg
-
 Usage
 -----
 
-Example 1: setup gerrit client::
+Example 1: setup gerrit client:
+
+.. code:: python
 
     from gerrit import GerritClient
     client = GerritClient(base_url="https://yourgerrit", username='******', password='xxxxx')
 
-Example 2: operate gerrit project::
+Example 2: operate gerrit project:
+
+.. code:: python
 
     # Retrieves a project.
     project = client.projects.get('MyProject')
 
     # or
     project = client.get(endpoint="/projects/MyProject")
 
@@ -146,15 +131,17 @@
     }
     new_branch = project.branches.create('stable', input_)
 
     # or
     result = client.put(endpoint="/projects/MyProject/branches/stable", json=input_)
 
 
-Example 3: operate gerrit change::
+Example 3: operate gerrit change:
+
+.. code:: python
 
     # Retrieves a change.
     change = client.changes.get('python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
     # or
     change = client.get(endpoint='/changes/python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
@@ -177,30 +164,34 @@
 
     # get a file by path
     file = revision.files.get('sonarqube/community/favorites.py')
 
     # Gets the diff of a file from a certain revision.
     file_diff = file.get_diff()
 
-Example 4: operate gerrit account::
+Example 4: operate gerrit account:
+
+.. code:: python
 
     # Retrieves an account
     account = client.accounts.get('kevin.shi')
 
     # Sets the full name of an account.
     input_ = {
         "name": "Keven Shi"
     }
     result = account.set_name(input_)
 
     # Adds an SSH key for a user.
     ssh_key = 'ssh-rsa xxx'
     result = account.ssh_keys.add(ssh_key)
 
-Example 5: operate gerrit group::
+Example 5: operate gerrit group:
+
+.. code:: python
 
     # Retrieves a group.
     group = client.groups.get('af01a8cb8cbd8ee7be072b98b1ee882867c0cf06')
 
     # Adds a user as member to a Gerrit internal group.
     result = group.add_member("ci_jenkins")
 
@@ -304,7 +295,26 @@
 Support and bug-reports: https://github.com/shijl0925/python-gerrit-api/issues?direction=desc&sort=comments&state=open
 
 Project source code: github: https://github.com/shijl0925/python-gerrit-api
 
 Project documentation: https://python-gerrit-api.readthedocs.org/en/latest/
 
 Releases: http://pypi.python.org/pypi/python-gerrit-api
+
+Donate
+------
+
+donations are not mandatory but very welcomed
+If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
+
+Paypal
+------
+.. image:: https://raw.githubusercontent.com/andreostrovsky/donate-with-paypal/master/blue.svg
+    :target: https://paypal.me/shijialiang0925
+
+Wechat Pay
+----------
+.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/wechat.jpg
+
+Alipay
+------
+.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/alipay.jpg
```

### Comparing `python-gerrit-api-2.1.6/README.rst` & `python-gerrit-api-2.1.7/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -41,42 +41,27 @@
 
 .. code-block:: bash
 
     git clone https://github.com/shijl0925/python-gerrit-api.git
     cd python-gerrit-api
     python setup.py install
 
-Donate
-------
-
-donations are not mandatory but very welcomed
-If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
-
-Paypal
-------
-.. image:: https://raw.githubusercontent.com/andreostrovsky/donate-with-paypal/master/blue.svg
-    :target: https://paypal.me/shijialiang0925
-
-Wechat Pay
-----------
-.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/wechat.jpg
-
-Alipay
-------
-.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/alipay.jpg
-
 Usage
 -----
 
-Example 1: setup gerrit client::
+Example 1: setup gerrit client:
+
+.. code:: python
 
     from gerrit import GerritClient
     client = GerritClient(base_url="https://yourgerrit", username='******', password='xxxxx')
 
-Example 2: operate gerrit project::
+Example 2: operate gerrit project:
+
+.. code:: python
 
     # Retrieves a project.
     project = client.projects.get('MyProject')
 
     # or
     project = client.get(endpoint="/projects/MyProject")
 
@@ -123,15 +108,17 @@
     }
     new_branch = project.branches.create('stable', input_)
 
     # or
     result = client.put(endpoint="/projects/MyProject/branches/stable", json=input_)
 
 
-Example 3: operate gerrit change::
+Example 3: operate gerrit change:
+
+.. code:: python
 
     # Retrieves a change.
     change = client.changes.get('python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
     # or
     change = client.get(endpoint='/changes/python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
@@ -154,30 +141,34 @@
 
     # get a file by path
     file = revision.files.get('sonarqube/community/favorites.py')
 
     # Gets the diff of a file from a certain revision.
     file_diff = file.get_diff()
 
-Example 4: operate gerrit account::
+Example 4: operate gerrit account:
+
+.. code:: python
 
     # Retrieves an account
     account = client.accounts.get('kevin.shi')
 
     # Sets the full name of an account.
     input_ = {
         "name": "Keven Shi"
     }
     result = account.set_name(input_)
 
     # Adds an SSH key for a user.
     ssh_key = 'ssh-rsa xxx'
     result = account.ssh_keys.add(ssh_key)
 
-Example 5: operate gerrit group::
+Example 5: operate gerrit group:
+
+.. code:: python
 
     # Retrieves a group.
     group = client.groups.get('af01a8cb8cbd8ee7be072b98b1ee882867c0cf06')
 
     # Adds a user as member to a Gerrit internal group.
     result = group.add_member("ci_jenkins")
 
@@ -281,7 +272,26 @@
 Support and bug-reports: https://github.com/shijl0925/python-gerrit-api/issues?direction=desc&sort=comments&state=open
 
 Project source code: github: https://github.com/shijl0925/python-gerrit-api
 
 Project documentation: https://python-gerrit-api.readthedocs.org/en/latest/
 
 Releases: http://pypi.python.org/pypi/python-gerrit-api
+
+Donate
+------
+
+donations are not mandatory but very welcomed
+If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
+
+Paypal
+------
+.. image:: https://raw.githubusercontent.com/andreostrovsky/donate-with-paypal/master/blue.svg
+    :target: https://paypal.me/shijialiang0925
+
+Wechat Pay
+----------
+.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/wechat.jpg
+
+Alipay
+------
+.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/alipay.jpg
```

### Comparing `python-gerrit-api-2.1.6/gerrit/__init__.py` & `python-gerrit-api-2.1.7/gerrit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+__version__ = "2.1.7"
+
 import json
 import netrc
 from gerrit.utils.requester import Requester
 from gerrit.config.config import GerritConfig
 from gerrit.projects.projects import GerritProjects
 from gerrit.accounts.accounts import GerritAccounts
 from gerrit.groups.groups import GerritGroups
```

### Comparing `python-gerrit-api-2.1.6/gerrit/accounts/account.py` & `python-gerrit-api-2.1.7/gerrit/accounts/account.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/accounts/accounts.py` & `python-gerrit-api-2.1.7/gerrit/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/accounts/emails.py` & `python-gerrit-api-2.1.7/gerrit/accounts/emails.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/accounts/gpg_keys.py` & `python-gerrit-api-2.1.7/gerrit/accounts/gpg_keys.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/accounts/ssh_keys.py` & `python-gerrit-api-2.1.7/gerrit/accounts/ssh_keys.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/changes/change.py` & `python-gerrit-api-2.1.7/gerrit/changes/change.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/changes/changes.py` & `python-gerrit-api-2.1.7/gerrit/changes/changes.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/changes/edit.py` & `python-gerrit-api-2.1.7/gerrit/changes/edit.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/changes/messages.py` & `python-gerrit-api-2.1.7/gerrit/changes/messages.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/changes/reviewers.py` & `python-gerrit-api-2.1.7/gerrit/changes/reviewers.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/changes/revision/__init__.py` & `python-gerrit-api-2.1.7/gerrit/changes/revision/__init__.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/changes/revision/comments.py` & `python-gerrit-api-2.1.7/gerrit/changes/revision/comments.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/changes/revision/drafts.py` & `python-gerrit-api-2.1.7/gerrit/changes/revision/drafts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/changes/revision/files.py` & `python-gerrit-api-2.1.7/gerrit/changes/revision/files.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/config/caches.py` & `python-gerrit-api-2.1.7/gerrit/config/caches.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/config/config.py` & `python-gerrit-api-2.1.7/gerrit/config/config.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/config/tasks.py` & `python-gerrit-api-2.1.7/gerrit/config/tasks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/gitiles/__init__.py` & `python-gerrit-api-2.1.7/gerrit/gitiles/__init__.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/groups/group.py` & `python-gerrit-api-2.1.7/gerrit/groups/group.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/groups/groups.py` & `python-gerrit-api-2.1.7/gerrit/groups/groups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/groups/members.py` & `python-gerrit-api-2.1.7/gerrit/groups/members.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/groups/subgroups.py` & `python-gerrit-api-2.1.7/gerrit/groups/subgroups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/plugins/plugins.py` & `python-gerrit-api-2.1.7/gerrit/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/projects/branches.py` & `python-gerrit-api-2.1.7/gerrit/projects/branches.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/projects/commit.py` & `python-gerrit-api-2.1.7/gerrit/projects/commit.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/projects/dashboards.py` & `python-gerrit-api-2.1.7/gerrit/projects/dashboards.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/projects/labels.py` & `python-gerrit-api-2.1.7/gerrit/projects/labels.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/projects/project.py` & `python-gerrit-api-2.1.7/gerrit/projects/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+from packaging.version import parse
 from gerrit.projects.branches import GerritProjectBranches
 from gerrit.projects.tags import GerritProjectTags
 from gerrit.projects.commit import GerritProjectCommit
 from gerrit.projects.dashboards import GerritProjectDashboards
 from gerrit.projects.labels import GerritProjectLabels
 from gerrit.projects.webhooks import GerritProjectWebHooks
 from gerrit.changes.change import GerritChange
```

### Comparing `python-gerrit-api-2.1.6/gerrit/projects/projects.py` & `python-gerrit-api-2.1.7/gerrit/projects/projects.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/projects/tags.py` & `python-gerrit-api-2.1.7/gerrit/projects/tags.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/projects/webhooks.py` & `python-gerrit-api-2.1.7/gerrit/projects/webhooks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/utils/common.py` & `python-gerrit-api-2.1.7/gerrit/utils/common.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/utils/entity.py` & `python-gerrit-api-2.1.7/gerrit/utils/entity.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/utils/exceptions.py` & `python-gerrit-api-2.1.7/gerrit/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/utils/models.py` & `python-gerrit-api-2.1.7/gerrit/utils/models.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/gerrit/utils/requester.py` & `python-gerrit-api-2.1.7/gerrit/utils/requester.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/python_gerrit_api.egg-info/PKG-INFO` & `python-gerrit-api-2.1.7/python_gerrit_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 2.1.6
+Version: 2.1.7
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -64,42 +64,27 @@
 
 .. code-block:: bash
 
     git clone https://github.com/shijl0925/python-gerrit-api.git
     cd python-gerrit-api
     python setup.py install
 
-Donate
-------
-
-donations are not mandatory but very welcomed
-If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
-
-Paypal
-------
-.. image:: https://raw.githubusercontent.com/andreostrovsky/donate-with-paypal/master/blue.svg
-    :target: https://paypal.me/shijialiang0925
-
-Wechat Pay
-----------
-.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/wechat.jpg
-
-Alipay
-------
-.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/alipay.jpg
-
 Usage
 -----
 
-Example 1: setup gerrit client::
+Example 1: setup gerrit client:
+
+.. code:: python
 
     from gerrit import GerritClient
     client = GerritClient(base_url="https://yourgerrit", username='******', password='xxxxx')
 
-Example 2: operate gerrit project::
+Example 2: operate gerrit project:
+
+.. code:: python
 
     # Retrieves a project.
     project = client.projects.get('MyProject')
 
     # or
     project = client.get(endpoint="/projects/MyProject")
 
@@ -146,15 +131,17 @@
     }
     new_branch = project.branches.create('stable', input_)
 
     # or
     result = client.put(endpoint="/projects/MyProject/branches/stable", json=input_)
 
 
-Example 3: operate gerrit change::
+Example 3: operate gerrit change:
+
+.. code:: python
 
     # Retrieves a change.
     change = client.changes.get('python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
     # or
     change = client.get(endpoint='/changes/python-sonarqube-api~stable3~I60c3bf10a5b0daf62a0f7c38bdf90b15026bbc2e')
 
@@ -177,30 +164,34 @@
 
     # get a file by path
     file = revision.files.get('sonarqube/community/favorites.py')
 
     # Gets the diff of a file from a certain revision.
     file_diff = file.get_diff()
 
-Example 4: operate gerrit account::
+Example 4: operate gerrit account:
+
+.. code:: python
 
     # Retrieves an account
     account = client.accounts.get('kevin.shi')
 
     # Sets the full name of an account.
     input_ = {
         "name": "Keven Shi"
     }
     result = account.set_name(input_)
 
     # Adds an SSH key for a user.
     ssh_key = 'ssh-rsa xxx'
     result = account.ssh_keys.add(ssh_key)
 
-Example 5: operate gerrit group::
+Example 5: operate gerrit group:
+
+.. code:: python
 
     # Retrieves a group.
     group = client.groups.get('af01a8cb8cbd8ee7be072b98b1ee882867c0cf06')
 
     # Adds a user as member to a Gerrit internal group.
     result = group.add_member("ci_jenkins")
 
@@ -304,7 +295,26 @@
 Support and bug-reports: https://github.com/shijl0925/python-gerrit-api/issues?direction=desc&sort=comments&state=open
 
 Project source code: github: https://github.com/shijl0925/python-gerrit-api
 
 Project documentation: https://python-gerrit-api.readthedocs.org/en/latest/
 
 Releases: http://pypi.python.org/pypi/python-gerrit-api
+
+Donate
+------
+
+donations are not mandatory but very welcomed
+If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
+
+Paypal
+------
+.. image:: https://raw.githubusercontent.com/andreostrovsky/donate-with-paypal/master/blue.svg
+    :target: https://paypal.me/shijialiang0925
+
+Wechat Pay
+----------
+.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/wechat.jpg
+
+Alipay
+------
+.. image:: https://raw.githubusercontent.com/shijl0925/python-gerrit-api/master/docs/alipay.jpg
```

### Comparing `python-gerrit-api-2.1.6/python_gerrit_api.egg-info/SOURCES.txt` & `python-gerrit-api-2.1.7/python_gerrit_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.6/setup.py` & `python-gerrit-api-2.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,27 @@
 # Get the long description from the relevant file
 with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
+def get_version() -> str:
+    version = ""
+    with open("gerrit/__init__.py", "r", encoding="utf-8") as f:
+        for line in f:
+            if line.startswith("__version__"):
+                version = eval(line.split("=")[-1])
+                break
+    return version
+
 setup(
     name="python-gerrit-api",
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="2.1.6",
+    version=get_version(),
     description="Python wrapper for the Gerrit REST API.",
     long_description=long_description,
     url="https://github.com/shijl0925/python-gerrit-api",
     author="Jialiang Shi",
     author_email="kevin09254930sjl@gmail.com",
     license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

