# Comparing `tmp/xj_user-1.2.98.tar.gz` & `tmp/xj_user-1.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_user-1.2.98.tar", last modified: Tue Feb 28 05:04:34 2023, max compression
+gzip compressed data, was "dist\xj_user-1.2.99.tar", last modified: Wed Mar  1 09:26:15 2023, max compression
```

## Comparing `xj_user-1.2.98.tar` & `xj_user-1.2.99.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 05:04:34.000000 xj_user-1.2.98/
--rw-rw-rw-   0        0        0      582 2023-02-28 05:04:34.000000 xj_user-1.2.98/PKG-INFO
--rw-rw-rw-   0        0        0      212 2022-08-25 05:15:54.000000 xj_user-1.2.98/README.md
--rw-rw-rw-   0        0        0       42 2023-02-28 05:04:34.000000 xj_user-1.2.98/setup.cfg
--rw-rw-rw-   0        0        0     2060 2023-02-28 05:04:23.000000 xj_user-1.2.98/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-28 05:04:34.000000 xj_user-1.2.98/xj_user/
--rw-rw-rw-   0        0        0        0 2023-01-09 07:55:37.000000 xj_user-1.2.98/xj_user/__init__.py
--rw-rw-rw-   0        0        0     5968 2023-01-05 00:47:18.000000 xj_user-1.2.98/xj_user/admin.py
--rw-rw-rw-   0        0        0     4367 2022-08-27 10:02:03.000000 xj_user-1.2.98/xj_user/api2.py
-drwxrwxrwx   0        0        0        0 2023-02-28 05:04:34.000000 xj_user-1.2.98/xj_user/apis/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_user-1.2.98/xj_user/apis/__init__.py
--rw-rw-rw-   0        0        0     6203 2022-12-05 10:39:40.000000 xj_user-1.2.98/xj_user/apis/user_add.py
--rw-rw-rw-   0        0        0     2939 2023-01-05 01:06:01.000000 xj_user-1.2.98/xj_user/apis/user_contact_book.py
--rw-rw-rw-   0        0        0     2980 2022-12-16 02:57:24.000000 xj_user-1.2.98/xj_user/apis/user_detail_info.py
--rw-rw-rw-   0        0        0    11751 2023-02-14 06:45:39.000000 xj_user-1.2.98/xj_user/apis/user_edit.py
--rw-rw-rw-   0        0        0      722 2022-09-01 06:39:57.000000 xj_user-1.2.98/xj_user/apis/user_group.py
--rw-rw-rw-   0        0        0      871 2022-09-02 06:16:55.000000 xj_user-1.2.98/xj_user/apis/user_group_tree.py
--rw-rw-rw-   0        0        0     4268 2023-02-04 04:11:11.000000 xj_user-1.2.98/xj_user/apis/user_info.py
--rw-rw-rw-   0        0        0     3849 2023-02-14 08:35:53.000000 xj_user-1.2.98/xj_user/apis/user_list.py
--rw-rw-rw-   0        0        0     4566 2023-02-04 04:11:11.000000 xj_user-1.2.98/xj_user/apis/user_login.py
--rw-rw-rw-   0        0        0     2792 2023-02-15 06:30:04.000000 xj_user-1.2.98/xj_user/apis/user_login_short_message.py
--rw-rw-rw-   0        0        0     1165 2023-02-15 07:20:59.000000 xj_user-1.2.98/xj_user/apis/user_login_wechat.py
--rw-rw-rw-   0        0        0     5057 2022-12-31 07:12:11.000000 xj_user-1.2.98/xj_user/apis/user_password.py
--rw-rw-rw-   0        0        0     1022 2022-09-01 06:39:57.000000 xj_user-1.2.98/xj_user/apis/user_permission.py
--rw-rw-rw-   0        0        0     3957 2023-02-14 01:11:46.000000 xj_user-1.2.98/xj_user/apis/user_platform.py
--rw-rw-rw-   0        0        0    11777 2022-12-16 02:16:23.000000 xj_user-1.2.98/xj_user/apis/user_register.py
--rw-rw-rw-   0        0        0     3163 2023-02-04 06:20:41.000000 xj_user-1.2.98/xj_user/apis/user_relate_apis.py
--rw-rw-rw-   0        0        0      970 2022-10-27 05:31:52.000000 xj_user-1.2.98/xj_user/apis/user_sso_serve.py
--rw-rw-rw-   0        0        0      579 2022-11-03 02:54:30.000000 xj_user-1.2.98/xj_user/apis/user_statistics.py
--rw-rw-rw-   0        0        0      202 2022-09-06 06:10:27.000000 xj_user-1.2.98/xj_user/apps.py
--rw-rw-rw-   0        0        0      466 2022-08-27 10:02:03.000000 xj_user-1.2.98/xj_user/config[del].py
-drwxrwxrwx   0        0        0        0 2023-02-28 05:04:34.000000 xj_user-1.2.98/xj_user/migrations/
--rw-rw-rw-   0        0        0      802 2023-02-02 00:46:15.000000 xj_user-1.2.98/xj_user/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-02-02 00:46:15.000000 xj_user-1.2.98/xj_user/migrations/__init__.py
--rw-rw-rw-   0        0        0    23147 2023-02-14 08:34:38.000000 xj_user-1.2.98/xj_user/models.py
-drwxrwxrwx   0        0        0        0 2023-02-28 05:04:34.000000 xj_user-1.2.98/xj_user/services/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_user-1.2.98/xj_user/services/__init__.py
--rw-rw-rw-   0        0        0     1064 2023-01-09 07:52:08.000000 xj_user-1.2.98/xj_user/services/contact_book.py
--rw-rw-rw-   0        0        0     7364 2023-02-14 08:30:04.000000 xj_user-1.2.98/xj_user/services/user_detail_info_service.py
--rw-rw-rw-   0        0        0     2335 2023-01-05 01:01:39.000000 xj_user-1.2.98/xj_user/services/user_group_tree_service.py
--rw-rw-rw-   0        0        0     4330 2022-10-16 06:45:39.000000 xj_user-1.2.98/xj_user/services/user_login_register.py
--rw-rw-rw-   0        0        0     3440 2022-09-01 05:25:48.000000 xj_user-1.2.98/xj_user/services/user_permission_service.py
--rw-rw-rw-   0        0        0     5344 2023-02-27 08:36:25.000000 xj_user-1.2.98/xj_user/services/user_platform_service.py
--rw-rw-rw-   0        0        0     8516 2023-02-27 02:23:09.000000 xj_user-1.2.98/xj_user/services/user_relate_service.py
--rw-rw-rw-   0        0        0     7752 2022-08-27 10:02:03.000000 xj_user-1.2.98/xj_user/services/user_service v1 [by dict].py
--rw-rw-rw-   0        0        0    31871 2023-02-28 01:15:45.000000 xj_user-1.2.98/xj_user/services/user_service.py
--rw-rw-rw-   0        0        0     7340 2023-02-15 07:22:49.000000 xj_user-1.2.98/xj_user/services/user_sms_service.py
--rw-rw-rw-   0        0        0     1021 2022-11-23 07:24:12.000000 xj_user-1.2.98/xj_user/services/user_sso_serve_service.py
--rw-rw-rw-   0        0        0      928 2022-11-03 03:05:27.000000 xj_user-1.2.98/xj_user/services/user_statistics_service.py
--rw-rw-rw-   0        0        0    11981 2023-02-15 07:23:16.000000 xj_user-1.2.98/xj_user/services/wechat_service.py
--rw-rw-rw-   0        0        0     3443 2023-02-14 06:25:15.000000 xj_user-1.2.98/xj_user/urls.py
-drwxrwxrwx   0        0        0        0 2023-02-28 05:04:34.000000 xj_user-1.2.98/xj_user/utils/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_user-1.2.98/xj_user/utils/__init__.py
--rw-rw-rw-   0        0        0     1076 2022-08-27 10:02:03.000000 xj_user-1.2.98/xj_user/utils/custom_authorization.py
--rw-rw-rw-   0        0        0     1463 2022-12-16 03:19:42.000000 xj_user-1.2.98/xj_user/utils/custom_response.py
--rw-rw-rw-   0        0        0     9769 2023-02-27 03:32:12.000000 xj_user-1.2.98/xj_user/utils/custom_tool.py
--rw-rw-rw-   0        0        0      814 2022-12-31 07:12:11.000000 xj_user-1.2.98/xj_user/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-08-27 10:02:03.000000 xj_user-1.2.98/xj_user/utils/j_dict.py
--rw-rw-rw-   0        0        0      464 2022-08-27 10:02:03.000000 xj_user-1.2.98/xj_user/utils/join_list.py
--rw-rw-rw-   0        0        0     7026 2022-12-13 05:27:07.000000 xj_user-1.2.98/xj_user/utils/model_handle.py
--rw-rw-rw-   0        0        0    41472 2022-11-03 03:06:06.000000 xj_user-1.2.98/xj_user/utils/nickname_generate.py
--rw-rw-rw-   0        0        0     4188 2022-12-31 07:12:11.000000 xj_user-1.2.98/xj_user/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     2682 2022-08-27 10:02:03.000000 xj_user-1.2.98/xj_user/utils/validator.py
--rw-rw-rw-   0        0        0      521 2022-08-27 10:02:03.000000 xj_user-1.2.98/xj_user/validator.py
--rw-rw-rw-   0        0        0     1627 2022-08-31 06:40:35.000000 xj_user-1.2.98/xj_user/views.py
-drwxrwxrwx   0        0        0        0 2023-02-28 05:04:34.000000 xj_user-1.2.98/xj_user.egg-info/
--rw-rw-rw-   0        0        0      582 2023-02-28 05:04:33.000000 xj_user-1.2.98/xj_user.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1856 2023-02-28 05:04:33.000000 xj_user-1.2.98/xj_user.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 05:04:33.000000 xj_user-1.2.98/xj_user.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-02-28 05:04:33.000000 xj_user-1.2.98/xj_user.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-28 05:04:33.000000 xj_user-1.2.98/xj_user.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-01 09:26:15.000000 xj_user-1.2.99/
+-rw-rw-rw-   0        0        0      582 2023-03-01 09:26:15.000000 xj_user-1.2.99/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2022-08-25 05:15:54.000000 xj_user-1.2.99/README.md
+-rw-rw-rw-   0        0        0       42 2023-03-01 09:26:15.000000 xj_user-1.2.99/setup.cfg
+-rw-rw-rw-   0        0        0     2060 2023-03-01 09:26:01.000000 xj_user-1.2.99/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-01 09:26:15.000000 xj_user-1.2.99/xj_user/
+-rw-rw-rw-   0        0        0        0 2023-01-09 07:55:37.000000 xj_user-1.2.99/xj_user/__init__.py
+-rw-rw-rw-   0        0        0     5968 2023-01-05 00:47:18.000000 xj_user-1.2.99/xj_user/admin.py
+-rw-rw-rw-   0        0        0     4367 2022-08-27 10:02:03.000000 xj_user-1.2.99/xj_user/api2.py
+drwxrwxrwx   0        0        0        0 2023-03-01 09:26:15.000000 xj_user-1.2.99/xj_user/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_user-1.2.99/xj_user/apis/__init__.py
+-rw-rw-rw-   0        0        0     6203 2022-12-05 10:39:40.000000 xj_user-1.2.99/xj_user/apis/user_add.py
+-rw-rw-rw-   0        0        0     2939 2023-01-05 01:06:01.000000 xj_user-1.2.99/xj_user/apis/user_contact_book.py
+-rw-rw-rw-   0        0        0     2980 2022-12-16 02:57:24.000000 xj_user-1.2.99/xj_user/apis/user_detail_info.py
+-rw-rw-rw-   0        0        0    11800 2023-03-01 08:52:55.000000 xj_user-1.2.99/xj_user/apis/user_edit.py
+-rw-rw-rw-   0        0        0      722 2022-09-01 06:39:57.000000 xj_user-1.2.99/xj_user/apis/user_group.py
+-rw-rw-rw-   0        0        0      871 2022-09-02 06:16:55.000000 xj_user-1.2.99/xj_user/apis/user_group_tree.py
+-rw-rw-rw-   0        0        0     4268 2023-02-04 04:11:11.000000 xj_user-1.2.99/xj_user/apis/user_info.py
+-rw-rw-rw-   0        0        0     3849 2023-02-14 08:35:53.000000 xj_user-1.2.99/xj_user/apis/user_list.py
+-rw-rw-rw-   0        0        0     4566 2023-02-04 04:11:11.000000 xj_user-1.2.99/xj_user/apis/user_login.py
+-rw-rw-rw-   0        0        0     2792 2023-02-15 06:30:04.000000 xj_user-1.2.99/xj_user/apis/user_login_short_message.py
+-rw-rw-rw-   0        0        0     1165 2023-02-15 07:20:59.000000 xj_user-1.2.99/xj_user/apis/user_login_wechat.py
+-rw-rw-rw-   0        0        0     5057 2022-12-31 07:12:11.000000 xj_user-1.2.99/xj_user/apis/user_password.py
+-rw-rw-rw-   0        0        0     1022 2022-09-01 06:39:57.000000 xj_user-1.2.99/xj_user/apis/user_permission.py
+-rw-rw-rw-   0        0        0     3957 2023-02-14 01:11:46.000000 xj_user-1.2.99/xj_user/apis/user_platform.py
+-rw-rw-rw-   0        0        0    11777 2022-12-16 02:16:23.000000 xj_user-1.2.99/xj_user/apis/user_register.py
+-rw-rw-rw-   0        0        0     3163 2023-02-04 06:20:41.000000 xj_user-1.2.99/xj_user/apis/user_relate_apis.py
+-rw-rw-rw-   0        0        0      970 2022-10-27 05:31:52.000000 xj_user-1.2.99/xj_user/apis/user_sso_serve.py
+-rw-rw-rw-   0        0        0      579 2022-11-03 02:54:30.000000 xj_user-1.2.99/xj_user/apis/user_statistics.py
+-rw-rw-rw-   0        0        0      202 2022-09-06 06:10:27.000000 xj_user-1.2.99/xj_user/apps.py
+-rw-rw-rw-   0        0        0      466 2022-08-27 10:02:03.000000 xj_user-1.2.99/xj_user/config[del].py
+drwxrwxrwx   0        0        0        0 2023-03-01 09:26:15.000000 xj_user-1.2.99/xj_user/migrations/
+-rw-rw-rw-   0        0        0      802 2023-02-02 00:46:15.000000 xj_user-1.2.99/xj_user/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 00:46:15.000000 xj_user-1.2.99/xj_user/migrations/__init__.py
+-rw-rw-rw-   0        0        0    23147 2023-02-14 08:34:38.000000 xj_user-1.2.99/xj_user/models.py
+drwxrwxrwx   0        0        0        0 2023-03-01 09:26:15.000000 xj_user-1.2.99/xj_user/services/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_user-1.2.99/xj_user/services/__init__.py
+-rw-rw-rw-   0        0        0     1064 2023-01-09 07:52:08.000000 xj_user-1.2.99/xj_user/services/contact_book.py
+-rw-rw-rw-   0        0        0     7364 2023-02-14 08:30:04.000000 xj_user-1.2.99/xj_user/services/user_detail_info_service.py
+-rw-rw-rw-   0        0        0     2335 2023-01-05 01:01:39.000000 xj_user-1.2.99/xj_user/services/user_group_tree_service.py
+-rw-rw-rw-   0        0        0     4330 2022-10-16 06:45:39.000000 xj_user-1.2.99/xj_user/services/user_login_register.py
+-rw-rw-rw-   0        0        0     3440 2022-09-01 05:25:48.000000 xj_user-1.2.99/xj_user/services/user_permission_service.py
+-rw-rw-rw-   0        0        0     5344 2023-02-27 08:36:25.000000 xj_user-1.2.99/xj_user/services/user_platform_service.py
+-rw-rw-rw-   0        0        0     8516 2023-02-27 02:23:09.000000 xj_user-1.2.99/xj_user/services/user_relate_service.py
+-rw-rw-rw-   0        0        0     7752 2022-08-27 10:02:03.000000 xj_user-1.2.99/xj_user/services/user_service v1 [by dict].py
+-rw-rw-rw-   0        0        0    31871 2023-02-28 01:15:45.000000 xj_user-1.2.99/xj_user/services/user_service.py
+-rw-rw-rw-   0        0        0     7340 2023-02-15 07:22:49.000000 xj_user-1.2.99/xj_user/services/user_sms_service.py
+-rw-rw-rw-   0        0        0     1021 2022-11-23 07:24:12.000000 xj_user-1.2.99/xj_user/services/user_sso_serve_service.py
+-rw-rw-rw-   0        0        0      928 2022-11-03 03:05:27.000000 xj_user-1.2.99/xj_user/services/user_statistics_service.py
+-rw-rw-rw-   0        0        0    11981 2023-02-15 07:23:16.000000 xj_user-1.2.99/xj_user/services/wechat_service.py
+-rw-rw-rw-   0        0        0     3443 2023-02-14 06:25:15.000000 xj_user-1.2.99/xj_user/urls.py
+drwxrwxrwx   0        0        0        0 2023-03-01 09:26:15.000000 xj_user-1.2.99/xj_user/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_user-1.2.99/xj_user/utils/__init__.py
+-rw-rw-rw-   0        0        0     1076 2022-08-27 10:02:03.000000 xj_user-1.2.99/xj_user/utils/custom_authorization.py
+-rw-rw-rw-   0        0        0     1463 2022-12-16 03:19:42.000000 xj_user-1.2.99/xj_user/utils/custom_response.py
+-rw-rw-rw-   0        0        0    12871 2023-03-01 09:21:08.000000 xj_user-1.2.99/xj_user/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      814 2022-12-31 07:12:11.000000 xj_user-1.2.99/xj_user/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-08-27 10:02:03.000000 xj_user-1.2.99/xj_user/utils/j_dict.py
+-rw-rw-rw-   0        0        0      464 2022-08-27 10:02:03.000000 xj_user-1.2.99/xj_user/utils/join_list.py
+-rw-rw-rw-   0        0        0     7026 2022-12-13 05:27:07.000000 xj_user-1.2.99/xj_user/utils/model_handle.py
+-rw-rw-rw-   0        0        0    41472 2022-11-03 03:06:06.000000 xj_user-1.2.99/xj_user/utils/nickname_generate.py
+-rw-rw-rw-   0        0        0     4188 2022-12-31 07:12:11.000000 xj_user-1.2.99/xj_user/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     2682 2022-08-27 10:02:03.000000 xj_user-1.2.99/xj_user/utils/validator.py
+-rw-rw-rw-   0        0        0      521 2022-08-27 10:02:03.000000 xj_user-1.2.99/xj_user/validator.py
+-rw-rw-rw-   0        0        0     1627 2022-08-31 06:40:35.000000 xj_user-1.2.99/xj_user/views.py
+drwxrwxrwx   0        0        0        0 2023-03-01 09:26:15.000000 xj_user-1.2.99/xj_user.egg-info/
+-rw-rw-rw-   0        0        0      582 2023-03-01 09:26:15.000000 xj_user-1.2.99/xj_user.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1856 2023-03-01 09:26:15.000000 xj_user-1.2.99/xj_user.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-01 09:26:15.000000 xj_user-1.2.99/xj_user.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-03-01 09:26:15.000000 xj_user-1.2.99/xj_user.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-03-01 09:26:15.000000 xj_user-1.2.99/xj_user.egg-info/top_level.txt
```

### Comparing `xj_user-1.2.98/PKG-INFO` & `xj_user-1.2.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_user
-Version: 1.2.98
+Version: 1.2.99
 Summary: 用户模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # Xj-User Module
         
         > 用户模块
