# Comparing `tmp/codeforlife-portal-6.8.9.tar.gz` & `tmp/codeforlife-portal-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeforlife-portal-6.8.9.tar", last modified: Tue Jun 21 09:04:13 2022, max compression
+gzip compressed data, was "codeforlife-portal-6.9.0.tar", last modified: Thu Jun 23 09:40:37 2022, max compression
```

## Comparing `codeforlife-portal-6.8.9.tar` & `codeforlife-portal-6.9.0.tar`

### file list

```diff
@@ -1,628 +1,628 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.696796 codeforlife-portal-6.8.9/
--rw-r--r--   0 root         (0) root         (0)    38929 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      165 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      293 2022-06-21 09:04:13.696796 codeforlife-portal-6.8.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1256 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.552796 codeforlife-portal-6.8.9/codeforlife_portal.egg-info/
--rw-r--r--   0 root         (0) root         (0)      293 2022-06-21 09:04:13.000000 codeforlife-portal-6.8.9/codeforlife_portal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25628 2022-06-21 09:04:13.000000 codeforlife-portal-6.8.9/codeforlife_portal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-21 09:04:13.000000 codeforlife-portal-6.8.9/codeforlife_portal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-21 09:00:41.000000 codeforlife-portal-6.8.9/codeforlife_portal.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      505 2022-06-21 09:04:13.000000 codeforlife-portal-6.8.9/codeforlife_portal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-06-21 09:04:13.000000 codeforlife-portal-6.8.9/codeforlife_portal.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.552796 codeforlife-portal-6.8.9/deploy/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/__init__.py
--rw-r--r--   0 root         (0) root         (0)       23 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/captcha.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.552796 codeforlife-portal-6.8.9/deploy/middleware/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/middleware/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1207 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/middleware/admin_access.py
--rw-r--r--   0 root         (0) root         (0)     1170 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/middleware/basicauth.py
--rw-r--r--   0 root         (0) root         (0)      474 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/middleware/exceptionlogging.py
--rw-r--r--   0 root         (0) root         (0)      751 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/middleware/security.py
--rw-r--r--   0 root         (0) root         (0)      881 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/middleware/session_timeout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.552796 codeforlife-portal-6.8.9/deploy/static/
--rw-r--r--   0 root         (0) root         (0)    24583 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/static/apple-touch-icon-120x120.png
--rw-r--r--   0 root         (0) root         (0)    36276 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/static/apple-touch-icon-152x152.png
--rw-r--r--   0 root         (0) root         (0)    47948 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/static/apple-touch-icon-180x180.png
--rw-r--r--   0 root         (0) root         (0)    11676 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/static/apple-touch-icon-76x76.png
--rw-r--r--   0 root         (0) root         (0)     7842 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/static/apple-touch-icon.png
--rw-r--r--   0 root         (0) root         (0)       24 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/static/robots.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.536796 codeforlife-portal-6.8.9/deploy/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.556796 codeforlife-portal-6.8.9/deploy/templates/deploy/
--rw-r--r--   0 root         (0) root         (0)      412 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/templates/deploy/csrf_failure.html
--rw-r--r--   0 root         (0) root         (0)      131 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/deploy/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.556796 codeforlife-portal-6.8.9/portal/
--rw-r--r--   0 root         (0) root         (0)       22 2022-06-21 09:04:10.000000 codeforlife-portal-6.8.9/portal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3284 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/admin.py
--rw-r--r--   0 root         (0) root         (0)      606 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/app_settings.py
--rw-r--r--   0 root         (0) root         (0)     5241 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/autoconfig.py
--rw-r--r--   0 root         (0) root         (0)      812 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/backends.py
--rw-r--r--   0 root         (0) root         (0)      255 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/beta.py
--rw-r--r--   0 root         (0) root         (0)      133 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/context_processors.py
--rw-r--r--   0 root         (0) root         (0)     1979 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/csp_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.560796 codeforlife-portal-6.8.9/portal/forms/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/forms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1045 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/forms/add_game.py
--rw-r--r--   0 root         (0) root         (0)     2080 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/forms/admin.py
--rw-r--r--   0 root         (0) root         (0)      761 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/forms/dotmailer.py
--rw-r--r--   0 root         (0) root         (0)      148 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/forms/error_messages.py
--rw-r--r--   0 root         (0) root         (0)      430 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/forms/invite_teacher.py
--rw-r--r--   0 root         (0) root         (0)     3519 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/forms/organisation.py
--rw-r--r--   0 root         (0) root         (0)    10722 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/forms/play.py
--rw-r--r--   0 root         (0) root         (0)     5928 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/forms/registration.py
--rw-r--r--   0 root         (0) root         (0)    19219 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/forms/teach.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.560796 codeforlife-portal-6.8.9/portal/frontend/
--rw-r--r--   0 root         (0) root         (0)      993 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/asset-manifest.json
--rw-r--r--   0 root         (0) root         (0)      481 2022-06-21 09:03:32.000000 codeforlife-portal-6.8.9/portal/frontend/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     1003 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/index.html
--rw-r--r--   0 root         (0) root         (0)      492 2022-06-21 09:03:32.000000 codeforlife-portal-6.8.9/portal/frontend/manifest.json
--rw-r--r--   0 root         (0) root         (0)       40 2022-06-21 09:03:32.000000 codeforlife-portal-6.8.9/portal/frontend/portal.css
--rw-r--r--   0 root         (0) root         (0)       67 2022-06-21 09:03:32.000000 codeforlife-portal-6.8.9/portal/frontend/robots.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.536796 codeforlife-portal-6.8.9/portal/frontend/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.560796 codeforlife-portal-6.8.9/portal/frontend/static/css/
--rw-r--r--   0 root         (0) root         (0)       73 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/css/main.acb3d7db.css
--rw-r--r--   0 root         (0) root         (0)      207 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/css/main.acb3d7db.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.564796 codeforlife-portal-6.8.9/portal/frontend/static/js/
--rw-r--r--   0 root         (0) root         (0)     4597 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/js/787.cda612ba.chunk.js
--rw-r--r--   0 root         (0) root         (0)    10281 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/js/787.cda612ba.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)   345455 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/js/main.8c02947d.js
--rw-r--r--   0 root         (0) root         (0)     1694 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/js/main.8c02947d.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)  1283202 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/js/main.8c02947d.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.568796 codeforlife-portal-6.8.9/portal/frontend/static/media/
--rw-r--r--   0 root         (0) root         (0)      524 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/media/facebook.2bdba6ecdf25da4a6d91d9df9e3f5830.svg
--rw-r--r--   0 root         (0) root         (0)    16839 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/media/logo_cfl.06fffc34beb6c215ab01.png
--rw-r--r--   0 root         (0) root         (0)     5451 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/media/logo_ocado_group.bf2daf768df6901d40924159853b612d.svg
--rw-r--r--   0 root         (0) root         (0)    10993 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/media/ocado.5e7ae9a2adbc50ec6f96f3f6366eea25.svg
--rw-r--r--   0 root         (0) root         (0)      896 2022-06-21 09:04:08.000000 codeforlife-portal-6.8.9/portal/frontend/static/media/twitter.3f190a3549dea2464ca62924d629b961.svg
--rw-r--r--   0 root         (0) root         (0)      422 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.568796 codeforlife-portal-6.8.9/portal/helpers/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      254 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/helpers/captcha.py
--rw-r--r--   0 root         (0) root         (0)     2560 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/helpers/decorators.py
--rw-r--r--   0 root         (0) root         (0)     3483 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/helpers/password.py
--rw-r--r--   0 root         (0) root         (0)     6148 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/helpers/ratelimit.py
--rw-r--r--   0 root         (0) root         (0)      125 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/helpers/regexes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.576796 codeforlife-portal-6.8.9/portal/migrations/
--rw-r--r--   0 root         (0) root         (0)    29559 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0001_squashed_0041_new_news.py
--rw-r--r--   0 root         (0) root         (0)      423 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0042_school_country.py
--rw-r--r--   0 root         (0) root         (0)      461 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0043_auto_20150430_0952.py
--rw-r--r--   0 root         (0) root         (0)     1123 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0044_auto_20150430_0959.py
--rw-r--r--   0 root         (0) root         (0)      412 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0045_auto_20150430_1446.py
--rw-r--r--   0 root         (0) root         (0)      540 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0046_auto_20150723_1101.py
--rw-r--r--   0 root         (0) root         (0)      267 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0047_remove_userprofile_avatar.py
--rw-r--r--   0 root         (0) root         (0)      349 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0048_plural_management_frontnews.py
--rw-r--r--   0 root         (0) root         (0)     1091 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0049_refactor_emailverifications.py
--rw-r--r--   0 root         (0) root         (0)      876 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0050_refactor_emailverifications_2.py
--rw-r--r--   0 root         (0) root         (0)     1044 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0051_add_missing_ev_records.py
--rw-r--r--   0 root         (0) root         (0)      284 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0052_refactor_emailverifications_3.py
--rw-r--r--   0 root         (0) root         (0)     2134 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0053_refactor_teacher_student_1.py
--rw-r--r--   0 root         (0) root         (0)      564 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0054_pending_join_request_can_be_blank.py
--rw-r--r--   0 root         (0) root         (0)      557 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0055_add_preview_user.py
--rw-r--r--   0 root         (0) root         (0)      409 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0056_remove_preview_user.py
--rw-r--r--   0 root         (0) root         (0)      291 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0057_delete_frontpagenews.py
--rw-r--r--   0 root         (0) root         (0)     7111 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0058_move_to_common_models.py
--rw-r--r--   0 root         (0) root         (0)     1020 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0059_move_email_verifications_to_common.py
--rw-r--r--   0 root         (0) root         (0)      627 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0060_delete_guardian.py
--rw-r--r--   0 root         (0) root         (0)     3811 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0061_make_portaladmin_teacher.py
--rw-r--r--   0 root         (0) root         (0)     1306 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/0062_verify_portaladmin.py
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.576796 codeforlife-portal-6.8.9/portal/pipeline_compilers/
--rw-r--r--   0 root         (0) root         (0)       85 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/pipeline_compilers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      742 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/pipeline_compilers/libsass_compiler.py
--rw-r--r--   0 root         (0) root         (0)      227 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/reactTestSpace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.536796 codeforlife-portal-6.8.9/portal/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.540796 codeforlife-portal-6.8.9/portal/static/portal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.540796 codeforlife-portal-6.8.9/portal/static/portal/fonts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.576796 codeforlife-portal-6.8.9/portal/static/portal/fonts/bootstrap/
--rw-r--r--   0 root         (0) root         (0)    20127 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.eot
--rw-r--r--   0 root         (0) root         (0)   108738 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.svg
--rw-r--r--   0 root         (0) root         (0)    45404 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.ttf
--rw-r--r--   0 root         (0) root         (0)    23424 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.woff
--rw-r--r--   0 root         (0) root         (0)    18028 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.612796 codeforlife-portal-6.8.9/portal/static/portal/img/
--rw-r--r--   0 root         (0) root         (0)     3329 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/10x_logo.png
--rw-r--r--   0 root         (0) root         (0)    64472 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/RR_logo_grass_background.png
--rw-r--r--   0 root         (0) root         (0)  1177416 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/RR_logo_green.svg
--rw-r--r--   0 root         (0) root         (0)     8799 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/RR_logo_simple.png
--rw-r--r--   0 root         (0) root         (0)   140736 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/about_us_cfl.jpg
--rw-r--r--   0 root         (0) root         (0)    19287 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/about_us_hero.jpg
--rw-r--r--   0 root         (0) root         (0)   118428 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/about_us_ocado.jpg
--rw-r--r--   0 root         (0) root         (0)     9038 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/barefoot_logo.png
--rw-r--r--   0 root         (0) root         (0)     7562 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/bcs_logo.png
--rw-r--r--   0 root         (0) root         (0)   159021 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/clubs.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.612796 codeforlife-portal-6.8.9/portal/static/portal/img/colorboxImages/
--rwxr-xr-x   0 root         (0) root         (0)      112 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/colorboxImages/border.png
--rwxr-xr-x   0 root         (0) root         (0)     2893 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/colorboxImages/controls.png
--rwxr-xr-x   0 root         (0) root         (0)     9427 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/colorboxImages/loading.gif
--rwxr-xr-x   0 root         (0) root         (0)      157 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/colorboxImages/loading_background.png
--rwxr-xr-x   0 root         (0) root         (0)      182 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/colorboxImages/overlay.png
--rw-r--r--   0 root         (0) root         (0)     3723 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/confirmation_tick.png
--rw-r--r--   0 root         (0) root         (0)     1143 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/cross.png
--rw-r--r--   0 root         (0) root         (0)    45387 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/dee.png
--rw-r--r--   0 root         (0) root         (0)     6543 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/facebook.png
--rw-r--r--   0 root         (0) root         (0)      481 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   176315 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/get_involved_hero.png
--rw-r--r--   0 root         (0) root         (0)   177664 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/gitbook.png
--rw-r--r--   0 root         (0) root         (0)    62646 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/gitbook_space.png
--rw-r--r--   0 root         (0) root         (0)    63596 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/github.png
--rw-r--r--   0 root         (0) root         (0)    47014 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/github_hero.png
--rw-r--r--   0 root         (0) root         (0)     4387 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/gla_logo.png
--rw-r--r--   0 root         (0) root         (0)     1133 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/hamburger.png
--rw-r--r--   0 root         (0) root         (0)    47601 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/help_and_support_hero.jpg
--rw-r--r--   0 root         (0) root         (0)   194269 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/home_educate.png
--rw-r--r--   0 root         (0) root         (0)    88389 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/home_educate_hero.jpg
--rw-r--r--   0 root         (0) root         (0)    62414 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/home_learning_hero.jpg
--rw-r--r--   0 root         (0) root         (0)   191553 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/home_play.png
--rw-r--r--   0 root         (0) root         (0)   110397 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/home_play_hero.jpg
--rw-r--r--   0 root         (0) root         (0)     7967 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/hope_logo.png
--rw-r--r--   0 root         (0) root         (0)     3260 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/icl_logo.png
--rw-r--r--   0 root         (0) root         (0)     5948 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/icon_controller.png
--rw-r--r--   0 root         (0) root         (0)    19299 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/icon_free.png
--rw-r--r--   0 root         (0) root         (0)     6044 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/icon_globe.png
--rw-r--r--   0 root         (0) root         (0)     2636 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/icon_piechart.png
--rw-r--r--   0 root         (0) root         (0)     5006 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/icon_step_by_step.png
--rw-r--r--   0 root         (0) root         (0)      761 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/icon_tracking.png
--rw-r--r--   0 root         (0) root         (0)     6052 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/icon_uk_flag.png
--rw-r--r--   0 root         (0) root         (0)    31240 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/kirsty.png
--rw-r--r--   0 root         (0) root         (0)    80736 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/kurono_hero.jpg
--rw-r--r--   0 root         (0) root         (0)   254014 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/kurono_landing_hero.png
--rw-r--r--   0 root         (0) root         (0)     2930 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/kurono_logo.svg
--rw-r--r--   0 root         (0) root         (0)     3017 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/kurono_logo_grey_background.svg
--rw-r--r--   0 root         (0) root         (0)     1494 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/kurono_logo_mark.svg
--rw-r--r--   0 root         (0) root         (0)   119585 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/kurono_resources_hero.jpg
--rw-r--r--   0 root         (0) root         (0)   737438 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/kurono_story.png
--rw-r--r--   0 root         (0) root         (0)    16839 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/logo_cfl.png
--rw-r--r--   0 root         (0) root         (0)     8599 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/logo_cfl_reminder_cards.jpg
--rw-r--r--   0 root         (0) root         (0)     4747 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/logo_cfl_white_landscape.png
--rw-r--r--   0 root         (0) root         (0)     5232 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/logo_ocado.png
--rw-r--r--   0 root         (0) root         (0)     2543 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/logo_ocado_group.png
--rw-r--r--   0 root         (0) root         (0)     5451 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/logo_ocado_group.svg
--rw-r--r--   0 root         (0) root         (0)    10993 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/logo_ocado_group_white.svg
--rw-r--r--   0 root         (0) root         (0)     3095 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/mc_saatchi_logo.png
--rw-r--r--   0 root         (0) root         (0)    49149 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/nigel.png
--rw-r--r--   0 root         (0) root         (0)     2447 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/ocado-swirl.svg
--rw-r--r--   0 root         (0) root         (0)      511 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/oval_blue.svg
--rw-r--r--   0 root         (0) root         (0)      515 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/oval_pink.svg
--rw-r--r--   0 root         (0) root         (0)      511 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/oval_yellow.svg
--rw-r--r--   0 root         (0) root         (0)     2728 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/paper_plane.png
--rw-r--r--   0 root         (0) root         (0)    60371 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/phil.png
--rw-r--r--   0 root         (0) root         (0)      583 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/polygon_blue.svg
--rw-r--r--   0 root         (0) root         (0)      579 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/polygon_pink.svg
--rw-r--r--   0 root         (0) root         (0)      579 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/polygon_yellow.svg
--rw-r--r--   0 root         (0) root         (0)     2876 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/pressure_cooker_logo.png
--rw-r--r--   0 root         (0) root         (0)    77059 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/rapid_router.png
--rw-r--r--   0 root         (0) root         (0)   146564 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/rapid_router_landing_hero.png
--rw-r--r--   0 root         (0) root         (0)    36268 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/rapidrouter.png
--rw-r--r--   0 root         (0) root         (0)    65998 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/resources_hero.jpg
--rw-r--r--   0 root         (0) root         (0)    74159 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/resources_montage.jpg
--rw-r--r--   0 root         (0) root         (0)    93064 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/reuben.png
--rw-r--r--   0 root         (0) root         (0)   103324 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/rob.png
--rw-r--r--   0 root         (0) root         (0)    76220 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/rr_advanced.png
--rw-r--r--   0 root         (0) root         (0)    55473 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/rr_beginner.png
--rw-r--r--   0 root         (0) root         (0)    90538 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/rr_intermediate.png
--rw-r--r--   0 root         (0) root         (0)     2148 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/sadface.png
--rw-r--r--   0 root         (0) root         (0)     6949 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/sharon_harrison.jpg
--rw-r--r--   0 root         (0) root         (0)   116116 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/sian.png
--rw-r--r--   0 root         (0) root         (0)    60671 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/teaching_resources_hero.jpg
--rw-r--r--   0 root         (0) root         (0)    68282 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_educate_kurono.png
--rw-r--r--   0 root         (0) root         (0)    67570 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_educate_rapid_router.png
--rw-r--r--   0 root         (0) root         (0)    37070 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_educate_resources.png
--rw-r--r--   0 root         (0) root         (0)    34617 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_intro_c4l.jpg
--rw-r--r--   0 root         (0) root         (0)    37516 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_kurono_resources.png
--rw-r--r--   0 root         (0) root         (0)    69758 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_play_kurono.png
--rw-r--r--   0 root         (0) root         (0)    20989 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_play_rapid_router.png
--rw-r--r--   0 root         (0) root         (0)    15969 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/twitter.png
--rw-r--r--   0 root         (0) root         (0)   145961 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/universities.png
--rw-r--r--   0 root         (0) root         (0)    54619 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/wes.png
--rw-r--r--   0 root         (0) root         (0)     1051 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/img/x_close_video.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.616796 codeforlife-portal-6.8.9/portal/static/portal/js/
--rw-r--r--   0 root         (0) root         (0)     3004 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/aimmoGame.js
--rw-r--r--   0 root         (0) root         (0)    39680 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/bootstrap.min.js
--rw-r--r--   0 root         (0) root         (0)      778 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/carouselCards.js
--rw-r--r--   0 root         (0) root         (0)     4293 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/common.js
--rw-r--r--   0 root         (0) root         (0)     1919 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/fuzzySchoolLookup.js
--rw-r--r--   0 root         (0) root         (0)      393 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/join_create_game_toggle.js
--rw-r--r--   0 root         (0) root         (0)     5297 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/jquery.placeholder.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.616796 codeforlife-portal-6.8.9/portal/static/portal/js/lib/
--rw-r--r--   0 root         (0) root         (0)    89476 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/lib/jquery-3.5.1.min.js
--rwxr-xr-x   0 root         (0) root         (0)    19519 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/lib/jquery-video-lightning.js
--rwxr-xr-x   0 root         (0) root         (0)    29200 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/lib/jquery.colorbox.js
--rw-r--r--   0 root         (0) root         (0)     4278 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/lib/jquery.easy-ticker.js
--rw-r--r--   0 root         (0) root         (0)    36698 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/lib/modernizr-build.js
--rw-r--r--   0 root         (0) root         (0)    18829 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/lib/papaparse.min.js
--rw-r--r--   0 root         (0) root         (0)     2662 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/organisation_manage.js
--rw-r--r--   0 root         (0) root         (0)     2876 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/passwordStrength.js
--rw-r--r--   0 root         (0) root         (0)     1363 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/play.js
--rw-r--r--   0 root         (0) root         (0)     7108 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/riveted.min.js
--rw-r--r--   0 root         (0) root         (0)      850 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/sticky_subnav.js
--rw-r--r--   0 root         (0) root         (0)     2437 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/teach_browser.js
--rw-r--r--   0 root         (0) root         (0)     4947 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/js/teach_class.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.616796 codeforlife-portal-6.8.9/portal/static/portal/sass/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.628796 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/
--rw-r--r--   0 root         (0) root         (0)     1546 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_alerts.scss
--rw-r--r--   0 root         (0) root         (0)     1228 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_badges.scss
--rw-r--r--   0 root         (0) root         (0)      700 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_breadcrumbs.scss
--rw-r--r--   0 root         (0) root         (0)     5764 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_button-groups.scss
--rw-r--r--   0 root         (0) root         (0)     3819 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_buttons.scss
--rw-r--r--   0 root         (0) root         (0)     5738 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_carousel.scss
--rw-r--r--   0 root         (0) root         (0)      835 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_close.scss
--rw-r--r--   0 root         (0) root         (0)     1403 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_code.scss
--rw-r--r--   0 root         (0) root         (0)      820 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_component-animations.scss
--rw-r--r--   0 root         (0) root         (0)     4847 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_dropdowns.scss
--rw-r--r--   0 root         (0) root         (0)    16102 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_forms.scss
--rw-r--r--   0 root         (0) root         (0)    20445 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_glyphicons.scss
--rw-r--r--   0 root         (0) root         (0)     1569 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_grid.scss
--rw-r--r--   0 root         (0) root         (0)     4310 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_input-groups.scss
--rw-r--r--   0 root         (0) root         (0)     1144 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_jumbotron.scss
--rw-r--r--   0 root         (0) root         (0)     1155 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_labels.scss
--rw-r--r--   0 root         (0) root         (0)     3151 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_list-group.scss
--rw-r--r--   0 root         (0) root         (0)      900 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_media.scss
--rw-r--r--   0 root         (0) root         (0)     1073 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_mixins.scss
--rw-r--r--   0 root         (0) root         (0)     3575 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_modals.scss
--rw-r--r--   0 root         (0) root         (0)    14652 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_navbar.scss
--rw-r--r--   0 root         (0) root         (0)     4953 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_navs.scss
--rw-r--r--   0 root         (0) root         (0)     7707 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_normalize.scss
--rw-r--r--   0 root         (0) root         (0)      855 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_pager.scss
--rw-r--r--   0 root         (0) root         (0)     2073 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_pagination.scss
--rw-r--r--   0 root         (0) root         (0)     6388 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_panels.scss
--rw-r--r--   0 root         (0) root         (0)     3476 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_popovers.scss
--rw-r--r--   0 root         (0) root         (0)     1682 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_print.scss
--rw-r--r--   0 root         (0) root         (0)     1998 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_progress-bars.scss
--rw-r--r--   0 root         (0) root         (0)      546 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_responsive-embed.scss
--rw-r--r--   0 root         (0) root         (0)     4421 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_responsive-utilities.scss
--rw-r--r--   0 root         (0) root         (0)     3046 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_scaffolding.scss
--rw-r--r--   0 root         (0) root         (0)     4662 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_tables.scss
--rw-r--r--   0 root         (0) root         (0)     8620 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_theme.scss
--rw-r--r--   0 root         (0) root         (0)      892 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_thumbnails.scss
--rw-r--r--   0 root         (0) root         (0)     3023 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_tooltip.scss
--rw-r--r--   0 root         (0) root         (0)     6062 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_type.scss
--rw-r--r--   0 root         (0) root         (0)      765 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_utilities.scss
--rw-r--r--   0 root         (0) root         (0)    30168 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_variables.scss
--rw-r--r--   0 root         (0) root         (0)      541 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_wells.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.632796 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/
--rw-r--r--   0 root         (0) root         (0)      264 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_alerts.scss
--rw-r--r--   0 root         (0) root         (0)      233 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_background-variant.scss
--rw-r--r--   0 root         (0) root         (0)      484 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_border-radius.scss
--rw-r--r--   0 root         (0) root         (0)     4469 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_breakpoints.scss
--rw-r--r--   0 root         (0) root         (0)     1375 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_buttons.scss
--rw-r--r--   0 root         (0) root         (0)      126 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_center-block.scss
--rw-r--r--   0 root         (0) root         (0)      611 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_clearfix.scss
--rw-r--r--   0 root         (0) root         (0)     2780 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_forms.scss
--rw-r--r--   0 root         (0) root         (0)     4381 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_gradients.scss
--rw-r--r--   0 root         (0) root         (0)     2359 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_grid-framework.scss
--rw-r--r--   0 root         (0) root         (0)     3210 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_grid.scss
--rw-r--r--   0 root         (0) root         (0)      590 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_hide-text.scss
--rw-r--r--   0 root         (0) root         (0)     1107 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_image.scss
--rw-r--r--   0 root         (0) root         (0)      167 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_labels.scss
--rw-r--r--   0 root         (0) root         (0)      672 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_list-group.scss
--rw-r--r--   0 root         (0) root         (0)      238 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_nav-divider.scss
--rw-r--r--   0 root         (0) root         (0)      370 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_nav-vertical-align.scss
--rw-r--r--   0 root         (0) root         (0)      148 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_opacity.scss
--rw-r--r--   0 root         (0) root         (0)      507 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_pagination.scss
--rw-r--r--   0 root         (0) root         (0)      543 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_panels.scss
--rw-r--r--   0 root         (0) root         (0)      200 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_progress-bar.scss
--rw-r--r--   0 root         (0) root         (0)      246 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_reset-filter.scss
--rw-r--r--   0 root         (0) root         (0)      473 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_reset-text.scss
--rw-r--r--   0 root         (0) root         (0)      202 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_resize.scss
--rw-r--r--   0 root         (0) root         (0)      417 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_responsive-visibility.scss
--rw-r--r--   0 root         (0) root         (0)      147 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_size.scss
--rw-r--r--   0 root         (0) root         (0)      338 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_tab-focus.scss
--rw-r--r--   0 root         (0) root         (0)      715 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_table-row.scss
--rw-r--r--   0 root         (0) root         (0)      210 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_text-emphasis.scss
--rw-r--r--   0 root         (0) root         (0)      168 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_text-overflow.scss
--rw-r--r--   0 root         (0) root         (0)      168 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_text-truncate.scss
--rw-r--r--   0 root         (0) root         (0)     6645 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_vendor-prefixes.scss
--rw-r--r--   0 root         (0) root         (0)     2144 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.636796 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_mixins/
--rw-r--r--   0 root         (0) root         (0)       87 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_mixins/_all.scss
--rw-r--r--   0 root         (0) root         (0)      722 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_mixins/_border-radius.scss
--rw-r--r--   0 root         (0) root         (0)       87 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_mixins/_box-shadow.scss
--rw-r--r--   0 root         (0) root         (0)      997 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_mixins/_hover.scss
--rw-r--r--   0 root         (0) root         (0)      220 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_mixins/_nav-divider.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.636796 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_partials/
--rw-r--r--   0 root         (0) root         (0)     3382 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_partials/_dropdown.scss
--rw-r--r--   0 root         (0) root         (0)    14283 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_partials/_glyphicons.scss
--rw-r--r--   0 root         (0) root         (0)     7859 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_partials/_grid.scss
--rw-r--r--   0 root         (0) root         (0)    32032 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_partials/_variables.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.636796 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/
--rw-r--r--   0 root         (0) root         (0)      373 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_align.scss
--rw-r--r--   0 root         (0) root         (0)      399 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_background.scss
--rw-r--r--   0 root         (0) root         (0)      677 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_borders.scss
--rw-r--r--   0 root         (0) root         (0)       37 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_clearfix.scss
--rw-r--r--   0 root         (0) root         (0)       50 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_cursor.scss
--rw-r--r--   0 root         (0) root         (0)     1153 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_display.scss
--rw-r--r--   0 root         (0) root         (0)     2533 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_flex.scss
--rw-r--r--   0 root         (0) root         (0)      320 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_float.scss
--rw-r--r--   0 root         (0) root         (0)      283 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_position.scss
--rw-r--r--   0 root         (0) root         (0)      115 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_screenreaders.scss
--rw-r--r--   0 root         (0) root         (0)      251 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_sizing.scss
--rw-r--r--   0 root         (0) root         (0)     1521 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_spacing.scss
--rw-r--r--   0 root         (0) root         (0)     1502 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_text.scss
--rw-r--r--   0 root         (0) root         (0)      121 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_visibility.scss
--rw-r--r--   0 root         (0) root         (0)     3790 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/colorbox.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.640796 codeforlife-portal-6.8.9/portal/static/portal/sass/modules/
--rw-r--r--   0 root         (0) root         (0)      174 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/modules/_all.scss
--rw-r--r--   0 root         (0) root         (0)       39 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/modules/_animation.scss
--rw-r--r--   0 root         (0) root         (0)      498 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/modules/_breakpoints.scss
--rw-r--r--   0 root         (0) root         (0)      107 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/modules/_card_constants.scss
--rw-r--r--   0 root         (0) root         (0)     4211 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/modules/_colours.scss
--rw-r--r--   0 root         (0) root         (0)       44 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/modules/_homepage_constants.scss
--rw-r--r--   0 root         (0) root         (0)      105 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/modules/_levels.scss
--rw-r--r--   0 root         (0) root         (0)     1493 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/modules/_mixins.scss
--rw-r--r--   0 root         (0) root         (0)       31 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/modules/_spacing.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.644796 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/
--rw-r--r--   0 root         (0) root         (0)     8787 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_banners.scss
--rw-r--r--   0 root         (0) root         (0)       26 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_base.scss
--rw-r--r--   0 root         (0) root         (0)     9002 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_buttons.scss
--rw-r--r--   0 root         (0) root         (0)     3238 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_carousel.scss
--rw-r--r--   0 root         (0) root         (0)     2445 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_footer.scss
--rw-r--r--   0 root         (0) root         (0)     6245 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_forms.scss
--rw-r--r--   0 root         (0) root         (0)     5866 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_grids.scss
--rw-r--r--   0 root         (0) root         (0)     7316 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_header.scss
--rw-r--r--   0 root         (0) root         (0)     3087 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_images.scss
--rw-r--r--   0 root         (0) root         (0)     2126 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_popup.scss
--rw-r--r--   0 root         (0) root         (0)      144 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_progress-bars.scss
--rw-r--r--   0 root         (0) root         (0)     5052 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_subnavs.scss
--rw-r--r--   0 root         (0) root         (0)     2978 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_tables.scss
--rw-r--r--   0 root         (0) root         (0)     3788 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_text.scss
--rw-r--r--   0 root         (0) root         (0)      956 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_ui-dialog.scss
--rw-r--r--   0 root         (0) root         (0)     3468 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_utils.scss
--rw-r--r--   0 root         (0) root         (0)      303 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_videos.scss
--rw-r--r--   0 root         (0) root         (0)      807 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/sass/styles.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.644796 codeforlife-portal-6.8.9/portal/static/portal/video/
--rw-r--r--   0 root         (0) root         (0)   999060 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/video/aimmo_play_now_background_video.mp4
--rw-r--r--   0 root         (0) root         (0)   277957 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/static/portal/video/code for life .pdf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.644796 codeforlife-portal-6.8.9/portal/strings/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/strings/__init__.py
--rw-r--r--   0 root         (0) root         (0)      644 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/strings/about.py
--rw-r--r--   0 root         (0) root         (0)      386 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/strings/help_and_support.py
--rw-r--r--   0 root         (0) root         (0)      273 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/strings/home_learning.py
--rw-r--r--   0 root         (0) root         (0)      274 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/strings/materials.py
--rw-r--r--   0 root         (0) root         (0)      804 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/strings/play.py
--rw-r--r--   0 root         (0) root         (0)      235 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/strings/student_aimmo_dashboard.py
--rw-r--r--   0 root         (0) root         (0)      257 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/strings/teach.py
--rw-r--r--   0 root         (0) root         (0)      760 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/strings/teacher_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.648796 codeforlife-portal-6.8.9/portal/templates/
--rw-r--r--   0 root         (0) root         (0)     1169 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/403.html
--rw-r--r--   0 root         (0) root         (0)      563 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/404.html
--rw-r--r--   0 root         (0) root         (0)     1703 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.648796 codeforlife-portal-6.8.9/portal/templates/captcha/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.648796 codeforlife-portal-6.8.9/portal/templates/captcha/includes/
--rw-r--r--   0 root         (0) root         (0)     1409 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/captcha/includes/js_v2_invisible.html
--rw-r--r--   0 root         (0) root         (0)      306 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/captcha/widget_v2_invisible.html
--rw-r--r--   0 root         (0) root         (0)      268 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/email.html
--rw-r--r--   0 root         (0) root         (0)       19 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/email.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.652796 codeforlife-portal-6.8.9/portal/templates/portal/
--rw-r--r--   0 root         (0) root         (0)     9902 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/about.html
--rw-r--r--   0 root         (0) root         (0)     9060 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/base.html
--rw-r--r--   0 root         (0) root         (0)      447 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/base_no_userprofile.html
--rw-r--r--   0 root         (0) root         (0)     4001 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/contribute.html
--rw-r--r--   0 root         (0) root         (0)      918 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/dotmailer_consent_form.html
--rw-r--r--   0 root         (0) root         (0)      641 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/email_invitation_sent.html
--rw-r--r--   0 root         (0) root         (0)    11935 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/email_style_template.html
--rw-r--r--   0 root         (0) root         (0)      806 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/email_verification_failed.html
--rw-r--r--   0 root         (0) root         (0)     1000 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/email_verification_needed.html
--rw-r--r--   0 root         (0) root         (0)     1223 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/form_shapes.html
--rw-r--r--   0 root         (0) root         (0)     2921 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/getinvolved.html
--rw-r--r--   0 root         (0) root         (0)     5342 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/home.html
--rw-r--r--   0 root         (0) root         (0)     9707 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/home_learning.html
--rw-r--r--   0 root         (0) root         (0)      894 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/locked_out.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.652796 codeforlife-portal-6.8.9/portal/templates/portal/login/
--rw-r--r--   0 root         (0) root         (0)     1523 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/login/independent_student.html
--rw-r--r--   0 root         (0) root         (0)     1011 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/login/student.html
--rw-r--r--   0 root         (0) root         (0)      966 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/login/student_class_code.html
--rw-r--r--   0 root         (0) root         (0)     2400 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/login/teacher.html
--rw-r--r--   0 root         (0) root         (0)      361 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/mouseflow.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.656796 codeforlife-portal-6.8.9/portal/templates/portal/partials/
--rw-r--r--   0 root         (0) root         (0)     4277 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/aimmo_games_table.html
--rw-r--r--   0 root         (0) root         (0)     1235 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/banner.html
--rw-r--r--   0 root         (0) root         (0)     2363 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/benefits.html
--rw-r--r--   0 root         (0) root         (0)     1550 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/card_list.html
--rw-r--r--   0 root         (0) root         (0)      415 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/character_list.html
--rw-r--r--   0 root         (0) root         (0)     1275 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/delete_popup.html
--rw-r--r--   0 root         (0) root         (0)     3652 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/footer.html
--rw-r--r--   0 root         (0) root         (0)    19148 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/header.html
--rw-r--r--   0 root         (0) root         (0)       89 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/headline.html
--rw-r--r--   0 root         (0) root         (0)      786 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/hero_card.html
--rw-r--r--   0 root         (0) root         (0)      566 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/info_popup.html
--rw-r--r--   0 root         (0) root         (0)      875 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/popup.html
--rw-r--r--   0 root         (0) root         (0)      329 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/register_newsletter_tickbox.html
--rw-r--r--   0 root         (0) root         (0)      311 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/register_over_required_age_tickbox.html
--rw-r--r--   0 root         (0) root         (0)      671 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/teacher_non_dashboard_subnav.html
--rw-r--r--   0 root         (0) root         (0)      671 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/partials/teacher_non_dashboard_subnav_account.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.660796 codeforlife-portal-6.8.9/portal/templates/portal/play/
--rw-r--r--   0 root         (0) root         (0)     2907 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/play/independent_student_dashboard.html
--rw-r--r--   0 root         (0) root         (0)     1403 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/play/student_aimmo_dashboard.html
--rw-r--r--   0 root         (0) root         (0)     3898 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/play/student_dashboard.html
--rw-r--r--   0 root         (0) root         (0)     6413 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/play/student_edit_account.html
--rw-r--r--   0 root         (0) root         (0)     2980 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/play/student_join_organisation.html
--rw-r--r--   0 root         (0) root         (0)     5162 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/play.html
--rw-r--r--   0 root         (0) root         (0)    33849 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/privacy_policy.html
--rw-r--r--   0 root         (0) root         (0)     7916 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/register.html
--rw-r--r--   0 root         (0) root         (0)     1373 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/reset_password.html
--rw-r--r--   0 root         (0) root         (0)     3041 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/reset_password_confirm.html
--rw-r--r--   0 root         (0) root         (0)      667 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/reset_password_done.html
--rw-r--r--   0 root         (0) root         (0)      748 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/reset_password_email_sent.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.660796 codeforlife-portal-6.8.9/portal/templates/portal/tag_manager/
--rw-r--r--   0 root         (0) root         (0)      661 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/tag_manager/tag_manager_body.html
--rw-r--r--   0 root         (0) root         (0)     1288 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/tag_manager/tag_manager_head.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.664796 codeforlife-portal-6.8.9/portal/templates/portal/teach/
--rw-r--r--   0 root         (0) root         (0)      582 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/base_registering.html
--rw-r--r--   0 root         (0) root         (0)     6997 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/class.html
--rw-r--r--   0 root         (0) root         (0)    29188 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/dashboard.html
--rw-r--r--   0 root         (0) root         (0)     1070 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/invite.html
--rw-r--r--   0 root         (0) root         (0)     2804 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/onboarding_classes.html
--rw-r--r--   0 root         (0) root         (0)     8862 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/onboarding_print.html
--rw-r--r--   0 root         (0) root         (0)     7768 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/onboarding_school.html
--rw-r--r--   0 root         (0) root         (0)     2399 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/onboarding_students.html
--rw-r--r--   0 root         (0) root         (0)     2453 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_add_external_student.html
--rw-r--r--   0 root         (0) root         (0)     1189 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_added_external_student.html
--rw-r--r--   0 root         (0) root         (0)     4427 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_aimmo_dashboard.html
--rw-r--r--   0 root         (0) root         (0)     4283 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_dismiss_students.html
--rw-r--r--   0 root         (0) root         (0)     4604 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_edit_class.html
--rw-r--r--   0 root         (0) root         (0)     2746 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_edit_student.html
--rw-r--r--   0 root         (0) root         (0)     1780 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_move_all_classes.html
--rw-r--r--   0 root         (0) root         (0)     1591 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_move_students.html
--rw-r--r--   0 root         (0) root         (0)     3348 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_move_students_to_class.html
--rw-r--r--   0 root         (0) root         (0)     2646 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_resources.html
--rw-r--r--   0 root         (0) root         (0)     8724 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/teach.html
--rw-r--r--   0 root         (0) root         (0)    19856 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/portal/terms.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.664796 codeforlife-portal-6.8.9/portal/templates/two_factor/
--rw-r--r--   0 root         (0) root         (0)      443 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/_base.html
--rw-r--r--   0 root         (0) root         (0)      355 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/_wizard_actions.html
--rw-r--r--   0 root         (0) root         (0)      358 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/_wizard_actions_enable_2fa.html
--rw-r--r--   0 root         (0) root         (0)      357 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/_wizard_actions_submit.html
--rw-r--r--   0 root         (0) root         (0)      267 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/_wizard_forms.html
--rw-r--r--   0 root         (0) root         (0)      262 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/_wizard_forms_token.html
--rw-r--r--   0 root         (0) root         (0)      262 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/backup_token.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.668796 codeforlife-portal-6.8.9/portal/templates/two_factor/core/
--rw-r--r--   0 root         (0) root         (0)     1442 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0 root         (0) root         (0)     2723 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/core/login.html
--rw-r--r--   0 root         (0) root         (0)     3145 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/core/setup.html
--rw-r--r--   0 root         (0) root         (0)      600 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/core/setup_complete.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.668796 codeforlife-portal-6.8.9/portal/templates/two_factor/profile/
--rw-r--r--   0 root         (0) root         (0)     1010 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/profile/disable.html
--rw-r--r--   0 root         (0) root         (0)     1800 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/profile/profile.html
--rw-r--r--   0 root         (0) root         (0)      266 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templates/two_factor/setup_wizard_token.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.668796 codeforlife-portal-6.8.9/portal/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4637 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templatetags/app_tags.py
--rw-r--r--   0 root         (0) root         (0)      823 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templatetags/banner_tags.py
--rw-r--r--   0 root         (0) root         (0)     1509 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templatetags/benefits_tags.py
--rw-r--r--   0 root         (0) root         (0)      509 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templatetags/card_list_tags.py
--rw-r--r--   0 root         (0) root         (0)      552 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templatetags/character_list_tags.py
--rw-r--r--   0 root         (0) root         (0)      165 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templatetags/future.py
--rw-r--r--   0 root         (0) root         (0)      420 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templatetags/headline_tags.py
--rw-r--r--   0 root         (0) root         (0)      939 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templatetags/hero_card_tags.py
--rw-r--r--   0 root         (0) root         (0)      448 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/templatetags/table_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.676796 codeforlife-portal-6.8.9/portal/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1716 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/base_test.py
--rw-r--r--   0 root         (0) root         (0)     1726 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.676796 codeforlife-portal-6.8.9/portal/tests/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2617 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_make_portaladmin_teacher.py
--rw-r--r--   0 root         (0) root         (0)      555 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_preview_user_remove.py
--rw-r--r--   0 root         (0) root         (0)      639 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_preview_users.py
--rw-r--r--   0 root         (0) root         (0)      391 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_remove_front_page_news.py
--rw-r--r--   0 root         (0) root         (0)      403 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_remove_guardian.py
--rw-r--r--   0 root         (0) root         (0)     1045 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_use_common_models.py
--rw-r--r--   0 root         (0) root         (0)     1089 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_verify_portaladmin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.676796 codeforlife-portal-6.8.9/portal/tests/pageObjects/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.680796 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.684796 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/admin/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/admin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      352 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/admin/admin_base_page.py
--rw-r--r--   0 root         (0) root         (0)      289 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/admin/admin_data_page.py
--rw-r--r--   0 root         (0) root         (0)      286 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/admin/admin_map_page.py
--rw-r--r--   0 root         (0) root         (0)     4780 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/base_page.py
--rw-r--r--   0 root         (0) root         (0)      458 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/email_verification_needed_page.py
--rw-r--r--   0 root         (0) root         (0)      235 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/forbidden_page.py
--rw-r--r--   0 root         (0) root         (0)     3672 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/game_page.py
--rw-r--r--   0 root         (0) root         (0)     1715 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/home_page.py
--rw-r--r--   0 root         (0) root         (0)     1352 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/independent_login_page.py
--rw-r--r--   0 root         (0) root         (0)     1419 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/kurono_teacher_dashboard_page.py
--rw-r--r--   0 root         (0) root         (0)     1106 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/password_reset_form_page.py
--rw-r--r--   0 root         (0) root         (0)      666 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/password_reset_page.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.684796 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/play/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/play/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3113 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/play/account_page.py
--rw-r--r--   0 root         (0) root         (0)      552 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/play/dashboard_page.py
--rw-r--r--   0 root         (0) root         (0)     1255 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/play/join_school_or_club_page.py
--rw-r--r--   0 root         (0) root         (0)      840 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/play/play_base_page.py
--rw-r--r--   0 root         (0) root         (0)      231 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/play_page.py
--rw-r--r--   0 root         (0) root         (0)      246 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/resources_page.py
--rw-r--r--   0 root         (0) root         (0)     2226 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/signup_page.py
--rw-r--r--   0 root         (0) root         (0)     1059 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/student_login_class_code.py
--rw-r--r--   0 root         (0) root         (0)     1012 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/student_login_page.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.688796 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/__init__.py
--rw-r--r--   0 root         (0) root         (0)      928 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/add_independent_student_to_class_page.py
--rw-r--r--   0 root         (0) root         (0)      539 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/added_independent_student_to_class_page.py
--rw-r--r--   0 root         (0) root         (0)     3943 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/class_page.py
--rw-r--r--   0 root         (0) root         (0)     7450 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/dashboard_page.py
--rw-r--r--   0 root         (0) root         (0)      833 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/dismiss_students_page.py
--rw-r--r--   0 root         (0) root         (0)     1346 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/edit_student_page.py
--rw-r--r--   0 root         (0) root         (0)     1057 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/move_class_page.py
--rw-r--r--   0 root         (0) root         (0)      836 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/move_classes_page.py
--rw-r--r--   0 root         (0) root         (0)      626 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/move_students_disambiguate_page.py
--rw-r--r--   0 root         (0) root         (0)     1125 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/move_students_page.py
--rw-r--r--   0 root         (0) root         (0)      998 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/onboarding_classes_page.py
--rw-r--r--   0 root         (0) root         (0)     2958 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/onboarding_organisation_page.py
--rw-r--r--   0 root         (0) root         (0)      815 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/onboarding_revoke_request_page.py
--rw-r--r--   0 root         (0) root         (0)     1185 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/onboarding_student_list_page.py
--rw-r--r--   0 root         (0) root         (0)      924 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/onboarding_students_page.py
--rw-r--r--   0 root         (0) root         (0)     1180 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/teach_base_page.py
--rw-r--r--   0 root         (0) root         (0)     1922 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teacher_login_page.py
--rw-r--r--   0 root         (0) root         (0)      469 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/selenium_test_case.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.688796 codeforlife-portal-6.8.9/portal/tests/snapshots/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/snapshots/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8572 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/snapshots/snap_test_partials.py
--rw-r--r--   0 root         (0) root         (0)     3846 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_2FA.py
--rw-r--r--   0 root         (0) root         (0)     1229 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_admin.py
--rw-r--r--   0 root         (0) root         (0)     5355 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_aimmo_dashboards.py
--rw-r--r--   0 root         (0) root         (0)    10772 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     1015 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_captcha_forms.py
--rw-r--r--   0 root         (0) root         (0)     7522 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_class.py
--rw-r--r--   0 root         (0) root         (0)     9654 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_emails.py
--rw-r--r--   0 root         (0) root         (0)    19336 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_independent_student.py
--rw-r--r--   0 root         (0) root         (0)      711 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_invite_teacher.py
--rw-r--r--   0 root         (0) root         (0)     5477 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_middleware.py
--rw-r--r--   0 root         (0) root         (0)      838 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_newsletter_footer.py
--rw-r--r--   0 root         (0) root         (0)    14140 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_organisation.py
--rw-r--r--   0 root         (0) root         (0)     4030 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_partials.py
--rw-r--r--   0 root         (0) root         (0)    12639 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_ratelimit.py
--rw-r--r--   0 root         (0) root         (0)      856 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_react_test_space.py
--rw-r--r--   0 root         (0) root         (0)     7965 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_school_student.py
--rw-r--r--   0 root         (0) root         (0)     3761 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_security.py
--rw-r--r--   0 root         (0) root         (0)    29040 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_teacher.py
--rw-r--r--   0 root         (0) root         (0)    21448 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_teacher_student.py
--rw-r--r--   0 root         (0) root         (0)    26171 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/test_views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.688796 codeforlife-portal-6.8.9/portal/tests/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      649 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/utils/aimmo_games.py
--rw-r--r--   0 root         (0) root         (0)      183 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/utils/classes.py
--rw-r--r--   0 root         (0) root         (0)     1852 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/tests/utils/messages.py
--rw-r--r--   0 root         (0) root         (0)    15571 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.692796 codeforlife-portal-6.8.9/portal/views/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)      443 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/about.py
--rw-r--r--   0 root         (0) root         (0)      957 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.692796 codeforlife-portal-6.8.9/portal/views/aimmo/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/aimmo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3877 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/aimmo/dashboard.py
--rw-r--r--   0 root         (0) root         (0)     6326 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/api.py
--rw-r--r--   0 root         (0) root         (0)     2299 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/dotmailer.py
--rw-r--r--   0 root         (0) root         (0)     3798 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/email.py
--rw-r--r--   0 root         (0) root         (0)     8400 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/home.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.692796 codeforlife-portal-6.8.9/portal/views/login/
--rw-r--r--   0 root         (0) root         (0)      399 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/login/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2662 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/login/independent_student.py
--rw-r--r--   0 root         (0) root         (0)     3720 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/login/student.py
--rw-r--r--   0 root         (0) root         (0)     1997 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/login/teacher.py
--rw-r--r--   0 root         (0) root         (0)     8123 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/organisation.py
--rw-r--r--   0 root         (0) root         (0)      308 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/play_landing_page.py
--rw-r--r--   0 root         (0) root         (0)      195 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/privacy_policy.py
--rw-r--r--   0 root         (0) root         (0)     8644 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/registration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.696796 codeforlife-portal-6.8.9/portal/views/student/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/student/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9315 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/student/edit_account_details.py
--rw-r--r--   0 root         (0) root         (0)     8362 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/student/play.py
--rw-r--r--   0 root         (0) root         (0)      210 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/teach.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.696796 codeforlife-portal-6.8.9/portal/views/teacher/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/teacher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18315 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/teacher/dashboard.py
--rw-r--r--   0 root         (0) root         (0)    32106 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/teacher/teach.py
--rw-r--r--   0 root         (0) root         (0)     1513 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/teacher/teacher_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 09:04:13.696796 codeforlife-portal-6.8.9/portal/views/two_factor/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/two_factor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/two_factor/core.py
--rw-r--r--   0 root         (0) root         (0)      257 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/two_factor/form.py
--rw-r--r--   0 root         (0) root         (0)      383 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/views/two_factor/profile.py
--rw-r--r--   0 root         (0) root         (0)      401 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/portal/wsgi.py
--rw-r--r--   0 root         (0) root         (0)      133 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      199 2022-06-21 09:04:13.696796 codeforlife-portal-6.8.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1543 2022-06-21 09:00:15.000000 codeforlife-portal-6.8.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.018178 codeforlife-portal-6.9.0/
+-rw-r--r--   0 root         (0) root         (0)    38929 2022-06-23 09:37:43.000000 codeforlife-portal-6.9.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      165 2022-06-23 09:37:43.000000 codeforlife-portal-6.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      293 2022-06-23 09:40:37.018178 codeforlife-portal-6.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1256 2022-06-23 09:37:43.000000 codeforlife-portal-6.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.930178 codeforlife-portal-6.9.0/codeforlife_portal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      293 2022-06-23 09:40:36.000000 codeforlife-portal-6.9.0/codeforlife_portal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25628 2022-06-23 09:40:36.000000 codeforlife-portal-6.9.0/codeforlife_portal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-23 09:40:36.000000 codeforlife-portal-6.9.0/codeforlife_portal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-23 09:38:11.000000 codeforlife-portal-6.9.0/codeforlife_portal.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      505 2022-06-23 09:40:36.000000 codeforlife-portal-6.9.0/codeforlife_portal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2022-06-23 09:40:36.000000 codeforlife-portal-6.9.0/codeforlife_portal.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.930178 codeforlife-portal-6.9.0/deploy/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/captcha.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.930178 codeforlife-portal-6.9.0/deploy/middleware/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/middleware/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/middleware/admin_access.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/middleware/basicauth.py
+-rw-r--r--   0 root         (0) root         (0)      474 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/middleware/exceptionlogging.py
+-rw-r--r--   0 root         (0) root         (0)      751 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/middleware/security.py
+-rw-r--r--   0 root         (0) root         (0)      881 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/middleware/session_timeout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.930178 codeforlife-portal-6.9.0/deploy/static/
+-rw-r--r--   0 root         (0) root         (0)    24583 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/static/apple-touch-icon-120x120.png
+-rw-r--r--   0 root         (0) root         (0)    36276 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/static/apple-touch-icon-152x152.png
+-rw-r--r--   0 root         (0) root         (0)    47948 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/static/apple-touch-icon-180x180.png
+-rw-r--r--   0 root         (0) root         (0)    11676 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/static/apple-touch-icon-76x76.png
+-rw-r--r--   0 root         (0) root         (0)     7842 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/static/apple-touch-icon.png
+-rw-r--r--   0 root         (0) root         (0)       24 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/static/robots.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.918178 codeforlife-portal-6.9.0/deploy/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.930178 codeforlife-portal-6.9.0/deploy/templates/deploy/
+-rw-r--r--   0 root         (0) root         (0)      412 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/templates/deploy/csrf_failure.html
+-rw-r--r--   0 root         (0) root         (0)      131 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/deploy/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.934178 codeforlife-portal-6.9.0/portal/
+-rw-r--r--   0 root         (0) root         (0)       22 2022-06-23 09:40:32.000000 codeforlife-portal-6.9.0/portal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/admin.py
+-rw-r--r--   0 root         (0) root         (0)      606 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5241 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/autoconfig.py
+-rw-r--r--   0 root         (0) root         (0)      812 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/backends.py
+-rw-r--r--   0 root         (0) root         (0)      255 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/beta.py
+-rw-r--r--   0 root         (0) root         (0)      133 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/context_processors.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/csp_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.934178 codeforlife-portal-6.9.0/portal/forms/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/forms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/forms/add_game.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/forms/admin.py
+-rw-r--r--   0 root         (0) root         (0)      761 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/forms/dotmailer.py
+-rw-r--r--   0 root         (0) root         (0)      148 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/forms/error_messages.py
+-rw-r--r--   0 root         (0) root         (0)      430 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/forms/invite_teacher.py
+-rw-r--r--   0 root         (0) root         (0)     3519 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/forms/organisation.py
+-rw-r--r--   0 root         (0) root         (0)    10722 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/forms/play.py
+-rw-r--r--   0 root         (0) root         (0)     5928 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/forms/registration.py
+-rw-r--r--   0 root         (0) root         (0)    19219 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/forms/teach.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.934178 codeforlife-portal-6.9.0/portal/frontend/
+-rw-r--r--   0 root         (0) root         (0)      993 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/asset-manifest.json
+-rw-r--r--   0 root         (0) root         (0)      481 2022-06-23 09:40:07.000000 codeforlife-portal-6.9.0/portal/frontend/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     1003 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/index.html
+-rw-r--r--   0 root         (0) root         (0)      492 2022-06-23 09:40:07.000000 codeforlife-portal-6.9.0/portal/frontend/manifest.json
+-rw-r--r--   0 root         (0) root         (0)       40 2022-06-23 09:40:07.000000 codeforlife-portal-6.9.0/portal/frontend/portal.css
+-rw-r--r--   0 root         (0) root         (0)       67 2022-06-23 09:40:07.000000 codeforlife-portal-6.9.0/portal/frontend/robots.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.918178 codeforlife-portal-6.9.0/portal/frontend/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.934178 codeforlife-portal-6.9.0/portal/frontend/static/css/
+-rw-r--r--   0 root         (0) root         (0)       73 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/css/main.acb3d7db.css
+-rw-r--r--   0 root         (0) root         (0)      207 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/css/main.acb3d7db.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.938178 codeforlife-portal-6.9.0/portal/frontend/static/js/
+-rw-r--r--   0 root         (0) root         (0)     4597 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/js/787.cda612ba.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    10281 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/js/787.cda612ba.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)   345455 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/js/main.8c02947d.js
+-rw-r--r--   0 root         (0) root         (0)     1694 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/js/main.8c02947d.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  1283202 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/js/main.8c02947d.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.938178 codeforlife-portal-6.9.0/portal/frontend/static/media/
+-rw-r--r--   0 root         (0) root         (0)      524 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/media/facebook.2bdba6ecdf25da4a6d91d9df9e3f5830.svg
+-rw-r--r--   0 root         (0) root         (0)    16839 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/media/logo_cfl.06fffc34beb6c215ab01.png
+-rw-r--r--   0 root         (0) root         (0)     5451 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/media/logo_ocado_group.bf2daf768df6901d40924159853b612d.svg
+-rw-r--r--   0 root         (0) root         (0)    10993 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/media/ocado.5e7ae9a2adbc50ec6f96f3f6366eea25.svg
+-rw-r--r--   0 root         (0) root         (0)      896 2022-06-23 09:40:31.000000 codeforlife-portal-6.9.0/portal/frontend/static/media/twitter.3f190a3549dea2464ca62924d629b961.svg
+-rw-r--r--   0 root         (0) root         (0)      422 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.938178 codeforlife-portal-6.9.0/portal/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      254 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/helpers/captcha.py
+-rw-r--r--   0 root         (0) root         (0)     2560 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/helpers/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     3483 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/helpers/password.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/helpers/ratelimit.py
+-rw-r--r--   0 root         (0) root         (0)      125 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/helpers/regexes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.942178 codeforlife-portal-6.9.0/portal/migrations/
+-rw-r--r--   0 root         (0) root         (0)    29559 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0001_squashed_0041_new_news.py
+-rw-r--r--   0 root         (0) root         (0)      423 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0042_school_country.py
+-rw-r--r--   0 root         (0) root         (0)      461 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0043_auto_20150430_0952.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0044_auto_20150430_0959.py
+-rw-r--r--   0 root         (0) root         (0)      412 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0045_auto_20150430_1446.py
+-rw-r--r--   0 root         (0) root         (0)      540 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0046_auto_20150723_1101.py
+-rw-r--r--   0 root         (0) root         (0)      267 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0047_remove_userprofile_avatar.py
+-rw-r--r--   0 root         (0) root         (0)      349 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0048_plural_management_frontnews.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0049_refactor_emailverifications.py
+-rw-r--r--   0 root         (0) root         (0)      876 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0050_refactor_emailverifications_2.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0051_add_missing_ev_records.py
+-rw-r--r--   0 root         (0) root         (0)      284 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0052_refactor_emailverifications_3.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0053_refactor_teacher_student_1.py
+-rw-r--r--   0 root         (0) root         (0)      564 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0054_pending_join_request_can_be_blank.py
+-rw-r--r--   0 root         (0) root         (0)      557 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0055_add_preview_user.py
+-rw-r--r--   0 root         (0) root         (0)      409 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0056_remove_preview_user.py
+-rw-r--r--   0 root         (0) root         (0)      291 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0057_delete_frontpagenews.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0058_move_to_common_models.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0059_move_email_verifications_to_common.py
+-rw-r--r--   0 root         (0) root         (0)      627 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0060_delete_guardian.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0061_make_portaladmin_teacher.py
+-rw-r--r--   0 root         (0) root         (0)     1306 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/0062_verify_portaladmin.py
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.942178 codeforlife-portal-6.9.0/portal/pipeline_compilers/
+-rw-r--r--   0 root         (0) root         (0)       85 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/pipeline_compilers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      742 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/pipeline_compilers/libsass_compiler.py
+-rw-r--r--   0 root         (0) root         (0)      227 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/reactTestSpace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.922178 codeforlife-portal-6.9.0/portal/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.922178 codeforlife-portal-6.9.0/portal/static/portal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.922178 codeforlife-portal-6.9.0/portal/static/portal/fonts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.942178 codeforlife-portal-6.9.0/portal/static/portal/fonts/bootstrap/
+-rw-r--r--   0 root         (0) root         (0)    20127 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.eot
+-rw-r--r--   0 root         (0) root         (0)   108738 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.svg
+-rw-r--r--   0 root         (0) root         (0)    45404 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 root         (0) root         (0)    23424 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.woff
+-rw-r--r--   0 root         (0) root         (0)    18028 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.962178 codeforlife-portal-6.9.0/portal/static/portal/img/
+-rw-r--r--   0 root         (0) root         (0)     3329 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/10x_logo.png
+-rw-r--r--   0 root         (0) root         (0)    64472 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/RR_logo_grass_background.png
+-rw-r--r--   0 root         (0) root         (0)  1177416 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/RR_logo_green.svg
+-rw-r--r--   0 root         (0) root         (0)     8799 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/RR_logo_simple.png
+-rw-r--r--   0 root         (0) root         (0)   140736 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/about_us_cfl.jpg
+-rw-r--r--   0 root         (0) root         (0)    19287 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/about_us_hero.jpg
+-rw-r--r--   0 root         (0) root         (0)   118428 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/about_us_ocado.jpg
+-rw-r--r--   0 root         (0) root         (0)     9038 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/barefoot_logo.png
+-rw-r--r--   0 root         (0) root         (0)     7562 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/bcs_logo.png
+-rw-r--r--   0 root         (0) root         (0)   159021 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/clubs.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.962178 codeforlife-portal-6.9.0/portal/static/portal/img/colorboxImages/
+-rwxr-xr-x   0 root         (0) root         (0)      112 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/colorboxImages/border.png
+-rwxr-xr-x   0 root         (0) root         (0)     2893 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/colorboxImages/controls.png
+-rwxr-xr-x   0 root         (0) root         (0)     9427 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/colorboxImages/loading.gif
+-rwxr-xr-x   0 root         (0) root         (0)      157 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/colorboxImages/loading_background.png
+-rwxr-xr-x   0 root         (0) root         (0)      182 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/colorboxImages/overlay.png
+-rw-r--r--   0 root         (0) root         (0)     3723 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/confirmation_tick.png
+-rw-r--r--   0 root         (0) root         (0)     1143 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/cross.png
+-rw-r--r--   0 root         (0) root         (0)    45387 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/dee.png
+-rw-r--r--   0 root         (0) root         (0)     6543 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/facebook.png
+-rw-r--r--   0 root         (0) root         (0)      481 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   176315 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/get_involved_hero.png
+-rw-r--r--   0 root         (0) root         (0)   177664 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/gitbook.png
+-rw-r--r--   0 root         (0) root         (0)    62646 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/gitbook_space.png
+-rw-r--r--   0 root         (0) root         (0)    63596 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/github.png
+-rw-r--r--   0 root         (0) root         (0)    47014 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/github_hero.png
+-rw-r--r--   0 root         (0) root         (0)     4387 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/gla_logo.png
+-rw-r--r--   0 root         (0) root         (0)     1133 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/hamburger.png
+-rw-r--r--   0 root         (0) root         (0)    47601 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/help_and_support_hero.jpg
+-rw-r--r--   0 root         (0) root         (0)   194269 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/home_educate.png
+-rw-r--r--   0 root         (0) root         (0)    88389 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/home_educate_hero.jpg
+-rw-r--r--   0 root         (0) root         (0)    62414 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/home_learning_hero.jpg
+-rw-r--r--   0 root         (0) root         (0)   191553 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/home_play.png
+-rw-r--r--   0 root         (0) root         (0)   110397 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/home_play_hero.jpg
+-rw-r--r--   0 root         (0) root         (0)     7967 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/hope_logo.png
+-rw-r--r--   0 root         (0) root         (0)     3260 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/icl_logo.png
+-rw-r--r--   0 root         (0) root         (0)     5948 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/icon_controller.png
+-rw-r--r--   0 root         (0) root         (0)    19299 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/icon_free.png
+-rw-r--r--   0 root         (0) root         (0)     6044 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/icon_globe.png
+-rw-r--r--   0 root         (0) root         (0)     2636 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/icon_piechart.png
+-rw-r--r--   0 root         (0) root         (0)     5006 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/icon_step_by_step.png
+-rw-r--r--   0 root         (0) root         (0)      761 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/icon_tracking.png
+-rw-r--r--   0 root         (0) root         (0)     6052 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/icon_uk_flag.png
+-rw-r--r--   0 root         (0) root         (0)    31240 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/kirsty.png
+-rw-r--r--   0 root         (0) root         (0)    80736 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/kurono_hero.jpg
+-rw-r--r--   0 root         (0) root         (0)   254014 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/kurono_landing_hero.png
+-rw-r--r--   0 root         (0) root         (0)     2930 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/kurono_logo.svg
+-rw-r--r--   0 root         (0) root         (0)     3017 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/kurono_logo_grey_background.svg
+-rw-r--r--   0 root         (0) root         (0)     1494 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/kurono_logo_mark.svg
+-rw-r--r--   0 root         (0) root         (0)   119585 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/kurono_resources_hero.jpg
+-rw-r--r--   0 root         (0) root         (0)   737438 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/kurono_story.png
+-rw-r--r--   0 root         (0) root         (0)    16839 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/logo_cfl.png
+-rw-r--r--   0 root         (0) root         (0)     8599 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/logo_cfl_reminder_cards.jpg
+-rw-r--r--   0 root         (0) root         (0)     4747 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/logo_cfl_white_landscape.png
+-rw-r--r--   0 root         (0) root         (0)     5232 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/logo_ocado.png
+-rw-r--r--   0 root         (0) root         (0)     2543 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/logo_ocado_group.png
+-rw-r--r--   0 root         (0) root         (0)     5451 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/logo_ocado_group.svg
+-rw-r--r--   0 root         (0) root         (0)    10993 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/logo_ocado_group_white.svg
+-rw-r--r--   0 root         (0) root         (0)     3095 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/mc_saatchi_logo.png
+-rw-r--r--   0 root         (0) root         (0)    49149 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/nigel.png
+-rw-r--r--   0 root         (0) root         (0)     2447 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/ocado-swirl.svg
+-rw-r--r--   0 root         (0) root         (0)      511 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/oval_blue.svg
+-rw-r--r--   0 root         (0) root         (0)      515 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/oval_pink.svg
+-rw-r--r--   0 root         (0) root         (0)      511 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/oval_yellow.svg
+-rw-r--r--   0 root         (0) root         (0)     2728 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/paper_plane.png
+-rw-r--r--   0 root         (0) root         (0)    60371 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/phil.png
+-rw-r--r--   0 root         (0) root         (0)      583 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/polygon_blue.svg
+-rw-r--r--   0 root         (0) root         (0)      579 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/polygon_pink.svg
+-rw-r--r--   0 root         (0) root         (0)      579 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/polygon_yellow.svg
+-rw-r--r--   0 root         (0) root         (0)     2876 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/pressure_cooker_logo.png
+-rw-r--r--   0 root         (0) root         (0)    77059 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/rapid_router.png
+-rw-r--r--   0 root         (0) root         (0)   146564 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/rapid_router_landing_hero.png
+-rw-r--r--   0 root         (0) root         (0)    36268 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/rapidrouter.png
+-rw-r--r--   0 root         (0) root         (0)    65998 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/resources_hero.jpg
+-rw-r--r--   0 root         (0) root         (0)    74159 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/resources_montage.jpg
+-rw-r--r--   0 root         (0) root         (0)    93064 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/reuben.png
+-rw-r--r--   0 root         (0) root         (0)   103324 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/rob.png
+-rw-r--r--   0 root         (0) root         (0)    76220 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/rr_advanced.png
+-rw-r--r--   0 root         (0) root         (0)    55473 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/rr_beginner.png
+-rw-r--r--   0 root         (0) root         (0)    90538 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/rr_intermediate.png
+-rw-r--r--   0 root         (0) root         (0)     2148 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/sadface.png
+-rw-r--r--   0 root         (0) root         (0)     6949 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/sharon_harrison.jpg
+-rw-r--r--   0 root         (0) root         (0)   116116 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/sian.png
+-rw-r--r--   0 root         (0) root         (0)    60671 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/teaching_resources_hero.jpg
+-rw-r--r--   0 root         (0) root         (0)    68282 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_educate_kurono.png
+-rw-r--r--   0 root         (0) root         (0)    67570 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_educate_rapid_router.png
+-rw-r--r--   0 root         (0) root         (0)    37070 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_educate_resources.png
+-rw-r--r--   0 root         (0) root         (0)    34617 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_intro_c4l.jpg
+-rw-r--r--   0 root         (0) root         (0)    37516 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_kurono_resources.png
+-rw-r--r--   0 root         (0) root         (0)    69758 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_play_kurono.png
+-rw-r--r--   0 root         (0) root         (0)    20989 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_play_rapid_router.png
+-rw-r--r--   0 root         (0) root         (0)    15969 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/twitter.png
+-rw-r--r--   0 root         (0) root         (0)   145961 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/universities.png
+-rw-r--r--   0 root         (0) root         (0)    54619 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/wes.png
+-rw-r--r--   0 root         (0) root         (0)     1051 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/img/x_close_video.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.966178 codeforlife-portal-6.9.0/portal/static/portal/js/
+-rw-r--r--   0 root         (0) root         (0)     3004 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/aimmoGame.js
+-rw-r--r--   0 root         (0) root         (0)    39680 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/bootstrap.min.js
+-rw-r--r--   0 root         (0) root         (0)      778 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/carouselCards.js
+-rw-r--r--   0 root         (0) root         (0)     4293 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/common.js
+-rw-r--r--   0 root         (0) root         (0)     1919 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/fuzzySchoolLookup.js
+-rw-r--r--   0 root         (0) root         (0)      393 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/join_create_game_toggle.js
+-rw-r--r--   0 root         (0) root         (0)     5297 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/jquery.placeholder.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.966178 codeforlife-portal-6.9.0/portal/static/portal/js/lib/
+-rw-r--r--   0 root         (0) root         (0)    89476 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/lib/jquery-3.5.1.min.js
+-rwxr-xr-x   0 root         (0) root         (0)    19519 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/lib/jquery-video-lightning.js
+-rwxr-xr-x   0 root         (0) root         (0)    29200 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/lib/jquery.colorbox.js
+-rw-r--r--   0 root         (0) root         (0)     4278 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/lib/jquery.easy-ticker.js
+-rw-r--r--   0 root         (0) root         (0)    36698 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/lib/modernizr-build.js
+-rw-r--r--   0 root         (0) root         (0)    18829 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/lib/papaparse.min.js
+-rw-r--r--   0 root         (0) root         (0)     2662 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/organisation_manage.js
+-rw-r--r--   0 root         (0) root         (0)     2876 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/passwordStrength.js
+-rw-r--r--   0 root         (0) root         (0)     1363 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/play.js
+-rw-r--r--   0 root         (0) root         (0)     7108 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/riveted.min.js
+-rw-r--r--   0 root         (0) root         (0)      850 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/sticky_subnav.js
+-rw-r--r--   0 root         (0) root         (0)     2437 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/teach_browser.js
+-rw-r--r--   0 root         (0) root         (0)     4947 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/js/teach_class.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.966178 codeforlife-portal-6.9.0/portal/static/portal/sass/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.974178 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/
+-rw-r--r--   0 root         (0) root         (0)     1546 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_alerts.scss
+-rw-r--r--   0 root         (0) root         (0)     1228 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_badges.scss
+-rw-r--r--   0 root         (0) root         (0)      700 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_breadcrumbs.scss
+-rw-r--r--   0 root         (0) root         (0)     5764 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_button-groups.scss
+-rw-r--r--   0 root         (0) root         (0)     3819 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_buttons.scss
+-rw-r--r--   0 root         (0) root         (0)     5738 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_carousel.scss
+-rw-r--r--   0 root         (0) root         (0)      835 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_close.scss
+-rw-r--r--   0 root         (0) root         (0)     1403 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_code.scss
+-rw-r--r--   0 root         (0) root         (0)      820 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_component-animations.scss
+-rw-r--r--   0 root         (0) root         (0)     4847 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_dropdowns.scss
+-rw-r--r--   0 root         (0) root         (0)    16102 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_forms.scss
+-rw-r--r--   0 root         (0) root         (0)    20445 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_glyphicons.scss
+-rw-r--r--   0 root         (0) root         (0)     1569 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_grid.scss
+-rw-r--r--   0 root         (0) root         (0)     4310 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_input-groups.scss
+-rw-r--r--   0 root         (0) root         (0)     1144 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_jumbotron.scss
+-rw-r--r--   0 root         (0) root         (0)     1155 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_labels.scss
+-rw-r--r--   0 root         (0) root         (0)     3151 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_list-group.scss
+-rw-r--r--   0 root         (0) root         (0)      900 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_media.scss
+-rw-r--r--   0 root         (0) root         (0)     1073 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_mixins.scss
+-rw-r--r--   0 root         (0) root         (0)     3575 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_modals.scss
+-rw-r--r--   0 root         (0) root         (0)    14652 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_navbar.scss
+-rw-r--r--   0 root         (0) root         (0)     4953 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_navs.scss
+-rw-r--r--   0 root         (0) root         (0)     7707 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_normalize.scss
+-rw-r--r--   0 root         (0) root         (0)      855 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_pager.scss
+-rw-r--r--   0 root         (0) root         (0)     2073 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_pagination.scss
+-rw-r--r--   0 root         (0) root         (0)     6388 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_panels.scss
+-rw-r--r--   0 root         (0) root         (0)     3476 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_popovers.scss
+-rw-r--r--   0 root         (0) root         (0)     1682 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_print.scss
+-rw-r--r--   0 root         (0) root         (0)     1998 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_progress-bars.scss
+-rw-r--r--   0 root         (0) root         (0)      546 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_responsive-embed.scss
+-rw-r--r--   0 root         (0) root         (0)     4421 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_responsive-utilities.scss
+-rw-r--r--   0 root         (0) root         (0)     3046 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_scaffolding.scss
+-rw-r--r--   0 root         (0) root         (0)     4662 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_tables.scss
+-rw-r--r--   0 root         (0) root         (0)     8620 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_theme.scss
+-rw-r--r--   0 root         (0) root         (0)      892 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_thumbnails.scss
+-rw-r--r--   0 root         (0) root         (0)     3023 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_tooltip.scss
+-rw-r--r--   0 root         (0) root         (0)     6062 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_type.scss
+-rw-r--r--   0 root         (0) root         (0)      765 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_utilities.scss
+-rw-r--r--   0 root         (0) root         (0)    30168 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_variables.scss
+-rw-r--r--   0 root         (0) root         (0)      541 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_wells.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.978178 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/
+-rw-r--r--   0 root         (0) root         (0)      264 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_alerts.scss
+-rw-r--r--   0 root         (0) root         (0)      233 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_background-variant.scss
+-rw-r--r--   0 root         (0) root         (0)      484 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_border-radius.scss
+-rw-r--r--   0 root         (0) root         (0)     4469 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_breakpoints.scss
+-rw-r--r--   0 root         (0) root         (0)     1375 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_buttons.scss
+-rw-r--r--   0 root         (0) root         (0)      126 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_center-block.scss
+-rw-r--r--   0 root         (0) root         (0)      611 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_clearfix.scss
+-rw-r--r--   0 root         (0) root         (0)     2780 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_forms.scss
+-rw-r--r--   0 root         (0) root         (0)     4381 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_gradients.scss
+-rw-r--r--   0 root         (0) root         (0)     2359 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_grid-framework.scss
+-rw-r--r--   0 root         (0) root         (0)     3210 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_grid.scss
+-rw-r--r--   0 root         (0) root         (0)      590 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_hide-text.scss
+-rw-r--r--   0 root         (0) root         (0)     1107 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_image.scss
+-rw-r--r--   0 root         (0) root         (0)      167 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_labels.scss
+-rw-r--r--   0 root         (0) root         (0)      672 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_list-group.scss
+-rw-r--r--   0 root         (0) root         (0)      238 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_nav-divider.scss
+-rw-r--r--   0 root         (0) root         (0)      370 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_nav-vertical-align.scss
+-rw-r--r--   0 root         (0) root         (0)      148 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_opacity.scss
+-rw-r--r--   0 root         (0) root         (0)      507 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_pagination.scss
+-rw-r--r--   0 root         (0) root         (0)      543 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_panels.scss
+-rw-r--r--   0 root         (0) root         (0)      200 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_progress-bar.scss
+-rw-r--r--   0 root         (0) root         (0)      246 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_reset-filter.scss
+-rw-r--r--   0 root         (0) root         (0)      473 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_reset-text.scss
+-rw-r--r--   0 root         (0) root         (0)      202 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_resize.scss
+-rw-r--r--   0 root         (0) root         (0)      417 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_responsive-visibility.scss
+-rw-r--r--   0 root         (0) root         (0)      147 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_size.scss
+-rw-r--r--   0 root         (0) root         (0)      338 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_tab-focus.scss
+-rw-r--r--   0 root         (0) root         (0)      715 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_table-row.scss
+-rw-r--r--   0 root         (0) root         (0)      210 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_text-emphasis.scss
+-rw-r--r--   0 root         (0) root         (0)      168 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_text-overflow.scss
+-rw-r--r--   0 root         (0) root         (0)      168 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_text-truncate.scss
+-rw-r--r--   0 root         (0) root         (0)     6645 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_vendor-prefixes.scss
+-rw-r--r--   0 root         (0) root         (0)     2144 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.978178 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_mixins/
+-rw-r--r--   0 root         (0) root         (0)       87 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_mixins/_all.scss
+-rw-r--r--   0 root         (0) root         (0)      722 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_mixins/_border-radius.scss
+-rw-r--r--   0 root         (0) root         (0)       87 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_mixins/_box-shadow.scss
+-rw-r--r--   0 root         (0) root         (0)      997 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_mixins/_hover.scss
+-rw-r--r--   0 root         (0) root         (0)      220 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_mixins/_nav-divider.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.978178 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_partials/
+-rw-r--r--   0 root         (0) root         (0)     3382 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_partials/_dropdown.scss
+-rw-r--r--   0 root         (0) root         (0)    14283 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_partials/_glyphicons.scss
+-rw-r--r--   0 root         (0) root         (0)     7859 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_partials/_grid.scss
+-rw-r--r--   0 root         (0) root         (0)    32032 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_partials/_variables.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.978178 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/
+-rw-r--r--   0 root         (0) root         (0)      373 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_align.scss
+-rw-r--r--   0 root         (0) root         (0)      399 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_background.scss
+-rw-r--r--   0 root         (0) root         (0)      677 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_borders.scss
+-rw-r--r--   0 root         (0) root         (0)       37 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_clearfix.scss
+-rw-r--r--   0 root         (0) root         (0)       50 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_cursor.scss
+-rw-r--r--   0 root         (0) root         (0)     1153 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_display.scss
+-rw-r--r--   0 root         (0) root         (0)     2533 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_flex.scss
+-rw-r--r--   0 root         (0) root         (0)      320 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_float.scss
+-rw-r--r--   0 root         (0) root         (0)      283 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_position.scss
+-rw-r--r--   0 root         (0) root         (0)      115 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_screenreaders.scss
+-rw-r--r--   0 root         (0) root         (0)      251 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_sizing.scss
+-rw-r--r--   0 root         (0) root         (0)     1521 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_spacing.scss
+-rw-r--r--   0 root         (0) root         (0)     1502 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_text.scss
+-rw-r--r--   0 root         (0) root         (0)      121 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_visibility.scss
+-rw-r--r--   0 root         (0) root         (0)     3790 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/colorbox.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.982178 codeforlife-portal-6.9.0/portal/static/portal/sass/modules/
+-rw-r--r--   0 root         (0) root         (0)      174 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/modules/_all.scss
+-rw-r--r--   0 root         (0) root         (0)       39 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/modules/_animation.scss
+-rw-r--r--   0 root         (0) root         (0)      498 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/modules/_breakpoints.scss
+-rw-r--r--   0 root         (0) root         (0)      107 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/modules/_card_constants.scss
+-rw-r--r--   0 root         (0) root         (0)     4211 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/modules/_colours.scss
+-rw-r--r--   0 root         (0) root         (0)       44 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/modules/_homepage_constants.scss
+-rw-r--r--   0 root         (0) root         (0)      105 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/modules/_levels.scss
+-rw-r--r--   0 root         (0) root         (0)     1493 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/modules/_mixins.scss
+-rw-r--r--   0 root         (0) root         (0)       31 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/modules/_spacing.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.982178 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/
+-rw-r--r--   0 root         (0) root         (0)     8787 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_banners.scss
+-rw-r--r--   0 root         (0) root         (0)       26 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_base.scss
+-rw-r--r--   0 root         (0) root         (0)     9002 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_buttons.scss
+-rw-r--r--   0 root         (0) root         (0)     3238 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_carousel.scss
+-rw-r--r--   0 root         (0) root         (0)     2445 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_footer.scss
+-rw-r--r--   0 root         (0) root         (0)     6245 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_forms.scss
+-rw-r--r--   0 root         (0) root         (0)     5866 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_grids.scss
+-rw-r--r--   0 root         (0) root         (0)     7316 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_header.scss
+-rw-r--r--   0 root         (0) root         (0)     3087 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_images.scss
+-rw-r--r--   0 root         (0) root         (0)     2126 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_popup.scss
+-rw-r--r--   0 root         (0) root         (0)      144 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_progress-bars.scss
+-rw-r--r--   0 root         (0) root         (0)     5052 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_subnavs.scss
+-rw-r--r--   0 root         (0) root         (0)     2978 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_tables.scss
+-rw-r--r--   0 root         (0) root         (0)     3788 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_text.scss
+-rw-r--r--   0 root         (0) root         (0)      956 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_ui-dialog.scss
+-rw-r--r--   0 root         (0) root         (0)     3468 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_utils.scss
+-rw-r--r--   0 root         (0) root         (0)      303 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_videos.scss
+-rw-r--r--   0 root         (0) root         (0)      807 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/sass/styles.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.986178 codeforlife-portal-6.9.0/portal/static/portal/video/
+-rw-r--r--   0 root         (0) root         (0)   999060 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/video/aimmo_play_now_background_video.mp4
+-rw-r--r--   0 root         (0) root         (0)   277957 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/static/portal/video/code for life .pdf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.986178 codeforlife-portal-6.9.0/portal/strings/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/strings/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      644 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/strings/about.py
+-rw-r--r--   0 root         (0) root         (0)      386 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/strings/help_and_support.py
+-rw-r--r--   0 root         (0) root         (0)      273 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/strings/home_learning.py
+-rw-r--r--   0 root         (0) root         (0)      274 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/strings/materials.py
+-rw-r--r--   0 root         (0) root         (0)      804 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/strings/play.py
+-rw-r--r--   0 root         (0) root         (0)      235 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/strings/student_aimmo_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)      257 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/strings/teach.py
+-rw-r--r--   0 root         (0) root         (0)      760 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/strings/teacher_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.986178 codeforlife-portal-6.9.0/portal/templates/
+-rw-r--r--   0 root         (0) root         (0)     1169 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/403.html
+-rw-r--r--   0 root         (0) root         (0)      563 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/404.html
+-rw-r--r--   0 root         (0) root         (0)     1703 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.986178 codeforlife-portal-6.9.0/portal/templates/captcha/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.986178 codeforlife-portal-6.9.0/portal/templates/captcha/includes/
+-rw-r--r--   0 root         (0) root         (0)     1409 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/captcha/includes/js_v2_invisible.html
+-rw-r--r--   0 root         (0) root         (0)      306 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/captcha/widget_v2_invisible.html
+-rw-r--r--   0 root         (0) root         (0)      268 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/email.html
+-rw-r--r--   0 root         (0) root         (0)       19 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/email.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.990178 codeforlife-portal-6.9.0/portal/templates/portal/
+-rw-r--r--   0 root         (0) root         (0)     9902 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/about.html
+-rw-r--r--   0 root         (0) root         (0)     9060 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/base.html
+-rw-r--r--   0 root         (0) root         (0)      447 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/base_no_userprofile.html
+-rw-r--r--   0 root         (0) root         (0)     4001 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/contribute.html
+-rw-r--r--   0 root         (0) root         (0)      918 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/dotmailer_consent_form.html
+-rw-r--r--   0 root         (0) root         (0)      641 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/email_invitation_sent.html
+-rw-r--r--   0 root         (0) root         (0)    11935 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/email_style_template.html
+-rw-r--r--   0 root         (0) root         (0)      806 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/email_verification_failed.html
+-rw-r--r--   0 root         (0) root         (0)     1000 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/email_verification_needed.html
+-rw-r--r--   0 root         (0) root         (0)     1223 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/form_shapes.html
+-rw-r--r--   0 root         (0) root         (0)     2921 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/getinvolved.html
+-rw-r--r--   0 root         (0) root         (0)     5342 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/home.html
+-rw-r--r--   0 root         (0) root         (0)     9707 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/home_learning.html
+-rw-r--r--   0 root         (0) root         (0)      894 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/locked_out.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.990178 codeforlife-portal-6.9.0/portal/templates/portal/login/
+-rw-r--r--   0 root         (0) root         (0)     1523 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/login/independent_student.html
+-rw-r--r--   0 root         (0) root         (0)     1011 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/login/student.html
+-rw-r--r--   0 root         (0) root         (0)      966 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/login/student_class_code.html
+-rw-r--r--   0 root         (0) root         (0)     2400 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/login/teacher.html
+-rw-r--r--   0 root         (0) root         (0)      361 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/mouseflow.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.994178 codeforlife-portal-6.9.0/portal/templates/portal/partials/
+-rw-r--r--   0 root         (0) root         (0)     4277 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/aimmo_games_table.html
+-rw-r--r--   0 root         (0) root         (0)     1235 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/banner.html
+-rw-r--r--   0 root         (0) root         (0)     2363 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/benefits.html
+-rw-r--r--   0 root         (0) root         (0)     1550 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/card_list.html
+-rw-r--r--   0 root         (0) root         (0)      415 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/character_list.html
+-rw-r--r--   0 root         (0) root         (0)     1275 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/delete_popup.html
+-rw-r--r--   0 root         (0) root         (0)     3652 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/footer.html
+-rw-r--r--   0 root         (0) root         (0)    19148 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/header.html
+-rw-r--r--   0 root         (0) root         (0)       89 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/headline.html
+-rw-r--r--   0 root         (0) root         (0)      786 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/hero_card.html
+-rw-r--r--   0 root         (0) root         (0)      566 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/info_popup.html
+-rw-r--r--   0 root         (0) root         (0)      875 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/popup.html
+-rw-r--r--   0 root         (0) root         (0)      329 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/register_newsletter_tickbox.html
+-rw-r--r--   0 root         (0) root         (0)      311 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/register_over_required_age_tickbox.html
+-rw-r--r--   0 root         (0) root         (0)      671 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/teacher_non_dashboard_subnav.html
+-rw-r--r--   0 root         (0) root         (0)      671 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/partials/teacher_non_dashboard_subnav_account.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.994178 codeforlife-portal-6.9.0/portal/templates/portal/play/
+-rw-r--r--   0 root         (0) root         (0)     2907 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/play/independent_student_dashboard.html
+-rw-r--r--   0 root         (0) root         (0)     1403 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/play/student_aimmo_dashboard.html
+-rw-r--r--   0 root         (0) root         (0)     3898 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/play/student_dashboard.html
+-rw-r--r--   0 root         (0) root         (0)     6882 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/play/student_edit_account.html
+-rw-r--r--   0 root         (0) root         (0)     2980 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/play/student_join_organisation.html
+-rw-r--r--   0 root         (0) root         (0)     5162 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/play.html
+-rw-r--r--   0 root         (0) root         (0)    33849 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/privacy_policy.html
+-rw-r--r--   0 root         (0) root         (0)     7916 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/register.html
+-rw-r--r--   0 root         (0) root         (0)     1373 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/reset_password.html
+-rw-r--r--   0 root         (0) root         (0)     3041 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/reset_password_confirm.html
+-rw-r--r--   0 root         (0) root         (0)      667 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/reset_password_done.html
+-rw-r--r--   0 root         (0) root         (0)      748 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/reset_password_email_sent.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.994178 codeforlife-portal-6.9.0/portal/templates/portal/tag_manager/
+-rw-r--r--   0 root         (0) root         (0)      661 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/tag_manager/tag_manager_body.html
+-rw-r--r--   0 root         (0) root         (0)     1288 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/tag_manager/tag_manager_head.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.998178 codeforlife-portal-6.9.0/portal/templates/portal/teach/
+-rw-r--r--   0 root         (0) root         (0)      582 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/base_registering.html
+-rw-r--r--   0 root         (0) root         (0)     6997 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/class.html
+-rw-r--r--   0 root         (0) root         (0)    29188 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/dashboard.html
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/invite.html
+-rw-r--r--   0 root         (0) root         (0)     2804 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/onboarding_classes.html
+-rw-r--r--   0 root         (0) root         (0)     8862 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/onboarding_print.html
+-rw-r--r--   0 root         (0) root         (0)     7768 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/onboarding_school.html
+-rw-r--r--   0 root         (0) root         (0)     2399 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/onboarding_students.html
+-rw-r--r--   0 root         (0) root         (0)     2453 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_add_external_student.html
+-rw-r--r--   0 root         (0) root         (0)     1189 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_added_external_student.html
+-rw-r--r--   0 root         (0) root         (0)     4427 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_aimmo_dashboard.html
+-rw-r--r--   0 root         (0) root         (0)     4283 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_dismiss_students.html
+-rw-r--r--   0 root         (0) root         (0)     4604 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_edit_class.html
+-rw-r--r--   0 root         (0) root         (0)     2746 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_edit_student.html
+-rw-r--r--   0 root         (0) root         (0)     1780 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_move_all_classes.html
+-rw-r--r--   0 root         (0) root         (0)     1591 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_move_students.html
+-rw-r--r--   0 root         (0) root         (0)     3348 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_move_students_to_class.html
+-rw-r--r--   0 root         (0) root         (0)     2646 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_resources.html
+-rw-r--r--   0 root         (0) root         (0)     8724 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/teach.html
+-rw-r--r--   0 root         (0) root         (0)    19856 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/portal/terms.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.998178 codeforlife-portal-6.9.0/portal/templates/two_factor/
+-rw-r--r--   0 root         (0) root         (0)      443 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/_base.html
+-rw-r--r--   0 root         (0) root         (0)      355 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0 root         (0) root         (0)      358 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/_wizard_actions_enable_2fa.html
+-rw-r--r--   0 root         (0) root         (0)      357 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/_wizard_actions_submit.html
+-rw-r--r--   0 root         (0) root         (0)      267 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/_wizard_forms.html
+-rw-r--r--   0 root         (0) root         (0)      262 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/_wizard_forms_token.html
+-rw-r--r--   0 root         (0) root         (0)      262 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/backup_token.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.998178 codeforlife-portal-6.9.0/portal/templates/two_factor/core/
+-rw-r--r--   0 root         (0) root         (0)     1442 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0 root         (0) root         (0)     2723 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/core/login.html
+-rw-r--r--   0 root         (0) root         (0)     3145 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/core/setup.html
+-rw-r--r--   0 root         (0) root         (0)      600 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/core/setup_complete.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:36.998178 codeforlife-portal-6.9.0/portal/templates/two_factor/profile/
+-rw-r--r--   0 root         (0) root         (0)     1010 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/profile/disable.html
+-rw-r--r--   0 root         (0) root         (0)     1800 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/profile/profile.html
+-rw-r--r--   0 root         (0) root         (0)      266 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templates/two_factor/setup_wizard_token.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.002178 codeforlife-portal-6.9.0/portal/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4637 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templatetags/app_tags.py
+-rw-r--r--   0 root         (0) root         (0)      823 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templatetags/banner_tags.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templatetags/benefits_tags.py
+-rw-r--r--   0 root         (0) root         (0)      509 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templatetags/card_list_tags.py
+-rw-r--r--   0 root         (0) root         (0)      552 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templatetags/character_list_tags.py
+-rw-r--r--   0 root         (0) root         (0)      165 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templatetags/future.py
+-rw-r--r--   0 root         (0) root         (0)      420 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templatetags/headline_tags.py
+-rw-r--r--   0 root         (0) root         (0)      939 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templatetags/hero_card_tags.py
+-rw-r--r--   0 root         (0) root         (0)      448 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/templatetags/table_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.002178 codeforlife-portal-6.9.0/portal/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/base_test.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.006178 codeforlife-portal-6.9.0/portal/tests/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_make_portaladmin_teacher.py
+-rw-r--r--   0 root         (0) root         (0)      555 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_preview_user_remove.py
+-rw-r--r--   0 root         (0) root         (0)      639 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_preview_users.py
+-rw-r--r--   0 root         (0) root         (0)      391 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_remove_front_page_news.py
+-rw-r--r--   0 root         (0) root         (0)      403 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_remove_guardian.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_use_common_models.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_verify_portaladmin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.006178 codeforlife-portal-6.9.0/portal/tests/pageObjects/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.006178 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.010178 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/admin/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/admin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      352 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/admin/admin_base_page.py
+-rw-r--r--   0 root         (0) root         (0)      289 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/admin/admin_data_page.py
+-rw-r--r--   0 root         (0) root         (0)      286 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/admin/admin_map_page.py
+-rw-r--r--   0 root         (0) root         (0)     4780 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/base_page.py
+-rw-r--r--   0 root         (0) root         (0)      458 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/email_verification_needed_page.py
+-rw-r--r--   0 root         (0) root         (0)      235 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/forbidden_page.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/game_page.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/home_page.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/independent_login_page.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/kurono_teacher_dashboard_page.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/password_reset_form_page.py
+-rw-r--r--   0 root         (0) root         (0)      666 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/password_reset_page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.010178 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/play/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/play/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3113 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/play/account_page.py
+-rw-r--r--   0 root         (0) root         (0)      552 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/play/dashboard_page.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/play/join_school_or_club_page.py
+-rw-r--r--   0 root         (0) root         (0)      840 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/play/play_base_page.py
+-rw-r--r--   0 root         (0) root         (0)      231 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/play_page.py
+-rw-r--r--   0 root         (0) root         (0)      246 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/resources_page.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/signup_page.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/student_login_class_code.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/student_login_page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.010178 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      928 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/add_independent_student_to_class_page.py
+-rw-r--r--   0 root         (0) root         (0)      539 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/added_independent_student_to_class_page.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/class_page.py
+-rw-r--r--   0 root         (0) root         (0)     7450 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/dashboard_page.py
+-rw-r--r--   0 root         (0) root         (0)      833 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/dismiss_students_page.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/edit_student_page.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/move_class_page.py
+-rw-r--r--   0 root         (0) root         (0)      836 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/move_classes_page.py
+-rw-r--r--   0 root         (0) root         (0)      626 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/move_students_disambiguate_page.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/move_students_page.py
+-rw-r--r--   0 root         (0) root         (0)      998 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/onboarding_classes_page.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/onboarding_organisation_page.py
+-rw-r--r--   0 root         (0) root         (0)      815 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/onboarding_revoke_request_page.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/onboarding_student_list_page.py
+-rw-r--r--   0 root         (0) root         (0)      924 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/onboarding_students_page.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/teach_base_page.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teacher_login_page.py
+-rw-r--r--   0 root         (0) root         (0)      469 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/selenium_test_case.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.010178 codeforlife-portal-6.9.0/portal/tests/snapshots/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/snapshots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8572 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/snapshots/snap_test_partials.py
+-rw-r--r--   0 root         (0) root         (0)     3846 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_2FA.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_admin.py
+-rw-r--r--   0 root         (0) root         (0)     5355 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_aimmo_dashboards.py
+-rw-r--r--   0 root         (0) root         (0)    10772 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_captcha_forms.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_class.py
+-rw-r--r--   0 root         (0) root         (0)     9654 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_emails.py
+-rw-r--r--   0 root         (0) root         (0)    19552 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_independent_student.py
+-rw-r--r--   0 root         (0) root         (0)      711 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_invite_teacher.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_middleware.py
+-rw-r--r--   0 root         (0) root         (0)      838 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_newsletter_footer.py
+-rw-r--r--   0 root         (0) root         (0)    14140 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     4030 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_partials.py
+-rw-r--r--   0 root         (0) root         (0)    12639 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_ratelimit.py
+-rw-r--r--   0 root         (0) root         (0)      856 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_react_test_space.py
+-rw-r--r--   0 root         (0) root         (0)     7965 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_school_student.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_security.py
+-rw-r--r--   0 root         (0) root         (0)    29040 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_teacher.py
+-rw-r--r--   0 root         (0) root         (0)    21448 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_teacher_student.py
+-rw-r--r--   0 root         (0) root         (0)    26171 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/test_views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.014178 codeforlife-portal-6.9.0/portal/tests/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      649 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/utils/aimmo_games.py
+-rw-r--r--   0 root         (0) root         (0)      183 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/utils/classes.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/tests/utils/messages.py
+-rw-r--r--   0 root         (0) root         (0)    15571 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.014178 codeforlife-portal-6.9.0/portal/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      443 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/about.py
+-rw-r--r--   0 root         (0) root         (0)      957 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.014178 codeforlife-portal-6.9.0/portal/views/aimmo/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/aimmo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3877 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/aimmo/dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/api.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/dotmailer.py
+-rw-r--r--   0 root         (0) root         (0)     3798 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/email.py
+-rw-r--r--   0 root         (0) root         (0)     8400 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/home.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.014178 codeforlife-portal-6.9.0/portal/views/login/
+-rw-r--r--   0 root         (0) root         (0)      399 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/login/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/login/independent_student.py
+-rw-r--r--   0 root         (0) root         (0)     3720 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/login/student.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/login/teacher.py
+-rw-r--r--   0 root         (0) root         (0)     8123 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/organisation.py
+-rw-r--r--   0 root         (0) root         (0)      308 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/play_landing_page.py
+-rw-r--r--   0 root         (0) root         (0)      195 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/privacy_policy.py
+-rw-r--r--   0 root         (0) root         (0)     8644 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.014178 codeforlife-portal-6.9.0/portal/views/student/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/student/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8551 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/student/edit_account_details.py
+-rw-r--r--   0 root         (0) root         (0)     8362 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/student/play.py
+-rw-r--r--   0 root         (0) root         (0)      210 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/teach.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.014178 codeforlife-portal-6.9.0/portal/views/teacher/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/teacher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18315 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/teacher/dashboard.py
+-rw-r--r--   0 root         (0) root         (0)    32106 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/teacher/teach.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/teacher/teacher_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-23 09:40:37.018178 codeforlife-portal-6.9.0/portal/views/two_factor/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/two_factor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/two_factor/core.py
+-rw-r--r--   0 root         (0) root         (0)      257 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/two_factor/form.py
+-rw-r--r--   0 root         (0) root         (0)      383 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/views/two_factor/profile.py
+-rw-r--r--   0 root         (0) root         (0)      401 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/portal/wsgi.py
+-rw-r--r--   0 root         (0) root         (0)      133 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      199 2022-06-23 09:40:37.018178 codeforlife-portal-6.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1543 2022-06-23 09:37:44.000000 codeforlife-portal-6.9.0/setup.py
```

### Comparing `codeforlife-portal-6.8.9/LICENSE.md` & `codeforlife-portal-6.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/README.md` & `codeforlife-portal-6.9.0/README.md`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/codeforlife_portal.egg-info/SOURCES.txt` & `codeforlife-portal-6.9.0/codeforlife_portal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/deploy/middleware/admin_access.py` & `codeforlife-portal-6.9.0/deploy/middleware/admin_access.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/deploy/middleware/basicauth.py` & `codeforlife-portal-6.9.0/deploy/middleware/basicauth.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/deploy/middleware/security.py` & `codeforlife-portal-6.9.0/deploy/middleware/security.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/deploy/middleware/session_timeout.py` & `codeforlife-portal-6.9.0/deploy/middleware/session_timeout.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/deploy/static/apple-touch-icon-120x120.png` & `codeforlife-portal-6.9.0/deploy/static/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/deploy/static/apple-touch-icon-152x152.png` & `codeforlife-portal-6.9.0/deploy/static/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/deploy/static/apple-touch-icon-180x180.png` & `codeforlife-portal-6.9.0/deploy/static/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/deploy/static/apple-touch-icon-76x76.png` & `codeforlife-portal-6.9.0/deploy/static/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/deploy/static/apple-touch-icon.png` & `codeforlife-portal-6.9.0/deploy/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/admin.py` & `codeforlife-portal-6.9.0/portal/admin.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/app_settings.py` & `codeforlife-portal-6.9.0/portal/app_settings.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/autoconfig.py` & `codeforlife-portal-6.9.0/portal/autoconfig.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/backends.py` & `codeforlife-portal-6.9.0/portal/backends.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/csp_config.py` & `codeforlife-portal-6.9.0/portal/csp_config.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/forms/add_game.py` & `codeforlife-portal-6.9.0/portal/forms/add_game.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/forms/admin.py` & `codeforlife-portal-6.9.0/portal/forms/admin.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/forms/dotmailer.py` & `codeforlife-portal-6.9.0/portal/forms/dotmailer.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/forms/organisation.py` & `codeforlife-portal-6.9.0/portal/forms/organisation.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/forms/play.py` & `codeforlife-portal-6.9.0/portal/forms/play.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/forms/registration.py` & `codeforlife-portal-6.9.0/portal/forms/registration.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/forms/teach.py` & `codeforlife-portal-6.9.0/portal/forms/teach.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/asset-manifest.json` & `codeforlife-portal-6.9.0/portal/frontend/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/index.html` & `codeforlife-portal-6.9.0/portal/frontend/index.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/static/js/787.cda612ba.chunk.js` & `codeforlife-portal-6.9.0/portal/frontend/static/js/787.cda612ba.chunk.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/static/js/787.cda612ba.chunk.js.map` & `codeforlife-portal-6.9.0/portal/frontend/static/js/787.cda612ba.chunk.js.map`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/static/js/main.8c02947d.js` & `codeforlife-portal-6.9.0/portal/frontend/static/js/main.8c02947d.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/static/js/main.8c02947d.js.LICENSE.txt` & `codeforlife-portal-6.9.0/portal/frontend/static/js/main.8c02947d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/static/js/main.8c02947d.js.map` & `codeforlife-portal-6.9.0/portal/frontend/static/js/main.8c02947d.js.map`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/static/media/facebook.2bdba6ecdf25da4a6d91d9df9e3f5830.svg` & `codeforlife-portal-6.9.0/portal/frontend/static/media/facebook.2bdba6ecdf25da4a6d91d9df9e3f5830.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/static/media/logo_cfl.06fffc34beb6c215ab01.png` & `codeforlife-portal-6.9.0/portal/frontend/static/media/logo_cfl.06fffc34beb6c215ab01.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/static/media/logo_ocado_group.bf2daf768df6901d40924159853b612d.svg` & `codeforlife-portal-6.9.0/portal/frontend/static/media/logo_ocado_group.bf2daf768df6901d40924159853b612d.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/static/media/ocado.5e7ae9a2adbc50ec6f96f3f6366eea25.svg` & `codeforlife-portal-6.9.0/portal/frontend/static/media/ocado.5e7ae9a2adbc50ec6f96f3f6366eea25.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/frontend/static/media/twitter.3f190a3549dea2464ca62924d629b961.svg` & `codeforlife-portal-6.9.0/portal/frontend/static/media/twitter.3f190a3549dea2464ca62924d629b961.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/helpers/decorators.py` & `codeforlife-portal-6.9.0/portal/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/helpers/password.py` & `codeforlife-portal-6.9.0/portal/helpers/password.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/helpers/ratelimit.py` & `codeforlife-portal-6.9.0/portal/helpers/ratelimit.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0001_squashed_0041_new_news.py` & `codeforlife-portal-6.9.0/portal/migrations/0001_squashed_0041_new_news.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0044_auto_20150430_0959.py` & `codeforlife-portal-6.9.0/portal/migrations/0044_auto_20150430_0959.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0046_auto_20150723_1101.py` & `codeforlife-portal-6.9.0/portal/migrations/0046_auto_20150723_1101.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0049_refactor_emailverifications.py` & `codeforlife-portal-6.9.0/portal/migrations/0049_refactor_emailverifications.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0050_refactor_emailverifications_2.py` & `codeforlife-portal-6.9.0/portal/migrations/0050_refactor_emailverifications_2.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0051_add_missing_ev_records.py` & `codeforlife-portal-6.9.0/portal/migrations/0051_add_missing_ev_records.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0053_refactor_teacher_student_1.py` & `codeforlife-portal-6.9.0/portal/migrations/0053_refactor_teacher_student_1.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0054_pending_join_request_can_be_blank.py` & `codeforlife-portal-6.9.0/portal/migrations/0054_pending_join_request_can_be_blank.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0055_add_preview_user.py` & `codeforlife-portal-6.9.0/portal/migrations/0055_add_preview_user.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0058_move_to_common_models.py` & `codeforlife-portal-6.9.0/portal/migrations/0058_move_to_common_models.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0059_move_email_verifications_to_common.py` & `codeforlife-portal-6.9.0/portal/migrations/0059_move_email_verifications_to_common.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0060_delete_guardian.py` & `codeforlife-portal-6.9.0/portal/migrations/0060_delete_guardian.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0061_make_portaladmin_teacher.py` & `codeforlife-portal-6.9.0/portal/migrations/0061_make_portaladmin_teacher.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/migrations/0062_verify_portaladmin.py` & `codeforlife-portal-6.9.0/portal/migrations/0062_verify_portaladmin.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/pipeline_compilers/libsass_compiler.py` & `codeforlife-portal-6.9.0/portal/pipeline_compilers/libsass_compiler.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.eot` & `codeforlife-portal-6.9.0/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.svg` & `codeforlife-portal-6.9.0/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.ttf` & `codeforlife-portal-6.9.0/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.woff` & `codeforlife-portal-6.9.0/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.woff2` & `codeforlife-portal-6.9.0/portal/static/portal/fonts/bootstrap/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/10x_logo.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/10x_logo.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/RR_logo_grass_background.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/RR_logo_grass_background.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/RR_logo_green.svg` & `codeforlife-portal-6.9.0/portal/static/portal/img/RR_logo_green.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/RR_logo_simple.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/RR_logo_simple.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/about_us_cfl.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/about_us_cfl.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/about_us_hero.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/about_us_hero.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/about_us_ocado.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/about_us_ocado.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/barefoot_logo.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/barefoot_logo.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/bcs_logo.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/bcs_logo.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/clubs.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/clubs.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/colorboxImages/controls.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/colorboxImages/controls.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/colorboxImages/loading.gif` & `codeforlife-portal-6.9.0/portal/static/portal/img/colorboxImages/loading.gif`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/confirmation_tick.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/confirmation_tick.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/cross.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/cross.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/dee.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/dee.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/facebook.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/facebook.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/get_involved_hero.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/get_involved_hero.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/gitbook.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/gitbook.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/gitbook_space.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/gitbook_space.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/github.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/github.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/github_hero.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/github_hero.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/gla_logo.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/gla_logo.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/hamburger.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/hamburger.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/help_and_support_hero.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/help_and_support_hero.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/home_educate.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/home_educate.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/home_educate_hero.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/home_educate_hero.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/home_learning_hero.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/home_learning_hero.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/home_play.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/home_play.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/home_play_hero.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/home_play_hero.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/hope_logo.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/hope_logo.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/icl_logo.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/icl_logo.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/icon_controller.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/icon_controller.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/icon_free.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/icon_free.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/icon_globe.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/icon_globe.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/icon_piechart.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/icon_piechart.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/icon_step_by_step.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/icon_step_by_step.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/icon_tracking.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/icon_tracking.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/icon_uk_flag.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/icon_uk_flag.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/kirsty.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/kirsty.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/kurono_hero.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/kurono_hero.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/kurono_landing_hero.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/kurono_landing_hero.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/kurono_logo.svg` & `codeforlife-portal-6.9.0/portal/static/portal/img/kurono_logo.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/kurono_logo_grey_background.svg` & `codeforlife-portal-6.9.0/portal/static/portal/img/kurono_logo_grey_background.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/kurono_logo_mark.svg` & `codeforlife-portal-6.9.0/portal/static/portal/img/kurono_logo_mark.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/kurono_resources_hero.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/kurono_resources_hero.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/kurono_story.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/kurono_story.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/logo_cfl.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/logo_cfl.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/logo_cfl_reminder_cards.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/logo_cfl_reminder_cards.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/logo_cfl_white_landscape.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/logo_cfl_white_landscape.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/logo_ocado.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/logo_ocado.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/logo_ocado_group.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/logo_ocado_group.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/logo_ocado_group.svg` & `codeforlife-portal-6.9.0/portal/static/portal/img/logo_ocado_group.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/logo_ocado_group_white.svg` & `codeforlife-portal-6.9.0/portal/static/portal/img/logo_ocado_group_white.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/mc_saatchi_logo.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/mc_saatchi_logo.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/nigel.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/nigel.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/ocado-swirl.svg` & `codeforlife-portal-6.9.0/portal/static/portal/img/ocado-swirl.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/oval_pink.svg` & `codeforlife-portal-6.9.0/portal/static/portal/img/oval_pink.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/paper_plane.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/paper_plane.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/phil.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/phil.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/polygon_blue.svg` & `codeforlife-portal-6.9.0/portal/static/portal/img/polygon_blue.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/polygon_pink.svg` & `codeforlife-portal-6.9.0/portal/static/portal/img/polygon_pink.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/polygon_yellow.svg` & `codeforlife-portal-6.9.0/portal/static/portal/img/polygon_yellow.svg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/pressure_cooker_logo.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/pressure_cooker_logo.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/rapid_router.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/rapid_router.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/rapid_router_landing_hero.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/rapid_router_landing_hero.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/rapidrouter.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/rapidrouter.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/resources_hero.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/resources_hero.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/resources_montage.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/resources_montage.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/reuben.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/reuben.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/rob.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/rob.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/rr_advanced.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/rr_advanced.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/rr_beginner.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/rr_beginner.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/rr_intermediate.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/rr_intermediate.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/sadface.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/sadface.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/sharon_harrison.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/sharon_harrison.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/sian.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/sian.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/teaching_resources_hero.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/teaching_resources_hero.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_educate_kurono.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_educate_kurono.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_educate_rapid_router.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_educate_rapid_router.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_educate_resources.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_educate_resources.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_intro_c4l.jpg` & `codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_intro_c4l.jpg`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_kurono_resources.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_kurono_resources.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_play_kurono.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_play_kurono.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/thumbnail_play_rapid_router.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/thumbnail_play_rapid_router.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/twitter.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/twitter.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/universities.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/universities.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/wes.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/wes.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/img/x_close_video.png` & `codeforlife-portal-6.9.0/portal/static/portal/img/x_close_video.png`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/aimmoGame.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/aimmoGame.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/bootstrap.min.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/carouselCards.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/carouselCards.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/common.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/common.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/fuzzySchoolLookup.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/fuzzySchoolLookup.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/jquery.placeholder.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/jquery.placeholder.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/lib/jquery-3.5.1.min.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/lib/jquery-3.5.1.min.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/lib/jquery-video-lightning.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/lib/jquery-video-lightning.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/lib/jquery.colorbox.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/lib/jquery.colorbox.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/lib/jquery.easy-ticker.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/lib/jquery.easy-ticker.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/lib/modernizr-build.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/lib/modernizr-build.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/lib/papaparse.min.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/lib/papaparse.min.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/organisation_manage.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/organisation_manage.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/passwordStrength.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/passwordStrength.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/play.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/play.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/riveted.min.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/riveted.min.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/sticky_subnav.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/sticky_subnav.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/teach_browser.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/teach_browser.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/js/teach_class.js` & `codeforlife-portal-6.9.0/portal/static/portal/js/teach_class.js`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_alerts.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_alerts.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_badges.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_badges.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_breadcrumbs.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_button-groups.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_button-groups.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_buttons.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_carousel.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_close.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_code.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_code.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_component-animations.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_component-animations.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_dropdowns.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_dropdowns.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_forms.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_forms.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_glyphicons.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_glyphicons.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_grid.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_input-groups.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_input-groups.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_jumbotron.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_jumbotron.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_labels.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_labels.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_list-group.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_media.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_media.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_mixins.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_modals.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_modals.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_navbar.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_navs.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_navs.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_normalize.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_normalize.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_pager.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_pager.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_pagination.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_panels.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_panels.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_popovers.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_popovers.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_print.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_print.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_progress-bars.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_progress-bars.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_responsive-embed.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_responsive-embed.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_responsive-utilities.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_responsive-utilities.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_scaffolding.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_scaffolding.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_tables.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_theme.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_theme.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_thumbnails.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_thumbnails.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_tooltip.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_type.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_utilities.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_variables.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/_wells.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/_wells.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_breakpoints.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_buttons.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_clearfix.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_clearfix.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_forms.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_gradients.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_grid-framework.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_grid-framework.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_grid.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_hide-text.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_hide-text.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_image.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_image.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_list-group.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_panels.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_panels.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_table-row.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_table-row.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap/mixins/_vendor-prefixes.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap/mixins/_vendor-prefixes.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_mixins/_border-radius.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_mixins/_hover.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_mixins/_hover.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_partials/_dropdown.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_partials/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_partials/_glyphicons.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_partials/_glyphicons.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_partials/_grid.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_partials/_grid.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_partials/_variables.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_partials/_variables.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_borders.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_borders.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_display.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_display.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_flex.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_flex.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_spacing.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_spacing.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/bootstrap_utilities/_text.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/bootstrap_utilities/_text.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/colorbox.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/colorbox.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/modules/_colours.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/modules/_colours.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/modules/_mixins.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/modules/_mixins.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_banners.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_banners.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_buttons.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_buttons.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_carousel.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_carousel.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_footer.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_footer.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_forms.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_forms.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_grids.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_grids.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_header.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_header.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_images.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_images.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_popup.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_popup.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_subnavs.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_subnavs.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_tables.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_tables.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_text.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_text.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_ui-dialog.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_ui-dialog.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/partials/_utils.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/partials/_utils.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/sass/styles.scss` & `codeforlife-portal-6.9.0/portal/static/portal/sass/styles.scss`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/video/aimmo_play_now_background_video.mp4` & `codeforlife-portal-6.9.0/portal/static/portal/video/aimmo_play_now_background_video.mp4`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/static/portal/video/code for life .pdf` & `codeforlife-portal-6.9.0/portal/static/portal/video/code for life .pdf`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/strings/about.py` & `codeforlife-portal-6.9.0/portal/strings/about.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/strings/play.py` & `codeforlife-portal-6.9.0/portal/strings/play.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/strings/teacher_resources.py` & `codeforlife-portal-6.9.0/portal/strings/teacher_resources.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/403.html` & `codeforlife-portal-6.9.0/portal/templates/403.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/404.html` & `codeforlife-portal-6.9.0/portal/templates/404.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/500.html` & `codeforlife-portal-6.9.0/portal/templates/500.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/captcha/includes/js_v2_invisible.html` & `codeforlife-portal-6.9.0/portal/templates/captcha/includes/js_v2_invisible.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/about.html` & `codeforlife-portal-6.9.0/portal/templates/portal/about.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/base.html` & `codeforlife-portal-6.9.0/portal/templates/portal/base.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/contribute.html` & `codeforlife-portal-6.9.0/portal/templates/portal/contribute.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/dotmailer_consent_form.html` & `codeforlife-portal-6.9.0/portal/templates/portal/dotmailer_consent_form.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/email_invitation_sent.html` & `codeforlife-portal-6.9.0/portal/templates/portal/email_invitation_sent.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/email_style_template.html` & `codeforlife-portal-6.9.0/portal/templates/portal/email_style_template.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/email_verification_failed.html` & `codeforlife-portal-6.9.0/portal/templates/portal/email_verification_failed.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/email_verification_needed.html` & `codeforlife-portal-6.9.0/portal/templates/portal/email_verification_needed.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/form_shapes.html` & `codeforlife-portal-6.9.0/portal/templates/portal/form_shapes.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/getinvolved.html` & `codeforlife-portal-6.9.0/portal/templates/portal/getinvolved.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/home.html` & `codeforlife-portal-6.9.0/portal/templates/portal/home.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/home_learning.html` & `codeforlife-portal-6.9.0/portal/templates/portal/home_learning.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/locked_out.html` & `codeforlife-portal-6.9.0/portal/templates/portal/locked_out.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/login/independent_student.html` & `codeforlife-portal-6.9.0/portal/templates/portal/login/independent_student.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/login/student.html` & `codeforlife-portal-6.9.0/portal/templates/portal/login/student.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/login/student_class_code.html` & `codeforlife-portal-6.9.0/portal/templates/portal/login/student_class_code.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/login/teacher.html` & `codeforlife-portal-6.9.0/portal/templates/portal/login/teacher.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/aimmo_games_table.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/aimmo_games_table.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/banner.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/banner.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/benefits.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/benefits.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/card_list.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/card_list.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/delete_popup.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/delete_popup.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/footer.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/footer.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/header.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/header.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/hero_card.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/hero_card.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/info_popup.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/info_popup.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/popup.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/popup.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/teacher_non_dashboard_subnav.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/teacher_non_dashboard_subnav.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/partials/teacher_non_dashboard_subnav_account.html` & `codeforlife-portal-6.9.0/portal/templates/portal/partials/teacher_non_dashboard_subnav_account.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/play/independent_student_dashboard.html` & `codeforlife-portal-6.9.0/portal/templates/portal/play/independent_student_dashboard.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/play/student_aimmo_dashboard.html` & `codeforlife-portal-6.9.0/portal/templates/portal/play/student_aimmo_dashboard.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/play/student_dashboard.html` & `codeforlife-portal-6.9.0/portal/templates/portal/play/student_dashboard.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/play/student_edit_account.html` & `codeforlife-portal-6.9.0/portal/templates/portal/play/student_edit_account.html`

 * *Files 12% similar despite different names*

```diff
@@ -21,381 +21,411 @@
 00000140: 742d 2d70 7269 6d61 7279 223e 5765 6c63  t--primary">Welc
 00000150: 6f6d 652c 207b 7b20 7573 6572 7c6d 616b  ome, {{ user|mak
 00000160: 655f 696e 746f 5f75 7365 726e 616d 6520  e_into_username 
 00000170: 7d7d 3c2f 6831 3e0a 2020 2020 2020 2020  }}</h1>.        
 00000180: 3c2f 6469 763e 0a20 2020 203c 2f73 6563  </div>.    </sec
 00000190: 7469 6f6e 3e0a 7b25 2065 6e64 626c 6f63  tion>.{% endbloc
 000001a0: 6b20 7375 624e 6176 2025 7d0a 0a7b 2520  k subNav %}..{% 
-000001b0: 626c 6f63 6b20 636f 6e74 656e 7420 257d  block content %}
-000001c0: 0a3c 6469 7620 6964 3d22 706c 6179 5f61  .<div id="play_a
-000001d0: 6363 6f75 6e74 5f70 6167 6522 3e3c 2f64  ccount_page"></d
-000001e0: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
-000001f0: 6261 636b 6772 6f75 6e64 2063 6f6e 7461  background conta
-00000200: 696e 6572 223e 0a20 2020 203c 7365 6374  iner">.    <sect
-00000210: 696f 6e3e 3c68 343e 0a20 2020 2020 2020  ion><h4>.       
-00000220: 207b 2520 6966 2075 7365 722e 6e65 775f   {% if user.new_
-00000230: 7374 7564 656e 742e 636c 6173 735f 6669  student.class_fi
-00000240: 656c 6420 257d 0a20 2020 2020 2020 2020  eld %}.         
-00000250: 2020 2055 7064 6174 6520 796f 7572 2070     Update your p
-00000260: 6173 7377 6f72 640a 2020 2020 2020 2020  assword.        
-00000270: 7b25 2065 6c73 6520 257d 0a20 2020 2020  {% else %}.     
-00000280: 2020 2020 2020 2055 7064 6174 6520 796f         Update yo
-00000290: 7572 2061 6363 6f75 6e74 2064 6574 6169  ur account detai
-000002a0: 6c73 0a20 2020 2020 2020 207b 2520 656e  ls.        {% en
-000002b0: 6469 6620 257d 0a20 2020 203c 2f68 343e  dif %}.    </h4>
-000002c0: 3c2f 7365 6374 696f 6e3e 0a0a 2020 2020  </section>..    
-000002d0: 7b25 2069 6620 7573 6572 2e6e 6577 5f73  {% if user.new_s
-000002e0: 7475 6465 6e74 2e63 6c61 7373 5f66 6965  tudent.class_fie
-000002f0: 6c64 2025 7d0a 2020 2020 2020 2020 3c70  ld %}.        <p
-00000300: 3e59 6f75 206d 6179 2065 6469 7420 796f  >You may edit yo
-00000310: 7572 2070 6173 7377 6f72 6420 6265 6c6f  ur password belo
-00000320: 772e 2049 7420 6d75 7374 2062 6520 6c6f  w. It must be lo
-00000330: 6e67 2065 6e6f 7567 6820 616e 6420 6861  ng enough and ha
-00000340: 7264 2065 6e6f 7567 6820 746f 2073 746f  rd enough to sto
-00000350: 7020 796f 7572 2066 7269 656e 6473 2067  p your friends g
-00000360: 7565 7373 696e 6720 6974 2061 6e64 0a20  uessing it and. 
-00000370: 2020 2020 2020 2020 2020 2073 7465 616c             steal
-00000380: 696e 6720 616c 6c20 6f66 2079 6f75 7220  ing all of your 
-00000390: 6861 7264 2077 6f72 6b2e 2043 686f 6f73  hard work. Choos
-000003a0: 6520 736f 6d65 7468 696e 6720 6d65 6d6f  e something memo
-000003b0: 7261 626c 6520 7468 6f75 6768 2e3c 2f70  rable though.</p
-000003c0: 3e0a 2020 2020 2020 2020 3c70 3e49 6620  >.        <p>If 
-000003d0: 796f 7520 6861 7665 2061 6e79 2070 726f  you have any pro
-000003e0: 626c 656d 732c 2061 736b 2061 2074 6561  blems, ask a tea
-000003f0: 6368 6572 2074 6f20 6865 6c70 2079 6f75  cher to help you
-00000400: 2e3c 2f70 3e0a 2020 2020 7b25 2065 6c73  .</p>.    {% els
-00000410: 6520 257d 0a20 2020 2020 2020 203c 703e  e %}.        <p>
-00000420: 596f 7520 6361 6e20 7570 6461 7465 2079  You can update y
-00000430: 6f75 7220 6163 636f 756e 7420 6465 7461  our account deta
-00000440: 696c 7320 6265 6c6f 772e 3c2f 703e 0a20  ils below.</p>. 
-00000450: 2020 2020 2020 203c 703e 506c 6561 7365         <p>Please
-00000460: 206e 6f74 653a 2049 6620 796f 7520 6368   note: If you ch
-00000470: 616e 6765 2079 6f75 7220 656d 6169 6c20  ange your email 
-00000480: 6164 6472 6573 732c 2079 6f75 2077 696c  address, you wil
-00000490: 6c20 6e65 6564 2074 6f20 7265 2d76 6572  l need to re-ver
-000004a0: 6966 7920 6974 2e3c 2f62 723e 0a20 2020  ify it.</br>.   
-000004b0: 2020 2020 2020 2020 2050 6c65 6173 6520           Please 
-000004c0: 656e 7375 7265 2079 6f75 7220 7061 7373  ensure your pass
-000004d0: 776f 7264 2069 7320 7374 726f 6e67 2065  word is strong e
-000004e0: 6e6f 7567 6820 746f 2062 6520 7365 6375  nough to be secu
-000004f0: 7265 2e3c 2f70 3e0a 2020 2020 7b25 2065  re.</p>.    {% e
-00000500: 6e64 6966 2025 7d0a 0a20 2020 203c 666f  ndif %}..    <fo
-00000510: 726d 2069 643d 2273 7475 6465 6e74 5f61  rm id="student_a
-00000520: 6363 6f75 6e74 5f66 6f72 6d22 206d 6574  ccount_form" met
-00000530: 686f 643d 2270 6f73 7422 3e0a 2020 2020  hod="post">.    
-00000540: 2020 2020 7b25 2063 7372 665f 746f 6b65      {% csrf_toke
-00000550: 6e20 257d 0a20 2020 2020 2020 207b 7b20  n %}.        {{ 
-00000560: 666f 726d 2e6e 6f6e 5f66 6965 6c64 5f65  form.non_field_e
-00000570: 7272 6f72 7320 7d7d 0a0a 2020 2020 2020  rrors }}..      
-00000580: 2020 3c64 6976 2063 6c61 7373 3d22 726f    <div class="ro
-00000590: 7720 666f 726d 2d2d 726f 7722 3e0a 0a20  w form--row">.. 
-000005a0: 2020 2020 2020 207b 2520 6966 206e 6f74         {% if not
-000005b0: 2075 7365 722e 6e65 775f 7374 7564 656e   user.new_studen
-000005c0: 742e 636c 6173 735f 6669 656c 6420 257d  t.class_field %}
-000005d0: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
-000005e0: 7620 636c 6173 733d 2266 6f72 6d2d 2d72  v class="form--r
-000005f0: 6f77 5f5f 696e 7075 7420 636f 6c2d 6d64  ow__input col-md
-00000600: 2d36 223e 0a20 2020 2020 2020 2020 2020  -6">.           
-00000610: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00000620: 2269 6e70 7574 2d2d 6963 6f6e 223e 0a20  "input--icon">. 
-00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000640: 2020 207b 7b20 666f 726d 2e6e 616d 6520     {{ form.name 
-00000650: 7d7d 0a20 2020 2020 2020 2020 2020 2020  }}.             
-00000660: 2020 2020 2020 203c 7370 616e 2063 6c61         <span cla
-00000670: 7373 3d22 6963 6f6e 6966 7922 2064 6174  ss="iconify" dat
-00000680: 612d 6963 6f6e 3d22 6d64 693a 6163 636f  a-icon="mdi:acco
-00000690: 756e 742d 6f75 746c 696e 6522 3e3c 2f73  unt-outline"></s
-000006a0: 7061 6e3e 0a20 2020 2020 2020 2020 2020  pan>.           
-000006b0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-000006c0: 2020 2020 2020 2020 2020 2020 3c73 6d61              <sma
-000006d0: 6c6c 3e7b 7b20 666f 726d 2e6e 616d 652e  ll>{{ form.name.
-000006e0: 6865 6c70 5f74 6578 7420 7d7d 3c2f 736d  help_text }}</sm
-000006f0: 616c 6c3e 0a20 2020 2020 2020 2020 2020  all>.           
-00000700: 2020 2020 207b 7b20 666f 726d 2e6e 616d       {{ form.nam
-00000710: 652e 6572 726f 7273 207d 7d0a 2020 2020  e.errors }}.    
-00000720: 2020 2020 2020 2020 3c2f 6469 763e 0a0a          </div>..
-00000730: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00000740: 2063 6c61 7373 3d22 666f 726d 2d2d 726f   class="form--ro
-00000750: 775f 5f69 6e70 7574 2063 6f6c 2d6d 642d  w__input col-md-
-00000760: 3622 3e0a 2020 2020 2020 2020 2020 2020  6">.            
-00000770: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00000780: 696e 7075 742d 2d69 636f 6e22 3e0a 2020  input--icon">.  
-00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007a0: 2020 7b7b 2066 6f72 6d2e 656d 6169 6c20    {{ form.email 
-000007b0: 7d7d 0a20 2020 2020 2020 2020 2020 2020  }}.             
-000007c0: 2020 2020 2020 203c 7370 616e 2063 6c61         <span cla
-000007d0: 7373 3d22 6963 6f6e 6966 7922 2064 6174  ss="iconify" dat
-000007e0: 612d 6963 6f6e 3d22 6d64 693a 656d 6169  a-icon="mdi:emai
-000007f0: 6c2d 6f75 746c 696e 6522 3e3c 2f73 7061  l-outline"></spa
-00000800: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
-00000810: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00000820: 2020 2020 2020 2020 2020 3c73 6d61 6c6c            <small
-00000830: 3e7b 7b20 666f 726d 2e65 6d61 696c 2e68  >{{ form.email.h
-00000840: 656c 705f 7465 7874 207d 7d3c 2f73 6d61  elp_text }}</sma
-00000850: 6c6c 3e0a 2020 2020 2020 2020 2020 2020  ll>.            
-00000860: 2020 2020 7b7b 2066 6f72 6d2e 656d 6169      {{ form.emai
-00000870: 6c2e 6572 726f 7273 207d 7d0a 2020 2020  l.errors }}.    
-00000880: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000890: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-000008a0: 257d 0a0a 2020 2020 2020 2020 2020 2020  %}..            
-000008b0: 3c64 6976 2063 6c61 7373 3d22 666f 726d  <div class="form
-000008c0: 2d2d 726f 775f 5f69 6e70 7574 2063 6f6c  --row__input col
-000008d0: 2d6d 642d 3422 3e0a 2020 2020 2020 2020  -md-4">.        
-000008e0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000008f0: 7373 3d22 696e 7075 742d 2d69 636f 6e22  ss="input--icon"
-00000900: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000910: 2020 2020 2020 7b7b 2066 6f72 6d2e 7061        {{ form.pa
-00000920: 7373 776f 7264 207d 7d0a 2020 2020 2020  ssword }}.      
-00000930: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00000940: 7061 6e20 636c 6173 733d 2269 636f 6e69  pan class="iconi
-00000950: 6679 2220 6461 7461 2d69 636f 6e3d 226d  fy" data-icon="m
-00000960: 6469 3a73 6563 7572 6974 7922 3e3c 2f73  di:security"></s
-00000970: 7061 6e3e 0a20 2020 2020 2020 2020 2020  pan>.           
-00000980: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000990: 2020 2020 2020 2020 2020 2020 3c73 6d61              <sma
-000009a0: 6c6c 3e7b 7b20 666f 726d 2e70 6173 7377  ll>{{ form.passw
-000009b0: 6f72 642e 6865 6c70 5f74 6578 7420 7d7d  ord.help_text }}
-000009c0: 3c2f 736d 616c 6c3e 0a20 2020 2020 2020  </small>.       
-000009d0: 2020 2020 2020 2020 207b 7b20 666f 726d           {{ form
-000009e0: 2e70 6173 7377 6f72 642e 6572 726f 7273  .password.errors
-000009f0: 207d 7d0a 2020 2020 2020 2020 2020 2020   }}.            
-00000a00: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00000a10: 2020 203c 6469 7620 636c 6173 733d 2266     <div class="f
-00000a20: 6f72 6d2d 2d72 6f77 5f5f 696e 7075 7420  orm--row__input 
-00000a30: 636f 6c2d 6d64 2d34 223e 0a20 2020 2020  col-md-4">.     
-00000a40: 2020 2020 2020 2020 2020 207b 7b20 666f             {{ fo
-00000a50: 726d 2e63 6f6e 6669 726d 5f70 6173 7377  rm.confirm_passw
-00000a60: 6f72 6420 7d7d 0a20 2020 2020 2020 2020  ord }}.         
-00000a70: 2020 2020 2020 203c 736d 616c 6c3e 7b7b         <small>{{
-00000a80: 2066 6f72 6d2e 636f 6e66 6972 6d5f 7061   form.confirm_pa
-00000a90: 7373 776f 7264 2e68 656c 705f 7465 7874  ssword.help_text
-00000aa0: 207d 7d3c 2f73 6d61 6c6c 3e0a 2020 2020   }}</small>.    
-00000ab0: 2020 2020 2020 2020 2020 2020 7b7b 2066              {{ f
-00000ac0: 6f72 6d2e 636f 6e66 6972 6d5f 7061 7373  orm.confirm_pass
-00000ad0: 776f 7264 2e65 7272 6f72 7320 7d7d 0a20  word.errors }}. 
-00000ae0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00000af0: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
-00000b00: 6976 2063 6c61 7373 3d22 666f 726d 2d2d  iv class="form--
-00000b10: 726f 775f 5f69 6e70 7574 2063 6f6c 2d6d  row__input col-m
-00000b20: 642d 3422 3e0a 2020 2020 2020 2020 2020  d-4">.          
-00000b30: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00000b40: 3d22 696e 7075 742d 2d69 636f 6e22 3e0a  ="input--icon">.
-00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b60: 2020 2020 7b7b 2066 6f72 6d2e 6375 7272      {{ form.curr
-00000b70: 656e 745f 7061 7373 776f 7264 207d 7d0a  ent_password }}.
-00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b90: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
-00000ba0: 2269 636f 6e69 6679 2220 6461 7461 2d69  "iconify" data-i
-00000bb0: 636f 6e3d 226d 6469 3a73 6563 7572 6974  con="mdi:securit
-00000bc0: 7922 3e3c 2f73 7061 6e3e 0a20 2020 2020  y"></span>.     
-00000bd0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00000be0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000bf0: 2020 3c73 6d61 6c6c 3e7b 7b20 666f 726d    <small>{{ form
-00000c00: 2e63 7572 7265 6e74 5f70 6173 7377 6f72  .current_passwor
-00000c10: 642e 6865 6c70 5f74 6578 7420 7d7d 3c2f  d.help_text }}</
-00000c20: 736d 616c 6c3e 0a20 2020 2020 2020 2020  small>.         
-00000c30: 2020 2020 2020 207b 7b20 666f 726d 2e63         {{ form.c
-00000c40: 7572 7265 6e74 5f70 6173 7377 6f72 642e  urrent_password.
-00000c50: 6572 726f 7273 207d 7d0a 2020 2020 2020  errors }}.      
-00000c60: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00000c70: 2020 2020 203c 2f64 6976 3e0a 0a20 2020       </div>..   
-00000c80: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00000c90: 2272 6f77 2d2d 756e 6465 7222 3e0a 2020  "row--under">.  
-00000ca0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00000cb0: 6c61 7373 3d22 7061 7373 776f 7264 2d73  lass="password-s
-00000cc0: 7472 656e 6774 682d 636f 6e74 6169 6e65  trength-containe
-00000cd0: 7222 3e0a 2020 2020 2020 2020 2020 2020  r">.            
-00000ce0: 2020 2020 3c64 6976 2069 643d 2273 7475      <div id="stu
-00000cf0: 6465 6e74 2d70 6173 7377 6f72 642d 7369  dent-password-si
-00000d00: 676e 2220 636c 6173 733d 2270 6173 7377  gn" class="passw
-00000d10: 6f72 642d 7374 7265 6e67 7468 2d73 6967  ord-strength-sig
-00000d20: 6e22 3e3c 2f64 6976 3e0a 2020 2020 2020  n"></div>.      
-00000d30: 2020 2020 2020 2020 2020 3c64 6976 2069            <div i
-00000d40: 643d 2273 7475 6465 6e74 2d70 6173 7377  d="student-passw
-00000d50: 6f72 642d 7465 7874 2220 636c 6173 733d  ord-text" class=
-00000d60: 2270 6173 7377 6f72 642d 7374 7265 6e67  "password-streng
-00000d70: 7468 2d74 6578 7422 3e3c 2f64 6976 3e0a  th-text"></div>.
-00000d80: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00000d90: 763e 0a20 2020 2020 2020 203c 2f64 6976  v>.        </div
-00000da0: 3e0a 0a20 2020 2020 2020 203c 6469 7620  >..        <div 
-00000db0: 636c 6173 733d 2262 7574 746f 6e2d 6772  class="button-gr
-00000dc0: 6f75 7022 3e0a 2020 2020 2020 2020 2020  oup">.          
-00000dd0: 2020 3c61 2069 643d 2263 616e 6365 6c5f    <a id="cancel_
-00000de0: 6275 7474 6f6e 2220 636c 6173 733d 2262  button" class="b
-00000df0: 7574 746f 6e20 6275 7474 6f6e 2d2d 7365  utton button--se
-00000e00: 636f 6e64 6172 7920 6275 7474 6f6e 2d2d  condary button--
-00000e10: 7365 636f 6e64 6172 792d 2d64 6172 6b22  secondary--dark"
-00000e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e30: 207b 2520 6966 2075 7365 722e 6e65 775f   {% if user.new_
-00000e40: 7374 7564 656e 742e 636c 6173 735f 6669  student.class_fi
-00000e50: 656c 6420 257d 0a20 2020 2020 2020 2020  eld %}.         
-00000e60: 2020 2020 2020 2020 2020 2068 7265 663d             href=
-00000e70: 227b 2520 7572 6c20 2773 7475 6465 6e74  "{% url 'student
-00000e80: 5f64 6574 6169 6c73 2720 257d 220a 2020  _details' %}".  
-00000e90: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000ea0: 2065 6c73 6520 257d 0a20 2020 2020 2020   else %}.       
-00000eb0: 2020 2020 2020 2020 2020 2020 2068 7265               hre
-00000ec0: 663d 227b 2520 7572 6c20 2769 6e64 6570  f="{% url 'indep
-00000ed0: 656e 6465 6e74 5f73 7475 6465 6e74 5f64  endent_student_d
-00000ee0: 6574 6169 6c73 2720 257d 220a 2020 2020  etails' %}".    
-00000ef0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-00000f00: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
-00000f10: 2020 2020 3e43 616e 6365 6c3c 2f61 3e0a      >Cancel</a>.
-00000f20: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
-00000f30: 746f 6e20 6964 3d22 7570 6461 7465 5f62  ton id="update_b
-00000f40: 7574 746f 6e22 2074 7970 653d 2273 7562  utton" type="sub
-00000f50: 6d69 7422 2063 6c61 7373 3d22 6275 7474  mit" class="butt
-00000f60: 6f6e 2062 7574 746f 6e2d 2d70 7269 6d61  on button--prima
-00000f70: 7279 2220 7661 6c75 653d 2255 7064 6174  ry" value="Updat
-00000f80: 6522 2f3e 0a20 2020 2020 2020 2020 2020  e"/>.           
-00000f90: 2020 2020 2055 7064 6174 6520 6465 7461       Update deta
-00000fa0: 696c 733c 2f62 7574 746f 6e3e 0a20 2020  ils</button>.   
-00000fb0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000fc0: 3c2f 666f 726d 3e0a 3c2f 6469 763e 0a0a  </form>.</div>..
-00000fd0: 7b25 2069 6620 6e6f 7420 7573 6572 2e6e  {% if not user.n
-00000fe0: 6577 5f73 7475 6465 6e74 2e63 6c61 7373  ew_student.class
-00000ff0: 5f66 6965 6c64 2025 7d0a 3c64 6976 2063  _field %}.<div c
-00001000: 6c61 7373 3d22 6261 636b 6772 6f75 6e64  lass="background
-00001010: 2062 6163 6b67 726f 756e 642d 2d70 7269   background--pri
-00001020: 6d61 7279 223e 0a20 2020 203c 6469 7620  mary">.    <div 
-00001030: 636c 6173 733d 2263 6f6e 7461 696e 6572  class="container
-00001040: 223e 0a20 2020 2020 2020 203c 6835 3e4a  ">.        <h5>J
-00001050: 6f69 6e20 6120 7363 686f 6f6c 206f 7220  oin a school or 
-00001060: 636c 7562 3c2f 6835 3e0a 2020 2020 2020  club</h5>.      
-00001070: 2020 3c70 3e54 6f20 6669 6e64 206f 7574    <p>To find out
-00001080: 2061 626f 7574 206c 696e 6b69 6e67 2079   about linking y
-00001090: 6f75 7220 436f 6465 2046 6f72 204c 6966  our Code For Lif
-000010a0: 6520 6163 636f 756e 7420 7769 7468 2061  e account with a
-000010b0: 2073 6368 6f6f 6c20 6f72 2063 6c75 622c   school or club,
-000010c0: 2063 6c69 636b 2027 4a6f 696e 272e 3c2f   click 'Join'.</
-000010d0: 703e 0a20 2020 2020 2020 203c 6120 636c  p>.        <a cl
-000010e0: 6173 733d 2262 7574 746f 6e20 6275 7474  ass="button butt
-000010f0: 6f6e 2d2d 7072 696d 6172 7922 2068 7265  on--primary" hre
-00001100: 663d 227b 2520 7572 6c20 2773 7475 6465  f="{% url 'stude
-00001110: 6e74 5f6a 6f69 6e5f 6f72 6761 6e69 7361  nt_join_organisa
-00001120: 7469 6f6e 2720 257d 223e 4a6f 696e 3c2f  tion' %}">Join</
-00001130: 613e 0a20 2020 203c 2f64 6976 3e0a 3c2f  a>.    </div>.</
-00001140: 6469 763e 0a3c 6469 7620 6964 3d22 6465  div>.<div id="de
-00001150: 6c65 7465 2d69 6e64 792d 6163 636f 756e  lete-indy-accoun
-00001160: 7422 2063 6c61 7373 3d22 6261 636b 6772  t" class="backgr
-00001170: 6f75 6e64 223e 0a20 2020 203c 6469 7620  ound">.    <div 
-00001180: 636c 6173 733d 2263 6f6e 7461 696e 6572  class="container
-00001190: 223e 0a20 2020 2020 2020 203c 6835 3e44  ">.        <h5>D
-000011a0: 656c 6574 6520 6163 636f 756e 743c 2f68  elete account</h
-000011b0: 353e 0a20 2020 2020 2020 203c 703e 4966  5>.        <p>If
-000011c0: 2079 6f75 206e 6f20 6c6f 6e67 6572 2077   you no longer w
-000011d0: 6973 6820 746f 2068 6176 6520 6120 436f  ish to have a Co
-000011e0: 6465 2066 6f72 204c 6966 6520 6163 636f  de for Life acco
-000011f0: 756e 742c 2079 6f75 2063 616e 2064 656c  unt, you can del
-00001200: 6574 6520 6974 2062 7920 636f 6e66 6972  ete it by confir
-00001210: 6d69 6e67 2062 656c 6f77 2e0a 2020 2020  ming below..    
-00001220: 2020 2020 2020 2020 596f 7520 7769 6c6c          You will
-00001230: 2072 6563 6569 7665 2061 6e20 656d 6169   receive an emai
-00001240: 6c20 746f 2063 6f6e 6669 726d 2074 6869  l to confirm thi
-00001250: 7320 6465 6369 7369 6f6e 2e0a 2020 2020  s decision..    
-00001260: 2020 2020 3c2f 703e 0a20 2020 2020 2020      </p>.       
-00001270: 203c 703e 3c62 3e54 6869 7320 6361 6e27   <p><b>This can'
-00001280: 7420 6265 2072 6576 6572 7365 642e 3c2f  t be reversed.</
-00001290: 623e 0a20 2020 2020 2020 203c 2f70 3e0a  b>.        </p>.
-000012a0: 0a20 2020 2020 2020 203c 666f 726d 206d  .        <form m
-000012b0: 6574 686f 643d 2270 6f73 7422 2069 643d  ethod="post" id=
-000012c0: 2266 6f72 6d2d 6465 6c65 7465 2d69 6e64  "form-delete-ind
-000012d0: 792d 6163 636f 756e 7422 3e0a 0a20 2020  y-account">..   
-000012e0: 2020 2020 207b 2520 6373 7266 5f74 6f6b       {% csrf_tok
-000012f0: 656e 2025 7d0a 0a20 2020 2020 2020 207b  en %}..        {
-00001300: 7b20 6465 6c65 7465 5f61 6363 6f75 6e74  { delete_account
-00001310: 5f66 6f72 6d2e 6e6f 6e5f 6669 656c 645f  _form.non_field_
-00001320: 6572 726f 7273 207d 7d0a 0a20 2020 2020  errors }}..     
-00001330: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
-00001340: 6f77 2066 6f72 6d2d 2d72 6f77 223e 0a20  ow form--row">. 
-00001350: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00001360: 636c 6173 733d 2266 6f72 6d2d 2d72 6f77  class="form--row
-00001370: 5f5f 696e 7075 7420 636f 6c2d 736d 2d36  __input col-sm-6
-00001380: 2063 6f6c 2d6d 642d 3422 3e0a 2020 2020   col-md-4">.    
-00001390: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-000013a0: 2063 6c61 7373 3d22 696e 7075 742d 2d69   class="input--i
-000013b0: 636f 6e22 3e0a 2020 2020 2020 2020 2020  con">.          
-000013c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000013d0: 7b20 6465 6c65 7465 5f61 6363 6f75 6e74  { delete_account
-000013e0: 5f66 6f72 6d2e 6465 6c65 7465 5f70 6173  _form.delete_pas
-000013f0: 7377 6f72 6420 7d7d 0a20 2020 2020 2020  sword }}.       
-00001400: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
-00001410: 616e 2063 6c61 7373 3d22 6963 6f6e 6966  an class="iconif
-00001420: 7922 2064 6174 612d 6963 6f6e 3d22 6d64  y" data-icon="md
-00001430: 693a 7365 6375 7269 7479 223e 3c2f 7370  i:security"></sp
-00001440: 616e 3e0a 2020 2020 2020 2020 2020 2020  an>.            
-00001450: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00001460: 2020 2020 2020 2020 2020 203c 736d 616c             <smal
-00001470: 6c3e 7b7b 2064 656c 6574 655f 6163 636f  l>{{ delete_acco
-00001480: 756e 745f 666f 726d 2e64 656c 6574 655f  unt_form.delete_
-00001490: 7061 7373 776f 7264 2e68 656c 705f 7465  password.help_te
-000014a0: 7874 207d 7d3c 2f73 6d61 6c6c 3e0a 2020  xt }}</small>.  
-000014b0: 2020 2020 2020 2020 2020 2020 2020 7b7b                {{
-000014c0: 2064 656c 6574 655f 6163 636f 756e 745f   delete_account_
-000014d0: 666f 726d 2e64 656c 6574 655f 7061 7373  form.delete_pass
-000014e0: 776f 7264 2e65 7272 6f72 7320 7d7d 0a20  word.errors }}. 
-000014f0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00001500: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
-00001510: 6976 2063 6c61 7373 3d22 666f 726d 2d2d  iv class="form--
-00001520: 726f 775f 5f69 6e70 7574 2063 6f6c 2d73  row__input col-s
-00001530: 6d2d 3620 636f 6c2d 6d64 2d38 223e 0a20  m-6 col-md-8">. 
-00001540: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001550: 6469 7620 636c 6173 733d 2266 6f72 6d5f  div class="form_
-00001560: 5f63 6865 636b 626f 7822 3e0a 2020 2020  _checkbox">.    
-00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001580: 3c64 6976 2063 6c61 7373 3d22 666f 726d  <div class="form
-00001590: 5f5f 6368 6563 6b62 6f78 2d69 6e70 7574  __checkbox-input
-000015a0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000015b0: 2020 2020 2020 2020 2020 207b 7b20 6465             {{ de
-000015c0: 6c65 7465 5f61 6363 6f75 6e74 5f66 6f72  lete_account_for
-000015d0: 6d2e 756e 7375 6273 6372 6962 655f 6e65  m.unsubscribe_ne
-000015e0: 7773 6c65 7474 6572 207d 7d0a 2020 2020  wsletter }}.    
-000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00001610: 2020 2020 2020 2020 2020 203c 6c61 6265             <labe
-00001620: 6c20 666f 723d 2269 645f 7b7b 2064 656c  l for="id_{{ del
-00001630: 6574 655f 6163 636f 756e 745f 666f 726d  ete_account_form
-00001640: 2e75 6e73 7562 7363 7269 6265 5f6e 6577  .unsubscribe_new
-00001650: 736c 6574 7465 722e 6874 6d6c 5f6e 616d  sletter.html_nam
-00001660: 6520 7d7d 223e 7b7b 2064 656c 6574 655f  e }}">{{ delete_
-00001670: 6163 636f 756e 745f 666f 726d 2e75 6e73  account_form.uns
-00001680: 7562 7363 7269 6265 5f6e 6577 736c 6574  ubscribe_newslet
-00001690: 7465 722e 6c61 6265 6c20 7d7d 3c2f 6c61  ter.label }}</la
-000016a0: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
-000016b0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-000016c0: 2020 2020 2020 2020 2020 2020 7b7b 2064              {{ d
-000016d0: 656c 6574 655f 6163 636f 756e 745f 666f  elete_account_fo
-000016e0: 726d 2e75 6e73 7562 7363 7269 6265 5f6e  rm.unsubscribe_n
-000016f0: 6577 736c 6574 7465 722e 6572 726f 7273  ewsletter.errors
-00001700: 207d 7d0a 2020 2020 2020 2020 2020 2020   }}.            
-00001710: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
-00001720: 2f64 6976 3e0a 2020 2020 2020 2020 3c62  /div>.        <b
-00001730: 7574 746f 6e20 6964 3d22 6465 6c65 7465  utton id="delete
-00001740: 5f61 6363 6f75 6e74 5f62 7574 746f 6e22  _account_button"
-00001750: 2063 6c61 7373 3d22 6275 7474 6f6e 2062   class="button b
-00001760: 7574 746f 6e2d 2d70 7269 6d61 7279 2062  utton--primary b
-00001770: 7574 746f 6e2d 2d70 7269 6d61 7279 2d2d  utton--primary--
-00001780: 6461 6e67 6572 2062 7574 746f 6e2d 2d69  danger button--i
-00001790: 636f 6e22 206e 616d 653d 2264 656c 6574  con" name="delet
-000017a0: 655f 6163 636f 756e 7422 3e0a 2020 2020  e_account">.    
-000017b0: 2020 2020 2020 2020 4465 6c65 7465 2061          Delete a
-000017c0: 6363 6f75 6e74 203c 7370 616e 2063 6c61  ccount <span cla
-000017d0: 7373 3d22 6963 6f6e 6966 7922 2064 6174  ss="iconify" dat
-000017e0: 612d 6963 6f6e 3d22 6d64 693a 6465 6c65  a-icon="mdi:dele
-000017f0: 7465 2d6f 7574 6c69 6e65 223e 3c2f 7370  te-outline"></sp
-00001800: 616e 3e0a 2020 2020 2020 2020 3c2f 6275  an>.        </bu
-00001810: 7474 6f6e 3e0a 2020 2020 2020 2020 3c2f  tton>.        </
-00001820: 666f 726d 3e0a 2020 2020 3c2f 6469 763e  form>.    </div>
-00001830: 0a3c 2f64 6976 3e0a 7b25 2065 6e64 6966  .</div>.{% endif
-00001840: 2025 7d0a 0a3c 7363 7269 7074 2074 7970   %}..<script typ
-00001850: 653d 2274 6578 742f 6a61 7661 7363 7269  e="text/javascri
-00001860: 7074 2220 7372 633d 227b 2520 7374 6174  pt" src="{% stat
-00001870: 6963 2027 706f 7274 616c 2f6a 732f 7061  ic 'portal/js/pa
-00001880: 7373 776f 7264 5374 7265 6e67 7468 2e6a  sswordStrength.j
-00001890: 7327 2025 7d22 3e3c 2f73 6372 6970 743e  s' %}"></script>
-000018a0: 0a3c 7363 7269 7074 3e0a 2020 2020 7661  .<script>.    va
-000018b0: 7220 494e 4445 505f 5354 5544 454e 545f  r INDEP_STUDENT_
-000018c0: 5041 5353 574f 5244 5f46 4945 4c44 5f49  PASSWORD_FIELD_I
-000018d0: 4420 3d20 277b 7b20 666f 726d 2e70 6173  D = '{{ form.pas
-000018e0: 7377 6f72 642e 6175 746f 5f69 6420 7d7d  sword.auto_id }}
-000018f0: 273b 0a3c 2f73 6372 6970 743e 0a0a 7b25  ';.</script>..{%
-00001900: 2065 6e64 626c 6f63 6b20 257d 0a          endblock %}.
+000001b0: 626c 6f63 6b20 7363 7269 7074 7320 257d  block scripts %}
+000001c0: 0a7b 7b20 626c 6f63 6b2e 7375 7065 7220  .{{ block.super 
+000001d0: 7d7d 0a3c 7363 7269 7074 2074 7970 653d  }}.<script type=
+000001e0: 2274 6578 742f 6a61 7661 7363 7269 7074  "text/javascript
+000001f0: 2220 7372 633d 227b 2520 7374 6174 6963  " src="{% static
+00000200: 2027 706f 7274 616c 2f6a 732f 6f72 6761   'portal/js/orga
+00000210: 6e69 7361 7469 6f6e 5f6d 616e 6167 652e  nisation_manage.
+00000220: 6a73 2720 257d 223e 3c2f 7363 7269 7074  js' %}"></script
+00000230: 3e0a 2020 2020 3c73 6372 6970 7420 7479  >.    <script ty
+00000240: 7065 3d22 7465 7874 2f6a 6176 6173 6372  pe="text/javascr
+00000250: 6970 7422 2073 7263 3d22 7b25 2073 7461  ipt" src="{% sta
+00000260: 7469 6320 2770 6f72 7461 6c2f 6a73 2f70  tic 'portal/js/p
+00000270: 6173 7377 6f72 6453 7472 656e 6774 682e  asswordStrength.
+00000280: 6a73 2720 257d 223e 3c2f 7363 7269 7074  js' %}"></script
+00000290: 3e0a 2020 2020 3c73 6372 6970 743e 0a20  >.    <script>. 
+000002a0: 2020 2020 2020 2076 6172 2049 4e44 4550         var INDEP
+000002b0: 5f53 5455 4445 4e54 5f50 4153 5357 4f52  _STUDENT_PASSWOR
+000002c0: 445f 4649 454c 445f 4944 203d 2027 7b7b  D_FIELD_ID = '{{
+000002d0: 2066 6f72 6d2e 7061 7373 776f 7264 2e61   form.password.a
+000002e0: 7574 6f5f 6964 207d 7d27 3b0a 2020 2020  uto_id }}';.    
+000002f0: 3c2f 7363 7269 7074 3e0a 2020 2020 3c73  </script>.    <s
+00000300: 6372 6970 743e 0a20 2020 2020 2020 207b  cript>.        {
+00000310: 2520 6966 2064 656c 6574 655f 6163 636f  % if delete_acco
+00000320: 756e 745f 636f 6e66 6972 6d20 257d 0a20  unt_confirm %}. 
+00000330: 2020 2020 2020 2020 2020 2073 686f 7744             showD
+00000340: 656c 6574 6541 6363 6f75 6e74 436f 6e66  eleteAccountConf
+00000350: 6972 6d61 7469 6f6e 2822 7b7b 2064 656c  irmation("{{ del
+00000360: 6574 655f 6163 636f 756e 745f 666f 726d  ete_account_form
+00000370: 2e64 656c 6574 655f 7061 7373 776f 7264  .delete_password
+00000380: 2e76 616c 7565 207d 7d22 2c20 227b 7b20  .value }}", "{{ 
+00000390: 6465 6c65 7465 5f61 6363 6f75 6e74 5f66  delete_account_f
+000003a0: 6f72 6d2e 756e 7375 6273 6372 6962 655f  orm.unsubscribe_
+000003b0: 6e65 7773 6c65 7474 6572 2e76 616c 7565  newsletter.value
+000003c0: 207d 7d22 2c20 6661 6c73 6529 0a20 2020   }}", false).   
+000003d0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+000003e0: 0a20 2020 203c 2f73 6372 6970 743e 0a7b  .    </script>.{
+000003f0: 2520 656e 6462 6c6f 636b 2073 6372 6970  % endblock scrip
+00000400: 7473 2025 7d0a 0a7b 2520 626c 6f63 6b20  ts %}..{% block 
+00000410: 636f 6e74 656e 7420 257d 0a7b 2520 696e  content %}.{% in
+00000420: 636c 7564 6520 2270 6f72 7461 6c2f 7061  clude "portal/pa
+00000430: 7274 6961 6c73 2f64 656c 6574 655f 706f  rtials/delete_po
+00000440: 7075 702e 6874 6d6c 2220 257d 0a0a 3c64  pup.html" %}..<d
+00000450: 6976 2069 643d 2270 6c61 795f 6163 636f  iv id="play_acco
+00000460: 756e 745f 7061 6765 223e 3c2f 6469 763e  unt_page"></div>
+00000470: 0a3c 6469 7620 636c 6173 733d 2262 6163  .<div class="bac
+00000480: 6b67 726f 756e 6420 636f 6e74 6169 6e65  kground containe
+00000490: 7222 3e0a 2020 2020 3c73 6563 7469 6f6e  r">.    <section
+000004a0: 3e3c 6834 3e0a 2020 2020 2020 2020 7b25  ><h4>.        {%
+000004b0: 2069 6620 7573 6572 2e6e 6577 5f73 7475   if user.new_stu
+000004c0: 6465 6e74 2e63 6c61 7373 5f66 6965 6c64  dent.class_field
+000004d0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000004e0: 5570 6461 7465 2079 6f75 7220 7061 7373  Update your pass
+000004f0: 776f 7264 0a20 2020 2020 2020 207b 2520  word.        {% 
+00000500: 656c 7365 2025 7d0a 2020 2020 2020 2020  else %}.        
+00000510: 2020 2020 5570 6461 7465 2079 6f75 7220      Update your 
+00000520: 6163 636f 756e 7420 6465 7461 696c 730a  account details.
+00000530: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+00000540: 2025 7d0a 2020 2020 3c2f 6834 3e3c 2f73   %}.    </h4></s
+00000550: 6563 7469 6f6e 3e0a 0a20 2020 207b 2520  ection>..    {% 
+00000560: 6966 2075 7365 722e 6e65 775f 7374 7564  if user.new_stud
+00000570: 656e 742e 636c 6173 735f 6669 656c 6420  ent.class_field 
+00000580: 257d 0a20 2020 2020 2020 203c 703e 596f  %}.        <p>Yo
+00000590: 7520 6d61 7920 6564 6974 2079 6f75 7220  u may edit your 
+000005a0: 7061 7373 776f 7264 2062 656c 6f77 2e20  password below. 
+000005b0: 4974 206d 7573 7420 6265 206c 6f6e 6720  It must be long 
+000005c0: 656e 6f75 6768 2061 6e64 2068 6172 6420  enough and hard 
+000005d0: 656e 6f75 6768 2074 6f20 7374 6f70 2079  enough to stop y
+000005e0: 6f75 7220 6672 6965 6e64 7320 6775 6573  our friends gues
+000005f0: 7369 6e67 2069 7420 616e 640a 2020 2020  sing it and.    
+00000600: 2020 2020 2020 2020 7374 6561 6c69 6e67          stealing
+00000610: 2061 6c6c 206f 6620 796f 7572 2068 6172   all of your har
+00000620: 6420 776f 726b 2e20 4368 6f6f 7365 2073  d work. Choose s
+00000630: 6f6d 6574 6869 6e67 206d 656d 6f72 6162  omething memorab
+00000640: 6c65 2074 686f 7567 682e 3c2f 703e 0a20  le though.</p>. 
+00000650: 2020 2020 2020 203c 703e 4966 2079 6f75         <p>If you
+00000660: 2068 6176 6520 616e 7920 7072 6f62 6c65   have any proble
+00000670: 6d73 2c20 6173 6b20 6120 7465 6163 6865  ms, ask a teache
+00000680: 7220 746f 2068 656c 7020 796f 752e 3c2f  r to help you.</
+00000690: 703e 0a20 2020 207b 2520 656c 7365 2025  p>.    {% else %
+000006a0: 7d0a 2020 2020 2020 2020 3c70 3e59 6f75  }.        <p>You
+000006b0: 2063 616e 2075 7064 6174 6520 796f 7572   can update your
+000006c0: 2061 6363 6f75 6e74 2064 6574 6169 6c73   account details
+000006d0: 2062 656c 6f77 2e3c 2f70 3e0a 2020 2020   below.</p>.    
+000006e0: 2020 2020 3c70 3e50 6c65 6173 6520 6e6f      <p>Please no
+000006f0: 7465 3a20 4966 2079 6f75 2063 6861 6e67  te: If you chang
+00000700: 6520 796f 7572 2065 6d61 696c 2061 6464  e your email add
+00000710: 7265 7373 2c20 796f 7520 7769 6c6c 206e  ress, you will n
+00000720: 6565 6420 746f 2072 652d 7665 7269 6679  eed to re-verify
+00000730: 2069 742e 3c2f 6272 3e0a 2020 2020 2020   it.</br>.      
+00000740: 2020 2020 2020 506c 6561 7365 2065 6e73        Please ens
+00000750: 7572 6520 796f 7572 2070 6173 7377 6f72  ure your passwor
+00000760: 6420 6973 2073 7472 6f6e 6720 656e 6f75  d is strong enou
+00000770: 6768 2074 6f20 6265 2073 6563 7572 652e  gh to be secure.
+00000780: 3c2f 703e 0a20 2020 207b 2520 656e 6469  </p>.    {% endi
+00000790: 6620 257d 0a0a 2020 2020 3c66 6f72 6d20  f %}..    <form 
+000007a0: 6964 3d22 7374 7564 656e 745f 6163 636f  id="student_acco
+000007b0: 756e 745f 666f 726d 2220 6d65 7468 6f64  unt_form" method
+000007c0: 3d22 706f 7374 223e 0a20 2020 2020 2020  ="post">.       
+000007d0: 207b 2520 6373 7266 5f74 6f6b 656e 2025   {% csrf_token %
+000007e0: 7d0a 2020 2020 2020 2020 7b7b 2066 6f72  }.        {{ for
+000007f0: 6d2e 6e6f 6e5f 6669 656c 645f 6572 726f  m.non_field_erro
+00000800: 7273 207d 7d0a 0a20 2020 2020 2020 203c  rs }}..        <
+00000810: 6469 7620 636c 6173 733d 2272 6f77 2066  div class="row f
+00000820: 6f72 6d2d 2d72 6f77 223e 0a0a 2020 2020  orm--row">..    
+00000830: 2020 2020 7b25 2069 6620 6e6f 7420 7573      {% if not us
+00000840: 6572 2e6e 6577 5f73 7475 6465 6e74 2e63  er.new_student.c
+00000850: 6c61 7373 5f66 6965 6c64 2025 7d0a 2020  lass_field %}.  
+00000860: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00000870: 6c61 7373 3d22 666f 726d 2d2d 726f 775f  lass="form--row_
+00000880: 5f69 6e70 7574 2063 6f6c 2d6d 642d 3622  _input col-md-6"
+00000890: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000008a0: 2020 3c64 6976 2063 6c61 7373 3d22 696e    <div class="in
+000008b0: 7075 742d 2d69 636f 6e22 3e0a 2020 2020  put--icon">.    
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008d0: 7b7b 2066 6f72 6d2e 6e61 6d65 207d 7d0a  {{ form.name }}.
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008f0: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
+00000900: 2269 636f 6e69 6679 2220 6461 7461 2d69  "iconify" data-i
+00000910: 636f 6e3d 226d 6469 3a61 6363 6f75 6e74  con="mdi:account
+00000920: 2d6f 7574 6c69 6e65 223e 3c2f 7370 616e  -outline"></span
+00000930: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000940: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000950: 2020 2020 2020 2020 203c 736d 616c 6c3e           <small>
+00000960: 7b7b 2066 6f72 6d2e 6e61 6d65 2e68 656c  {{ form.name.hel
+00000970: 705f 7465 7874 207d 7d3c 2f73 6d61 6c6c  p_text }}</small
+00000980: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000990: 2020 7b7b 2066 6f72 6d2e 6e61 6d65 2e65    {{ form.name.e
+000009a0: 7272 6f72 7320 7d7d 0a20 2020 2020 2020  rrors }}.       
+000009b0: 2020 2020 203c 2f64 6976 3e0a 0a20 2020       </div>..   
+000009c0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+000009d0: 6173 733d 2266 6f72 6d2d 2d72 6f77 5f5f  ass="form--row__
+000009e0: 696e 7075 7420 636f 6c2d 6d64 2d36 223e  input col-md-6">
+000009f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a00: 203c 6469 7620 636c 6173 733d 2269 6e70   <div class="inp
+00000a10: 7574 2d2d 6963 6f6e 223e 0a20 2020 2020  ut--icon">.     
+00000a20: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000a30: 7b20 666f 726d 2e65 6d61 696c 207d 7d0a  { form.email }}.
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a50: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
+00000a60: 2269 636f 6e69 6679 2220 6461 7461 2d69  "iconify" data-i
+00000a70: 636f 6e3d 226d 6469 3a65 6d61 696c 2d6f  con="mdi:email-o
+00000a80: 7574 6c69 6e65 223e 3c2f 7370 616e 3e0a  utline"></span>.
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00000ab0: 2020 2020 2020 203c 736d 616c 6c3e 7b7b         <small>{{
+00000ac0: 2066 6f72 6d2e 656d 6169 6c2e 6865 6c70   form.email.help
+00000ad0: 5f74 6578 7420 7d7d 3c2f 736d 616c 6c3e  _text }}</small>
+00000ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000af0: 207b 7b20 666f 726d 2e65 6d61 696c 2e65   {{ form.email.e
+00000b00: 7272 6f72 7320 7d7d 0a20 2020 2020 2020  rrors }}.       
+00000b10: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000b20: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+00000b30: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
+00000b40: 7620 636c 6173 733d 2266 6f72 6d2d 2d72  v class="form--r
+00000b50: 6f77 5f5f 696e 7075 7420 636f 6c2d 6d64  ow__input col-md
+00000b60: 2d34 223e 0a20 2020 2020 2020 2020 2020  -4">.           
+00000b70: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000b80: 2269 6e70 7574 2d2d 6963 6f6e 223e 0a20  "input--icon">. 
+00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ba0: 2020 207b 7b20 666f 726d 2e70 6173 7377     {{ form.passw
+00000bb0: 6f72 6420 7d7d 0a20 2020 2020 2020 2020  ord }}.         
+00000bc0: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+00000bd0: 2063 6c61 7373 3d22 6963 6f6e 6966 7922   class="iconify"
+00000be0: 2064 6174 612d 6963 6f6e 3d22 6d64 693a   data-icon="mdi:
+00000bf0: 7365 6375 7269 7479 223e 3c2f 7370 616e  security"></span
+00000c00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000c10: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000c20: 2020 2020 2020 2020 203c 736d 616c 6c3e           <small>
+00000c30: 7b7b 2066 6f72 6d2e 7061 7373 776f 7264  {{ form.password
+00000c40: 2e68 656c 705f 7465 7874 207d 7d3c 2f73  .help_text }}</s
+00000c50: 6d61 6c6c 3e0a 2020 2020 2020 2020 2020  mall>.          
+00000c60: 2020 2020 2020 7b7b 2066 6f72 6d2e 7061        {{ form.pa
+00000c70: 7373 776f 7264 2e65 7272 6f72 7320 7d7d  ssword.errors }}
+00000c80: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
+00000c90: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00000ca0: 3c64 6976 2063 6c61 7373 3d22 666f 726d  <div class="form
+00000cb0: 2d2d 726f 775f 5f69 6e70 7574 2063 6f6c  --row__input col
+00000cc0: 2d6d 642d 3422 3e0a 2020 2020 2020 2020  -md-4">.        
+00000cd0: 2020 2020 2020 2020 7b7b 2066 6f72 6d2e          {{ form.
+00000ce0: 636f 6e66 6972 6d5f 7061 7373 776f 7264  confirm_password
+00000cf0: 207d 7d0a 2020 2020 2020 2020 2020 2020   }}.            
+00000d00: 2020 2020 3c73 6d61 6c6c 3e7b 7b20 666f      <small>{{ fo
+00000d10: 726d 2e63 6f6e 6669 726d 5f70 6173 7377  rm.confirm_passw
+00000d20: 6f72 642e 6865 6c70 5f74 6578 7420 7d7d  ord.help_text }}
+00000d30: 3c2f 736d 616c 6c3e 0a20 2020 2020 2020  </small>.       
+00000d40: 2020 2020 2020 2020 207b 7b20 666f 726d           {{ form
+00000d50: 2e63 6f6e 6669 726d 5f70 6173 7377 6f72  .confirm_passwor
+00000d60: 642e 6572 726f 7273 207d 7d0a 2020 2020  d.errors }}.    
+00000d70: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000d80: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00000d90: 636c 6173 733d 2266 6f72 6d2d 2d72 6f77  class="form--row
+00000da0: 5f5f 696e 7075 7420 636f 6c2d 6d64 2d34  __input col-md-4
+00000db0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000dc0: 2020 203c 6469 7620 636c 6173 733d 2269     <div class="i
+00000dd0: 6e70 7574 2d2d 6963 6f6e 223e 0a20 2020  nput--icon">.   
+00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000df0: 207b 7b20 666f 726d 2e63 7572 7265 6e74   {{ form.current
+00000e00: 5f70 6173 7377 6f72 6420 7d7d 0a20 2020  _password }}.   
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e20: 203c 7370 616e 2063 6c61 7373 3d22 6963   <span class="ic
+00000e30: 6f6e 6966 7922 2064 6174 612d 6963 6f6e  onify" data-icon
+00000e40: 3d22 6d64 693a 7365 6375 7269 7479 223e  ="mdi:security">
+00000e50: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
+00000e60: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000e70: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000e80: 736d 616c 6c3e 7b7b 2066 6f72 6d2e 6375  small>{{ form.cu
+00000e90: 7272 656e 745f 7061 7373 776f 7264 2e68  rrent_password.h
+00000ea0: 656c 705f 7465 7874 207d 7d3c 2f73 6d61  elp_text }}</sma
+00000eb0: 6c6c 3e0a 2020 2020 2020 2020 2020 2020  ll>.            
+00000ec0: 2020 2020 7b7b 2066 6f72 6d2e 6375 7272      {{ form.curr
+00000ed0: 656e 745f 7061 7373 776f 7264 2e65 7272  ent_password.err
+00000ee0: 6f72 7320 7d7d 0a20 2020 2020 2020 2020  ors }}.         
+00000ef0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000f00: 2020 3c2f 6469 763e 0a0a 2020 2020 2020    </div>..      
+00000f10: 2020 3c64 6976 2063 6c61 7373 3d22 726f    <div class="ro
+00000f20: 772d 2d75 6e64 6572 223e 0a20 2020 2020  w--under">.     
+00000f30: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00000f40: 733d 2270 6173 7377 6f72 642d 7374 7265  s="password-stre
+00000f50: 6e67 7468 2d63 6f6e 7461 696e 6572 223e  ngth-container">
+00000f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000f70: 203c 6469 7620 6964 3d22 7374 7564 656e   <div id="studen
+00000f80: 742d 7061 7373 776f 7264 2d73 6967 6e22  t-password-sign"
+00000f90: 2063 6c61 7373 3d22 7061 7373 776f 7264   class="password
+00000fa0: 2d73 7472 656e 6774 682d 7369 676e 223e  -strength-sign">
+00000fb0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00000fc0: 2020 2020 2020 203c 6469 7620 6964 3d22         <div id="
+00000fd0: 7374 7564 656e 742d 7061 7373 776f 7264  student-password
+00000fe0: 2d74 6578 7422 2063 6c61 7373 3d22 7061  -text" class="pa
+00000ff0: 7373 776f 7264 2d73 7472 656e 6774 682d  ssword-strength-
+00001000: 7465 7874 223e 3c2f 6469 763e 0a20 2020  text"></div>.   
+00001010: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00001020: 2020 2020 2020 2020 3c2f 6469 763e 0a0a          </div>..
+00001030: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00001040: 7373 3d22 6275 7474 6f6e 2d67 726f 7570  ss="button-group
+00001050: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00001060: 6120 6964 3d22 6361 6e63 656c 5f62 7574  a id="cancel_but
+00001070: 746f 6e22 2063 6c61 7373 3d22 6275 7474  ton" class="butt
+00001080: 6f6e 2062 7574 746f 6e2d 2d73 6563 6f6e  on button--secon
+00001090: 6461 7279 2062 7574 746f 6e2d 2d73 6563  dary button--sec
+000010a0: 6f6e 6461 7279 2d2d 6461 726b 220a 2020  ondary--dark".  
+000010b0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000010c0: 2069 6620 7573 6572 2e6e 6577 5f73 7475   if user.new_stu
+000010d0: 6465 6e74 2e63 6c61 7373 5f66 6965 6c64  dent.class_field
+000010e0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000010f0: 2020 2020 2020 2020 6872 6566 3d22 7b25          href="{%
+00001100: 2075 726c 2027 7374 7564 656e 745f 6465   url 'student_de
+00001110: 7461 696c 7327 2025 7d22 0a20 2020 2020  tails' %}".     
+00001120: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+00001130: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
+00001140: 2020 2020 2020 2020 2020 6872 6566 3d22            href="
+00001150: 7b25 2075 726c 2027 696e 6465 7065 6e64  {% url 'independ
+00001160: 656e 745f 7374 7564 656e 745f 6465 7461  ent_student_deta
+00001170: 696c 7327 2025 7d22 0a20 2020 2020 2020  ils' %}".       
+00001180: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
+00001190: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
+000011a0: 203e 4361 6e63 656c 3c2f 613e 0a20 2020   >Cancel</a>.   
+000011b0: 2020 2020 2020 2020 203c 6275 7474 6f6e           <button
+000011c0: 2069 643d 2275 7064 6174 655f 6275 7474   id="update_butt
+000011d0: 6f6e 2220 7479 7065 3d22 7375 626d 6974  on" type="submit
+000011e0: 2220 636c 6173 733d 2262 7574 746f 6e20  " class="button 
+000011f0: 6275 7474 6f6e 2d2d 7072 696d 6172 7922  button--primary"
+00001200: 2076 616c 7565 3d22 5570 6461 7465 222f   value="Update"/
+00001210: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001220: 2020 5570 6461 7465 2064 6574 6169 6c73    Update details
+00001230: 3c2f 6275 7474 6f6e 3e0a 2020 2020 2020  </button>.      
+00001240: 2020 3c2f 6469 763e 0a20 2020 203c 2f66    </div>.    </f
+00001250: 6f72 6d3e 0a3c 2f64 6976 3e0a 0a7b 2520  orm>.</div>..{% 
+00001260: 6966 206e 6f74 2075 7365 722e 6e65 775f  if not user.new_
+00001270: 7374 7564 656e 742e 636c 6173 735f 6669  student.class_fi
+00001280: 656c 6420 257d 0a3c 6469 7620 636c 6173  eld %}.<div clas
+00001290: 733d 2262 6163 6b67 726f 756e 6420 6261  s="background ba
+000012a0: 636b 6772 6f75 6e64 2d2d 7072 696d 6172  ckground--primar
+000012b0: 7922 3e0a 2020 2020 3c64 6976 2063 6c61  y">.    <div cla
+000012c0: 7373 3d22 636f 6e74 6169 6e65 7222 3e0a  ss="container">.
+000012d0: 2020 2020 2020 2020 3c68 353e 4a6f 696e          <h5>Join
+000012e0: 2061 2073 6368 6f6f 6c20 6f72 2063 6c75   a school or clu
+000012f0: 623c 2f68 353e 0a20 2020 2020 2020 203c  b</h5>.        <
+00001300: 703e 546f 2066 696e 6420 6f75 7420 6162  p>To find out ab
+00001310: 6f75 7420 6c69 6e6b 696e 6720 796f 7572  out linking your
+00001320: 2043 6f64 6520 466f 7220 4c69 6665 2061   Code For Life a
+00001330: 6363 6f75 6e74 2077 6974 6820 6120 7363  ccount with a sc
+00001340: 686f 6f6c 206f 7220 636c 7562 2c20 636c  hool or club, cl
+00001350: 6963 6b20 274a 6f69 6e27 2e3c 2f70 3e0a  ick 'Join'.</p>.
+00001360: 2020 2020 2020 2020 3c61 2063 6c61 7373          <a class
+00001370: 3d22 6275 7474 6f6e 2062 7574 746f 6e2d  ="button button-
+00001380: 2d70 7269 6d61 7279 2220 6872 6566 3d22  -primary" href="
+00001390: 7b25 2075 726c 2027 7374 7564 656e 745f  {% url 'student_
+000013a0: 6a6f 696e 5f6f 7267 616e 6973 6174 696f  join_organisatio
+000013b0: 6e27 2025 7d22 3e4a 6f69 6e3c 2f61 3e0a  n' %}">Join</a>.
+000013c0: 2020 2020 3c2f 6469 763e 0a3c 2f64 6976      </div>.</div
+000013d0: 3e0a 3c64 6976 2069 643d 2264 656c 6574  >.<div id="delet
+000013e0: 652d 696e 6479 2d61 6363 6f75 6e74 2220  e-indy-account" 
+000013f0: 636c 6173 733d 2262 6163 6b67 726f 756e  class="backgroun
+00001400: 6422 3e0a 2020 2020 3c64 6976 2063 6c61  d">.    <div cla
+00001410: 7373 3d22 636f 6e74 6169 6e65 7222 3e0a  ss="container">.
+00001420: 2020 2020 2020 2020 3c68 353e 4465 6c65          <h5>Dele
+00001430: 7465 2061 6363 6f75 6e74 3c2f 6835 3e0a  te account</h5>.
+00001440: 2020 2020 2020 2020 3c70 3e49 6620 796f          <p>If yo
+00001450: 7520 6e6f 206c 6f6e 6765 7220 7769 7368  u no longer wish
+00001460: 2074 6f20 6861 7665 2061 2043 6f64 6520   to have a Code 
+00001470: 666f 7220 4c69 6665 2061 6363 6f75 6e74  for Life account
+00001480: 2c20 796f 7520 6361 6e20 6465 6c65 7465  , you can delete
+00001490: 2069 7420 6279 2063 6f6e 6669 726d 696e   it by confirmin
+000014a0: 6720 6265 6c6f 772e 0a20 2020 2020 2020  g below..       
+000014b0: 2020 2020 2059 6f75 2077 696c 6c20 7265       You will re
+000014c0: 6365 6976 6520 616e 2065 6d61 696c 2074  ceive an email t
+000014d0: 6f20 636f 6e66 6972 6d20 7468 6973 2064  o confirm this d
+000014e0: 6563 6973 696f 6e2e 0a20 2020 2020 2020  ecision..       
+000014f0: 203c 2f70 3e0a 2020 2020 2020 2020 3c70   </p>.        <p
+00001500: 3e3c 623e 5468 6973 2063 616e 2774 2062  ><b>This can't b
+00001510: 6520 7265 7665 7273 6564 2e3c 2f62 3e0a  e reversed.</b>.
+00001520: 2020 2020 2020 2020 3c2f 703e 0a0a 2020          </p>..  
+00001530: 2020 2020 2020 3c66 6f72 6d20 6d65 7468        <form meth
+00001540: 6f64 3d22 706f 7374 2220 6964 3d22 666f  od="post" id="fo
+00001550: 726d 2d64 656c 6574 652d 696e 6479 2d61  rm-delete-indy-a
+00001560: 6363 6f75 6e74 223e 0a0a 2020 2020 2020  ccount">..      
+00001570: 2020 7b25 2063 7372 665f 746f 6b65 6e20    {% csrf_token 
+00001580: 257d 0a0a 2020 2020 2020 2020 7b7b 2064  %}..        {{ d
+00001590: 656c 6574 655f 6163 636f 756e 745f 666f  elete_account_fo
+000015a0: 726d 2e6e 6f6e 5f66 6965 6c64 5f65 7272  rm.non_field_err
+000015b0: 6f72 7320 7d7d 0a0a 2020 2020 2020 2020  ors }}..        
+000015c0: 3c64 6976 2063 6c61 7373 3d22 726f 7720  <div class="row 
+000015d0: 666f 726d 2d2d 726f 7722 3e0a 2020 2020  form--row">.    
+000015e0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000015f0: 7373 3d22 666f 726d 2d2d 726f 775f 5f69  ss="form--row__i
+00001600: 6e70 7574 2063 6f6c 2d73 6d2d 3620 636f  nput col-sm-6 co
+00001610: 6c2d 6d64 2d34 223e 0a20 2020 2020 2020  l-md-4">.       
+00001620: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00001630: 6173 733d 2269 6e70 7574 2d2d 6963 6f6e  ass="input--icon
+00001640: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00001650: 2020 2020 2020 2020 2020 2020 7b7b 2064              {{ d
+00001660: 656c 6574 655f 6163 636f 756e 745f 666f  elete_account_fo
+00001670: 726d 2e64 656c 6574 655f 7061 7373 776f  rm.delete_passwo
+00001680: 7264 207d 7d0a 2020 2020 2020 2020 2020  rd }}.          
+00001690: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
+000016a0: 636c 6173 733d 2269 636f 6e69 6679 2220  class="iconify" 
+000016b0: 6461 7461 2d69 636f 6e3d 226d 6469 3a73  data-icon="mdi:s
+000016c0: 6563 7572 6974 7922 3e3c 2f73 7061 6e3e  ecurity"></span>
+000016d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000016e0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+000016f0: 2020 2020 2020 2020 3c73 6d61 6c6c 3e7b          <small>{
+00001700: 7b20 6465 6c65 7465 5f61 6363 6f75 6e74  { delete_account
+00001710: 5f66 6f72 6d2e 6465 6c65 7465 5f70 6173  _form.delete_pas
+00001720: 7377 6f72 642e 6865 6c70 5f74 6578 7420  sword.help_text 
+00001730: 7d7d 3c2f 736d 616c 6c3e 0a20 2020 2020  }}</small>.     
+00001740: 2020 2020 2020 2020 2020 207b 7b20 6465             {{ de
+00001750: 6c65 7465 5f61 6363 6f75 6e74 5f66 6f72  lete_account_for
+00001760: 6d2e 6465 6c65 7465 5f70 6173 7377 6f72  m.delete_passwor
+00001770: 642e 6572 726f 7273 207d 7d0a 2020 2020  d.errors }}.    
+00001780: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00001790: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000017a0: 636c 6173 733d 2266 6f72 6d2d 2d72 6f77  class="form--row
+000017b0: 5f5f 696e 7075 7420 636f 6c2d 736d 2d36  __input col-sm-6
+000017c0: 2063 6f6c 2d6d 642d 3822 3e0a 2020 2020   col-md-8">.    
+000017d0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000017e0: 2063 6c61 7373 3d22 666f 726d 5f5f 6368   class="form__ch
+000017f0: 6563 6b62 6f78 223e 0a20 2020 2020 2020  eckbox">.       
+00001800: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00001810: 7620 636c 6173 733d 2266 6f72 6d5f 5f63  v class="form__c
+00001820: 6865 636b 626f 782d 696e 7075 7422 3e0a  heckbox-input">.
+00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001840: 2020 2020 2020 2020 7b7b 2064 656c 6574          {{ delet
+00001850: 655f 6163 636f 756e 745f 666f 726d 2e75  e_account_form.u
+00001860: 6e73 7562 7363 7269 6265 5f6e 6577 736c  nsubscribe_newsl
+00001870: 6574 7465 7220 7d7d 0a20 2020 2020 2020  etter }}.       
+00001880: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00001890: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+000018a0: 2020 2020 2020 2020 3c6c 6162 656c 2066          <label f
+000018b0: 6f72 3d22 6964 5f7b 7b20 6465 6c65 7465  or="id_{{ delete
+000018c0: 5f61 6363 6f75 6e74 5f66 6f72 6d2e 756e  _account_form.un
+000018d0: 7375 6273 6372 6962 655f 6e65 7773 6c65  subscribe_newsle
+000018e0: 7474 6572 2e68 746d 6c5f 6e61 6d65 207d  tter.html_name }
+000018f0: 7d22 3e7b 7b20 6465 6c65 7465 5f61 6363  }">{{ delete_acc
+00001900: 6f75 6e74 5f66 6f72 6d2e 756e 7375 6273  ount_form.unsubs
+00001910: 6372 6962 655f 6e65 7773 6c65 7474 6572  cribe_newsletter
+00001920: 2e6c 6162 656c 207d 7d3c 2f6c 6162 656c  .label }}</label
+00001930: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001940: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00001950: 2020 2020 2020 2020 207b 7b20 6465 6c65           {{ dele
+00001960: 7465 5f61 6363 6f75 6e74 5f66 6f72 6d2e  te_account_form.
+00001970: 756e 7375 6273 6372 6962 655f 6e65 7773  unsubscribe_news
+00001980: 6c65 7474 6572 2e65 7272 6f72 7320 7d7d  letter.errors }}
+00001990: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
+000019a0: 6976 3e0a 2020 2020 2020 2020 3c2f 6469  iv>.        </di
+000019b0: 763e 0a20 2020 2020 2020 203c 6275 7474  v>.        <butt
+000019c0: 6f6e 2069 643d 2264 656c 6574 655f 6163  on id="delete_ac
+000019d0: 636f 756e 745f 6275 7474 6f6e 2220 636c  count_button" cl
+000019e0: 6173 733d 2262 7574 746f 6e20 6275 7474  ass="button butt
+000019f0: 6f6e 2d2d 7072 696d 6172 7920 6275 7474  on--primary butt
+00001a00: 6f6e 2d2d 7072 696d 6172 792d 2d64 616e  on--primary--dan
+00001a10: 6765 7220 6275 7474 6f6e 2d2d 6963 6f6e  ger button--icon
+00001a20: 2220 6e61 6d65 3d22 6465 6c65 7465 5f61  " name="delete_a
+00001a30: 6363 6f75 6e74 223e 0a20 2020 2020 2020  ccount">.       
+00001a40: 2020 2020 2044 656c 6574 6520 6163 636f       Delete acco
+00001a50: 756e 7420 3c73 7061 6e20 636c 6173 733d  unt <span class=
+00001a60: 2269 636f 6e69 6679 2220 6461 7461 2d69  "iconify" data-i
+00001a70: 636f 6e3d 226d 6469 3a64 656c 6574 652d  con="mdi:delete-
+00001a80: 6f75 746c 696e 6522 3e3c 2f73 7061 6e3e  outline"></span>
+00001a90: 0a20 2020 2020 2020 203c 2f62 7574 746f  .        </butto
+00001aa0: 6e3e 0a20 2020 2020 2020 203c 2f66 6f72  n>.        </for
+00001ab0: 6d3e 0a20 2020 203c 2f64 6976 3e0a 3c2f  m>.    </div>.</
+00001ac0: 6469 763e 0a7b 2520 656e 6469 6620 257d  div>.{% endif %}
+00001ad0: 0a0a 0a7b 2520 656e 6462 6c6f 636b 2025  ...{% endblock %
+00001ae0: 7d0a                                     }.
```

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/play/student_join_organisation.html` & `codeforlife-portal-6.9.0/portal/templates/portal/play/student_join_organisation.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/play.html` & `codeforlife-portal-6.9.0/portal/templates/portal/play.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/privacy_policy.html` & `codeforlife-portal-6.9.0/portal/templates/portal/privacy_policy.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/register.html` & `codeforlife-portal-6.9.0/portal/templates/portal/register.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/reset_password.html` & `codeforlife-portal-6.9.0/portal/templates/portal/reset_password.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/reset_password_confirm.html` & `codeforlife-portal-6.9.0/portal/templates/portal/reset_password_confirm.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/reset_password_done.html` & `codeforlife-portal-6.9.0/portal/templates/portal/reset_password_done.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/reset_password_email_sent.html` & `codeforlife-portal-6.9.0/portal/templates/portal/reset_password_email_sent.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/tag_manager/tag_manager_body.html` & `codeforlife-portal-6.9.0/portal/templates/portal/tag_manager/tag_manager_body.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/tag_manager/tag_manager_head.html` & `codeforlife-portal-6.9.0/portal/templates/portal/tag_manager/tag_manager_head.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/base_registering.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/base_registering.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/class.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/class.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/dashboard.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/dashboard.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/invite.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/invite.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/onboarding_classes.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/onboarding_classes.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/onboarding_print.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/onboarding_print.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/onboarding_school.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/onboarding_school.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/onboarding_students.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/onboarding_students.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_add_external_student.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_add_external_student.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_added_external_student.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_added_external_student.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_aimmo_dashboard.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_aimmo_dashboard.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_dismiss_students.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_dismiss_students.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_edit_class.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_edit_class.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_edit_student.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_edit_student.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_move_all_classes.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_move_all_classes.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_move_students.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_move_students.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_move_students_to_class.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_move_students_to_class.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach/teacher_resources.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach/teacher_resources.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/teach.html` & `codeforlife-portal-6.9.0/portal/templates/portal/teach.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/portal/terms.html` & `codeforlife-portal-6.9.0/portal/templates/portal/terms.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/two_factor/core/backup_tokens.html` & `codeforlife-portal-6.9.0/portal/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/two_factor/core/login.html` & `codeforlife-portal-6.9.0/portal/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/two_factor/core/setup.html` & `codeforlife-portal-6.9.0/portal/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/two_factor/core/setup_complete.html` & `codeforlife-portal-6.9.0/portal/templates/two_factor/core/setup_complete.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/two_factor/profile/disable.html` & `codeforlife-portal-6.9.0/portal/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templates/two_factor/profile/profile.html` & `codeforlife-portal-6.9.0/portal/templates/two_factor/profile/profile.html`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templatetags/app_tags.py` & `codeforlife-portal-6.9.0/portal/templatetags/app_tags.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templatetags/banner_tags.py` & `codeforlife-portal-6.9.0/portal/templatetags/banner_tags.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templatetags/benefits_tags.py` & `codeforlife-portal-6.9.0/portal/templatetags/benefits_tags.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templatetags/character_list_tags.py` & `codeforlife-portal-6.9.0/portal/templatetags/character_list_tags.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/templatetags/hero_card_tags.py` & `codeforlife-portal-6.9.0/portal/templatetags/hero_card_tags.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/base_test.py` & `codeforlife-portal-6.9.0/portal/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/conftest.py` & `codeforlife-portal-6.9.0/portal/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_make_portaladmin_teacher.py` & `codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_make_portaladmin_teacher.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_preview_user_remove.py` & `codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_preview_user_remove.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_preview_users.py` & `codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_preview_users.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_use_common_models.py` & `codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_use_common_models.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/migrations/test_migration_verify_portaladmin.py` & `codeforlife-portal-6.9.0/portal/tests/migrations/test_migration_verify_portaladmin.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/base_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/base_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/game_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/game_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/home_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/home_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/independent_login_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/independent_login_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/kurono_teacher_dashboard_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/kurono_teacher_dashboard_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/password_reset_form_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/password_reset_form_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/password_reset_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/password_reset_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/play/account_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/play/account_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/play/dashboard_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/play/dashboard_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/play/join_school_or_club_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/play/join_school_or_club_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/play/play_base_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/play/play_base_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/signup_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/signup_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/student_login_class_code.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/student_login_class_code.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/student_login_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/student_login_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/add_independent_student_to_class_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/add_independent_student_to_class_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/added_independent_student_to_class_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/added_independent_student_to_class_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/class_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/class_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/dashboard_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/dashboard_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/dismiss_students_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/dismiss_students_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/edit_student_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/edit_student_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/move_class_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/move_class_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/move_classes_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/move_classes_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/move_students_disambiguate_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/move_students_disambiguate_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/move_students_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/move_students_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/onboarding_classes_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/onboarding_classes_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/onboarding_organisation_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/onboarding_organisation_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/onboarding_revoke_request_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/onboarding_revoke_request_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/onboarding_student_list_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/onboarding_student_list_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/onboarding_students_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/onboarding_students_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teach/teach_base_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teach/teach_base_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/pageObjects/portal/teacher_login_page.py` & `codeforlife-portal-6.9.0/portal/tests/pageObjects/portal/teacher_login_page.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/snapshots/snap_test_partials.py` & `codeforlife-portal-6.9.0/portal/tests/snapshots/snap_test_partials.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_2FA.py` & `codeforlife-portal-6.9.0/portal/tests/test_2FA.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_admin.py` & `codeforlife-portal-6.9.0/portal/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_aimmo_dashboards.py` & `codeforlife-portal-6.9.0/portal/tests/test_aimmo_dashboards.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_api.py` & `codeforlife-portal-6.9.0/portal/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_captcha_forms.py` & `codeforlife-portal-6.9.0/portal/tests/test_captcha_forms.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_class.py` & `codeforlife-portal-6.9.0/portal/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_emails.py` & `codeforlife-portal-6.9.0/portal/tests/test_emails.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_independent_student.py` & `codeforlife-portal-6.9.0/portal/tests/test_independent_student.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,22 +140,28 @@
 
         delete_account_form = page.browser.find_element_by_name("delete_password")
         delete_account_form.send_keys(password)
 
         delete_account_button = page.browser.find_element_by_id("delete_account_button")
         delete_account_button.click()
 