```

### Comparing `xj_user-1.2.98/setup.py` & `xj_user-1.2.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_user',  # 模块名称
-    version='1.2.98',  # 模块版本
+    version='1.2.99',  # 模块版本
     description='用户模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     # author='sieyoo',
     # author_email='sieyoo@163.com',
     packages=find_packages(),  # 系统自动从当前目录开始找包
     # packages=['xj_user'],  # 系指定安装模块
```

### Comparing `xj_user-1.2.98/xj_user/admin.py` & `xj_user-1.2.99/xj_user/admin.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/api2.py` & `xj_user-1.2.99/xj_user/api2.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_add.py` & `xj_user-1.2.99/xj_user/apis/user_add.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_contact_book.py` & `xj_user-1.2.99/xj_user/apis/user_contact_book.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_detail_info.py` & `xj_user-1.2.99/xj_user/apis/user_detail_info.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_edit.py` & `xj_user-1.2.99/xj_user/apis/user_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from rest_framework import serializers
 from rest_framework.permissions import AllowAny
 
 from main.settings import BASE_DIR
 from xj_role.services.role_service import RoleService
 from xj_role.services.user_group_service import UserGroupService
 from ..models import *
-from ..services.user_detail_info_service import DetailInfoService, request_params_wrapper
+from ..services.user_detail_info_service import DetailInfoService, request_params_wrapper, flow_service_wrapper
 from ..services.user_service import UserService
 from ..utils.custom_response import util_response
 from ..utils.j_config import JConfig
 from ..utils.j_dict import JDict
 from ..utils.model_handle import parse_data
 from ..utils.user_wrapper import user_authentication_force_wrapper
 
@@ -255,14 +255,15 @@
                 'msg': '未知错误'
             }
 
         return response.Response(data=res, status=None, template_name=None, headers={"Authorization": token}, content_type=None)
 
     @user_authentication_force_wrapper
     @request_params_wrapper
+    @flow_service_wrapper
     def user_edit_v2(self, *args, user_info=None, request_params=None, **kwargs):
         if request_params is None:
             request_params = {}
         if user_info is None:
             user_info = {}
 
         user_id = request_params.pop("user_id", None) or user_info.get("user_id")  # 没有传则修改当前的用户的信息
```

### Comparing `xj_user-1.2.98/xj_user/apis/user_group.py` & `xj_user-1.2.99/xj_user/apis/user_group.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_group_tree.py` & `xj_user-1.2.99/xj_user/apis/user_group_tree.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_info.py` & `xj_user-1.2.99/xj_user/apis/user_info.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_list.py` & `xj_user-1.2.99/xj_user/apis/user_list.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_login.py` & `xj_user-1.2.99/xj_user/apis/user_login.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_login_short_message.py` & `xj_user-1.2.99/xj_user/apis/user_login_short_message.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_login_wechat.py` & `xj_user-1.2.99/xj_user/apis/user_login_wechat.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_password.py` & `xj_user-1.2.99/xj_user/apis/user_password.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_permission.py` & `xj_user-1.2.99/xj_user/apis/user_permission.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_platform.py` & `xj_user-1.2.99/xj_user/apis/user_platform.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_register.py` & `xj_user-1.2.99/xj_user/apis/user_register.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_relate_apis.py` & `xj_user-1.2.99/xj_user/apis/user_relate_apis.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_sso_serve.py` & `xj_user-1.2.99/xj_user/apis/user_sso_serve.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/apis/user_statistics.py` & `xj_user-1.2.99/xj_user/apis/user_statistics.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/migrations/0001_initial.py` & `xj_user-1.2.99/xj_user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/models.py` & `xj_user-1.2.99/xj_user/models.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/contact_book.py` & `xj_user-1.2.99/xj_user/services/contact_book.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/user_detail_info_service.py` & `xj_user-1.2.99/xj_user/services/user_detail_info_service.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/user_group_tree_service.py` & `xj_user-1.2.99/xj_user/services/user_group_tree_service.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/user_login_register.py` & `xj_user-1.2.99/xj_user/services/user_login_register.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/user_permission_service.py` & `xj_user-1.2.99/xj_user/services/user_permission_service.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/user_platform_service.py` & `xj_user-1.2.99/xj_user/services/user_platform_service.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/user_relate_service.py` & `xj_user-1.2.99/xj_user/services/user_relate_service.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/user_service v1 [by dict].py` & `xj_user-1.2.99/xj_user/services/user_service v1 [by dict].py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/user_service.py` & `xj_user-1.2.99/xj_user/services/user_service.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/user_sms_service.py` & `xj_user-1.2.99/xj_user/services/user_sms_service.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/user_sso_serve_service.py` & `xj_user-1.2.99/xj_user/services/user_sso_serve_service.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/user_statistics_service.py` & `xj_user-1.2.99/xj_user/services/user_statistics_service.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/services/wechat_service.py` & `xj_user-1.2.99/xj_user/services/wechat_service.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/urls.py` & `xj_user-1.2.99/xj_user/urls.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/utils/custom_authorization.py` & `xj_user-1.2.99/xj_user/utils/custom_authorization.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/utils/custom_response.py` & `xj_user-1.2.99/xj_user/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/utils/custom_tool.py` & `xj_user-1.2.99/xj_user/utils/custom_tool.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 @author: 孙楷炎
 @Email: sky4834@163.com
 @synopsis: CURD 工具
 @created_time: 2022/6/15 14:14
 """
 
 import json
+from logging import getLogger
 import random
+import sys
+import time
 from urllib.parse import parse_qs
 import uuid
 
 from django.core.handlers.asgi import ASGIRequest
 from django.core.handlers.wsgi import WSGIRequest
 from rest_framework.request import Request
 import xmltodict
@@ -262,7 +265,75 @@
     buffer = []
     for i in range(0, length):
         start = i * 4
         end = i * 4 + 4
         val = int(random_id[start:end], 16)
         buffer.append(dictionary[val % 62])
     return "".join(buffer)
+
+
+def write_to_log(level="info", prefix="系统异常", content="", err_obj=None):
+    """
+    写入日志, 注意仅仅支持python3.0以上版本
+    :param level: 写入错误日志等级
+    :param prefix: 提示错误类型
+    :param content: 错误内容
+    :param err_obj: try except 捕捉到的错误对象, 自动处理日志格式
+    :return: data, err_msg
+    """
+    logger = getLogger('log')
+    try:
+        if not err_obj is None:
+            logger.error(
+                '---' + prefix + ":" + str(err_obj) + ";" +
+                (" content:" + str(content) + ";" if content else "") +
+                " line:" + str(err_obj.__traceback__.tb_lineno) + ";" +
+                " file:" + str(err_obj.__traceback__.tb_frame.f_globals["__file__"]) + ";" +
+                " datetime:" + time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(time.time())) + ";"
+            )
+
+        if level == "info":
+            logger.error('---' + prefix + ":" + str(content))
+        elif level == "error":
+            logger.error('---' + prefix + ":" + str(content))
+        return True, None
+    except Exception as err:
+        return False, str(err)
+
+
+def flow_service_wrapper(func):
+    """
+    API 流程中间件装饰器
+    PS 该装饰器必须配套request_params_wrapper装饰一起使用
+    """
+    if not sys.modules.get("xj_flow.services.flow_process_service.FlowProcessService"):
+        from xj_flow.services.flow_process_service import FlowProcessService
+
+    # 解析请求参数 兼容 APIView与View的情况，View 没有request.data
+    def wrapper(instance, arg_request=None, *args, request=None, request_params=None, **kwargs):
+        """
+        @param instance 实例是一个APIView的实例
+        @param args 其它可变参数元组
+        @param kwargs 其它可变关键字参数字典
+        :param request_params: 请求参数解析
+        """
+        if isinstance(instance, WSGIRequest) or isinstance(instance, Request) or isinstance(instance, ASGIRequest):
+            request = instance
+        if isinstance(arg_request, WSGIRequest) or isinstance(arg_request, Request) or isinstance(arg_request, ASGIRequest):
+            request = arg_request
+        if request_params is None:
+            request_params = {}
+
+        flow_node_id = request_params.pop("flow_node_id", None)
+        flow_action_id = request_params.pop("flow_action_id", None)
+        if not flow_node_id or not flow_action_id:
+            return func(instance, *args, request=request, request_params=request_params, **kwargs, )
+
+        service = FlowProcessService()
+        data, err = service.do_once_flow_in_service(flow_node_id, flow_action_id, source_params=request_params)
+        if err:
+            write_to_log(prefix="流程装饰器调用异常:", content=err)
+
+        request_params = data.get("source_params", request_params)
+        return func(instance, *args, request=request, request_params=request_params, **kwargs, )
+
+    return wrapper
```

### Comparing `xj_user-1.2.98/xj_user/utils/j_config.py` & `xj_user-1.2.99/xj_user/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/utils/model_handle.py` & `xj_user-1.2.99/xj_user/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/utils/nickname_generate.py` & `xj_user-1.2.99/xj_user/utils/nickname_generate.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/utils/user_wrapper.py` & `xj_user-1.2.99/xj_user/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/utils/validator.py` & `xj_user-1.2.99/xj_user/utils/validator.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/validator.py` & `xj_user-1.2.99/xj_user/validator.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user/views.py` & `xj_user-1.2.99/xj_user/views.py`

 * *Files identical despite different names*

### Comparing `xj_user-1.2.98/xj_user.egg-info/PKG-INFO` & `xj_user-1.2.99/xj_user.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-user
-Version: 1.2.98
+Version: 1.2.99
 Summary: 用户模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # Xj-User Module
         
         > 用户模块
```

### Comparing `xj_user-1.2.98/xj_user.egg-info/SOURCES.txt` & `xj_user-1.2.99/xj_user.egg-info/SOURCES.txt`

 * *Files identical despite different names*