+        delete_button_confirm = page.browser.find_element_by_id("delete_button")
+        delete_button_confirm.click()
+
         # check if can still login to the account
         page = self.go_to_homepage()
         assert page.go_to_independent_student_login_page().independent_student_login_failure(email, password)
 
         # now check if anonymised
         assert not User.objects.get(id=user_id).is_active
 
-    def test_signup(self):
+        # check if email has been sent
+        assert len(mail.outbox) == 1
+
+    def test_signup_without_newsletter(self):
         page = self.go_to_homepage()
         page, _, _, _, _ = create_independent_student(page)
         assert is_email_verified_message_showing(self.selenium)
 
     def test_signup_duplicate_email_failure(self):
         page = self.go_to_homepage()
         page, _, _, email, _ = create_independent_student(page)
```

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_invite_teacher.py` & `codeforlife-portal-6.9.0/portal/tests/test_invite_teacher.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_middleware.py` & `codeforlife-portal-6.9.0/portal/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_newsletter_footer.py` & `codeforlife-portal-6.9.0/portal/tests/test_newsletter_footer.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_organisation.py` & `codeforlife-portal-6.9.0/portal/tests/test_organisation.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_partials.py` & `codeforlife-portal-6.9.0/portal/tests/test_partials.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_ratelimit.py` & `codeforlife-portal-6.9.0/portal/tests/test_ratelimit.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_react_test_space.py` & `codeforlife-portal-6.9.0/portal/tests/test_react_test_space.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_school_student.py` & `codeforlife-portal-6.9.0/portal/tests/test_school_student.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_security.py` & `codeforlife-portal-6.9.0/portal/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_teacher.py` & `codeforlife-portal-6.9.0/portal/tests/test_teacher.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_teacher_student.py` & `codeforlife-portal-6.9.0/portal/tests/test_teacher_student.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/test_views.py` & `codeforlife-portal-6.9.0/portal/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/utils/aimmo_games.py` & `codeforlife-portal-6.9.0/portal/tests/utils/aimmo_games.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/tests/utils/messages.py` & `codeforlife-portal-6.9.0/portal/tests/utils/messages.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/urls.py` & `codeforlife-portal-6.9.0/portal/urls.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/admin.py` & `codeforlife-portal-6.9.0/portal/views/admin.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/aimmo/dashboard.py` & `codeforlife-portal-6.9.0/portal/views/aimmo/dashboard.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/api.py` & `codeforlife-portal-6.9.0/portal/views/api.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/dotmailer.py` & `codeforlife-portal-6.9.0/portal/views/dotmailer.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/email.py` & `codeforlife-portal-6.9.0/portal/views/email.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/home.py` & `codeforlife-portal-6.9.0/portal/views/home.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/login/independent_student.py` & `codeforlife-portal-6.9.0/portal/views/login/independent_student.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/login/student.py` & `codeforlife-portal-6.9.0/portal/views/login/student.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/login/teacher.py` & `codeforlife-portal-6.9.0/portal/views/login/teacher.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/organisation.py` & `codeforlife-portal-6.9.0/portal/views/organisation.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/registration.py` & `codeforlife-portal-6.9.0/portal/views/registration.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/student/edit_account_details.py` & `codeforlife-portal-6.9.0/portal/views/student/edit_account_details.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,52 +127,31 @@
             messages.success(request, "Your account details have been successfully changed.")
         else:
             anchor = old_anchor
 
         return changing_email, new_email, changing_password, changing_first_name, anchor
 
     if request.method == "POST":
-        if "delete_password" in request.POST:
+        if "delete_account" in request.POST:
             delete_account_form = DeleteAccountForm(user, request.POST)
             if not delete_account_form.is_valid():
                 messages.warning(request, "Your account was not deleted due to incorrect password.")
-                return render(
-                    request,
-                    template_name,
-                    {"form": change_email_password_form, "delete_account_form": delete_account_form},
-                )
             else:
                 delete_account_confirm = True
-                email = user.email
-                anonymise(user)
-
-                # remove from dotmailer
-                if bool(request.POST.get("unsubscribe_newsletter")):
-                    delete_contact(email)
-
-                # send confirmation email
-                message = accountDeletionEmail(request)
-                send_email(
-                    NOTIFICATION_EMAIL,
-                    [email],
-                    message["subject"],
-                    message["message"],
-                    message["title"],
-                )
-
-                return HttpResponseRedirect(reverse_lazy("home"))
-
         else:
             change_email_password_form = IndependentStudentEditAccountForm(request.user, request.POST)
             if not change_email_password_form.is_valid():
                 messages.warning(request, "Your account was not updated do to incorrect details")
                 return render(
                     request,
                     template_name,
-                    {"form": change_email_password_form, "delete_account_form": delete_account_form},
+                    {
+                        "form": change_email_password_form,
+                        "delete_account_form": delete_account_form,
+                    },
                 )
             else:
                 (
                     changing_email,
                     new_email,
                     changing_password,
                     changing_first_name,
```

### Comparing `codeforlife-portal-6.8.9/portal/views/student/play.py` & `codeforlife-portal-6.9.0/portal/views/student/play.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/teacher/dashboard.py` & `codeforlife-portal-6.9.0/portal/views/teacher/dashboard.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/teacher/teach.py` & `codeforlife-portal-6.9.0/portal/views/teacher/teach.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/teacher/teacher_resources.py` & `codeforlife-portal-6.9.0/portal/views/teacher/teacher_resources.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/portal/views/two_factor/core.py` & `codeforlife-portal-6.9.0/portal/views/two_factor/core.py`

 * *Files identical despite different names*

### Comparing `codeforlife-portal-6.8.9/setup.py` & `codeforlife-portal-6.9.0/setup.py`

 * *Files identical despite different names*

