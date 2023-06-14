# Comparing `tmp/bl_hector-0.1.0a7.tar.gz` & `tmp/bl_hector-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.1.0a7.tar", max compression
+gzip compressed data, was "bl_hector-0.1.0a8.tar", max compression
```

## Comparing `bl_hector-0.1.0a7.tar` & `bl_hector-0.1.0a8.tar`

### file list

```diff
@@ -1,93 +1,92 @@
--rw-r--r--   0        0        0    34523 2023-05-31 09:45:12.827540 bl_hector-0.1.0a7/LICENSE
--rw-r--r--   0        0        0     1507 2023-06-13 08:52:57.770248 bl_hector-0.1.0a7/README.md
--rw-r--r--   0        0        0      807 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     3807 2023-06-13 17:10:53.285803 bl_hector-0.1.0a7/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     1981 2023-06-09 06:16:19.350310 bl_hector-0.1.0a7/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     3480 2023-06-13 07:05:26.339251 bl_hector-0.1.0a7/bl_hector/application/use_cases/import_books.py
--rw-r--r--   0        0        0     1979 2023-06-13 07:05:37.235116 bl_hector-0.1.0a7/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     3755 2023-06-11 08:06:35.483796 bl_hector-0.1.0a7/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     3805 2023-06-13 17:23:36.928433 bl_hector-0.1.0a7/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0      808 2023-06-09 13:18:08.922894 bl_hector-0.1.0a7/bl_hector/domain/administration/enumerations.py
--rw-r--r--   0        0        0     1659 2023-06-09 13:18:04.750942 bl_hector-0.1.0a7/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1567 2023-06-13 17:10:09.238345 bl_hector-0.1.0a7/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0      996 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/collection_management/exceptions.py
--rw-r--r--   0        0        0     1509 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0     1173 2023-06-13 16:46:31.847726 bl_hector-0.1.0a7/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     1804 2023-06-11 08:06:35.483796 bl_hector-0.1.0a7/bl_hector/domain/collection_management/validators.py
--rw-r--r--   0        0        0     3749 2023-06-13 16:39:49.484615 bl_hector-0.1.0a7/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0     1453 2023-06-13 16:46:31.579729 bl_hector-0.1.0a7/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     3706 2023-06-13 11:18:20.228210 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     1693 2023-06-09 08:04:31.521092 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     4116 2023-06-13 17:14:54.950836 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     3466 2023-06-13 16:45:43.904308 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      664 2023-06-13 07:15:23.075945 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0    35880 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
--rw-r--r--   0        0        0      928 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0     3602 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
--rw-r--r--   0        0        0    42819 2023-06-07 16:14:27.670555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-07 16:14:27.670555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-07 16:14:27.670555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-07 16:14:27.670555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     2112 2023-06-13 09:33:38.004683 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/totp/__init__.py
--rw-r--r--   0        0        0     1265 2023-06-09 13:18:08.926894 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4544 2023-06-13 08:24:56.879217 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3282 2023-06-13 05:56:18.671790 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1789 2023-06-13 17:15:23.130490 bl_hector-0.1.0a7/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1568 2023-06-13 07:05:37.235116 bl_hector-0.1.0a7/bl_hector/infrastructure/requests/__init__.py
--rw-r--r--   0        0        0     2138 2023-06-13 11:18:20.228210 bl_hector-0.1.0a7/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     8340 2023-06-13 17:24:02.232123 bl_hector-0.1.0a7/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2957 2023-06-13 16:46:20.467864 bl_hector-0.1.0a7/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     2099 2023-06-13 07:05:37.235116 bl_hector-0.1.0a7/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0     1393 2023-06-13 05:56:18.671790 bl_hector-0.1.0a7/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0      761 2023-06-10 16:50:21.825376 bl_hector-0.1.0a7/bl_hector/interfaces/exceptions.py
--rw-r--r--   0        0        0     3371 2023-06-11 08:23:57.603430 bl_hector-0.1.0a7/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1659 2023-06-13 07:05:37.239116 bl_hector-0.1.0a7/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1435 2023-06-07 17:00:49.589157 bl_hector-0.1.0a7/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     4568 2023-06-13 17:14:28.243164 bl_hector-0.1.0a7/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     5167 2023-06-13 17:14:41.846997 bl_hector-0.1.0a7/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1407 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    15005 2023-06-13 17:13:45.447689 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1247 2023-06-09 13:26:25.425148 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     4296 2023-06-13 14:17:08.848203 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     2100 2023-06-13 17:14:13.355347 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     2048 2023-06-11 09:09:06.457902 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
--rw-r--r--   0        0        0     5607 2023-06-13 14:17:08.848203 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3589 2023-06-13 08:34:41.343554 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      982 2023-06-09 13:18:08.934894 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2026 2023-06-09 13:26:33.641053 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1127 2023-06-13 07:11:41.542636 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     4134 2023-06-11 08:39:27.744213 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     1992 2023-06-13 14:17:08.848203 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     1400 2023-06-13 09:27:19.501527 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
--rw-r--r--   0        0        0     2010 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-13 07:05:37.239116 bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     4445 2023-06-11 08:06:35.487796 bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     1516 2023-06-13 17:25:15.715222 bl_hector-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0     4246 2023-06-13 17:25:55.523007 bl_hector-0.1.0a7/setup.py
--rw-r--r--   0        0        0     2560 2023-06-13 17:25:55.524440 bl_hector-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-31 09:45:12.827540 bl_hector-0.1.0a8/LICENSE
+-rw-r--r--   0        0        0     1854 2023-06-14 06:53:49.525288 bl_hector-0.1.0a8/README.md
+-rw-r--r--   0        0        0      807 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3803 2023-06-14 08:52:32.636997 bl_hector-0.1.0a8/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     1977 2023-06-14 08:52:32.588998 bl_hector-0.1.0a8/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     1975 2023-06-14 08:52:32.616998 bl_hector-0.1.0a8/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     3751 2023-06-14 08:52:32.600998 bl_hector-0.1.0a8/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     3801 2023-06-14 08:52:32.580998 bl_hector-0.1.0a8/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0      808 2023-06-09 13:18:08.922894 bl_hector-0.1.0a8/bl_hector/domain/administration/enumerations.py
+-rw-r--r--   0        0        0     1659 2023-06-09 13:18:04.750942 bl_hector-0.1.0a8/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1563 2023-06-14 08:54:37.759525 bl_hector-0.1.0a8/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0      996 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/collection_management/errors.py
+-rw-r--r--   0        0        0     1509 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0     1173 2023-06-13 16:46:31.847726 bl_hector-0.1.0a8/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     1800 2023-06-14 08:53:33.276286 bl_hector-0.1.0a8/bl_hector/domain/collection_management/validators.py
+-rw-r--r--   0        0        0     3325 2023-06-14 08:52:32.560998 bl_hector-0.1.0a8/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0     1453 2023-06-13 16:46:31.579729 bl_hector-0.1.0a8/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3738 2023-06-14 08:44:03.058810 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-07 16:14:27.658555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1693 2023-06-09 08:04:31.521092 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     4116 2023-06-13 17:14:54.950836 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     3466 2023-06-13 16:45:43.904308 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      664 2023-06-13 07:15:23.075945 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0    35880 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
+-rw-r--r--   0        0        0      928 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0     3602 2023-06-07 16:14:27.662555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
+-rw-r--r--   0        0        0    42819 2023-06-07 16:14:27.670555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-07 16:14:27.670555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     6828 2023-06-07 16:14:27.670555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-07 16:14:27.670555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     2363 2023-06-14 06:38:35.772624 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/totp/__init__.py
+-rw-r--r--   0        0        0     1265 2023-06-09 13:18:08.926894 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4544 2023-06-13 08:24:56.879217 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-13 05:56:18.671790 bl_hector-0.1.0a8/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1789 2023-06-13 17:15:23.130490 bl_hector-0.1.0a8/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1568 2023-06-13 07:05:37.235116 bl_hector-0.1.0a8/bl_hector/infrastructure/requests/__init__.py
+-rw-r--r--   0        0        0     2615 2023-06-14 06:22:16.919024 bl_hector-0.1.0a8/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     8336 2023-06-14 08:52:32.540998 bl_hector-0.1.0a8/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-07 16:14:27.674555 bl_hector-0.1.0a8/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2419 2023-06-14 08:58:30.132757 bl_hector-0.1.0a8/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     2099 2023-06-14 08:40:08.593384 bl_hector-0.1.0a8/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0     1845 2023-06-14 08:54:22.907701 bl_hector-0.1.0a8/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-10 16:50:21.825376 bl_hector-0.1.0a8/bl_hector/interfaces/exceptions.py
+-rw-r--r--   0        0        0     3371 2023-06-11 08:23:57.603430 bl_hector-0.1.0a8/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1659 2023-06-13 07:05:37.239116 bl_hector-0.1.0a8/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1435 2023-06-07 17:00:49.589157 bl_hector-0.1.0a8/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     4568 2023-06-13 17:14:28.243164 bl_hector-0.1.0a8/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     5167 2023-06-13 17:14:41.846997 bl_hector-0.1.0a8/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1407 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    14753 2023-06-14 08:55:58.762565 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1331 2023-06-14 09:08:21.253609 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     4296 2023-06-13 14:17:08.848203 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     2100 2023-06-13 17:14:13.355347 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     2043 2023-06-14 08:24:15.964273 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
+-rw-r--r--   0        0        0     5646 2023-06-14 09:05:35.607596 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3589 2023-06-13 08:34:41.343554 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      982 2023-06-09 13:18:08.934894 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2045 2023-06-14 09:04:09.936643 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1127 2023-06-13 07:11:41.542636 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     4129 2023-06-14 08:23:59.692482 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     1992 2023-06-13 14:17:08.848203 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     1400 2023-06-13 09:27:19.501527 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
+-rw-r--r--   0        0        0     2010 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-13 07:05:37.239116 bl_hector-0.1.0a8/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     3888 2023-06-14 08:58:01.757097 bl_hector-0.1.0a8/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-07 16:14:27.682555 bl_hector-0.1.0a8/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     1516 2023-06-14 09:09:41.284665 bl_hector-0.1.0a8/pyproject.toml
+-rw-r--r--   0        0        0     4603 2023-06-14 09:10:49.897226 bl_hector-0.1.0a8/setup.py
+-rw-r--r--   0        0        0     2907 2023-06-14 09:10:49.898937 bl_hector-0.1.0a8/PKG-INFO
```

### Comparing `bl_hector-0.1.0a7/LICENSE` & `bl_hector-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/README.md` & `bl_hector-0.1.0a8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 # Hector — a collection manager
 
 ## Install
 
-For the time being, Hector cannot be installed from PyPI.
-See [CONTRIBUTING.md]() to set up a development environment.
+Hector is available on PyPI under the name `bl_hector`.
+To install, just run `python -m pip install bl_hector`.
 
 
 ## Configure
 
 Hector is configured using environment variables.
-All the variable names are prefixed with `HECTOR_`.
+See [the `settings` module](bl_hector/infrastructure/settings.py) for
+a comprehensive list of configuration variables.
+
+All the variable names must be prefixed with `HECTOR_`. For instance :
 
 ```console
+# The secret can be generated using the `secrets.token_hex()` function.
 $ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
+
+# Additional Python database drivers might be required depending on the DSN.
 $ export HECTOR_DSN="sqlite:///data.sqlite"
 ```
 
-The secret can be generated using the `token_hex()` function from
-the Python's `secrets` module.
-
-Additional Python database drivers might be required depending on the DSN.
-
-See [the `settings` module](bl_hector/infrastructure/settings.py) for
-a comprehensive list of configuration variables.
-
 
 ## Authentication
 
 To enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)
 and enable it explicitly:
 
 ```console
-$ export HECTOR_WEBAUTHN=1
+$ export HECTOR_WEBAUTHN_ENABLED=1
 ```
 
-To enable TOTP authentication, you must install extra dependencies (`bl-hector[totp]`)
-and enable it explicitly by setting a base32 random secret (`pyotp.random_base32()`):
+TOTP authentication is provided to be able to login on servers that do not (yet) support
+the `cryptography` module. You must install extra dependencies (`bl-hector[totp]`)
+and enable it explicitly by setting a base32 random secret:
 
 ```console
-$ export HECTOR_TOTP=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
+# The secret can be generated using the `pyotp.random_base32()` function.
+$ export HECTOR_TOTP_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
 ```
 
+Note that it is a highly insecure way of authenticating, as anyone gaining access to your
+OTP generator would be able to login.
+
+
 ## Initialise
 
 Once configured, you must initialise Hector's database with the dedicated command:
 
 ```console
 $ hector init-db
 ```
@@ -54,7 +58,12 @@
 
 Hector being a Flask application, it can be run using any WSGI server,
 for instance, with [Gunicorn](https://gunicorn.org):
 
 ```console
 $ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"
 ```
+
+
+## Contributing
+
+See [CONTRIBUTING.md]() to set up a development environment.
```

### Comparing `bl_hector-0.1.0a7/bl_hector/__init__.py` & `bl_hector-0.1.0a8/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/application/__init__.py` & `bl_hector-0.1.0a8/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.1.0a8/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.1.0a8/bl_hector/application/use_cases/add_book.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing import Optional
 
 from bl_hector.domain.administration.enumerations import Permissions as P
 from bl_hector.domain.administration.repositories import Permissions
 from bl_hector.domain.administration.value_objects import UserId
 from bl_hector.domain.collection_management import validators
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.exceptions import IncorrectValue
+from bl_hector.domain.collection_management.errors import IncorrectValue
 from bl_hector.domain.collection_management.repositories import Books
 from bl_hector.domain.collection_management.services import Calendar
 from bl_hector.domain.collection_management.value_objects import (
     Author,
     Cover,
     Genre,
     Isbn,
```

### Comparing `bl_hector-0.1.0a7/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.1.0a8/bl_hector/application/use_cases/display_book.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.exceptions import IncorrectValue
+from bl_hector.domain.collection_management.errors import IncorrectValue
 from bl_hector.domain.collection_management.repositories import Books
 from bl_hector.domain.collection_management.value_objects import Isbn
 
 
 @dataclass(frozen=True)
 class Request:
     isbn: str
```

### Comparing `bl_hector-0.1.0a7/bl_hector/application/use_cases/import_books.py` & `bl_hector-0.1.0a8/bl_hector/application/use_cases/update_book.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,92 +11,109 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
-from pathlib import Path
+from dataclasses import dataclass, fields
 from typing import Optional
 
+from bl_hector.domain.administration.enumerations import Permissions as P
+from bl_hector.domain.administration.repositories import Permissions
+from bl_hector.domain.administration.value_objects import UserId
+from bl_hector.domain.collection_management import validators
 from bl_hector.domain.collection_management.entities import Book
+from bl_hector.domain.collection_management.errors import IncorrectValue
 from bl_hector.domain.collection_management.repositories import Books
-from bl_hector.domain.collection_management.services import BookInfoProvider
-from bl_hector.domain.collection_management.value_objects import Isbn
+from bl_hector.domain.collection_management.services import Calendar
+from bl_hector.domain.collection_management.value_objects import (
+    Author,
+    Cover,
+    Genre,
+    Isbn,
+    Title,
+    Year,
+)
 
 
 @dataclass(frozen=True)
 class Request:
-    path: str
+    user_id: str
+    isbn: str
+    title: str
+    year: int
+    authors: list[str]
+    genres: list[str]
+    cover: str = ""
+
+
+@dataclass
+class Errors:
+    title: Optional[IncorrectValue] = None
+    year: Optional[IncorrectValue] = None
+    authors: Optional[IncorrectValue] = None
 
+    def __bool__(self) -> bool:
+        return any([getattr(self, f.name) for f in fields(self)])
 
-class Presenter(ABC):
-    @abstractmethod
-    def file_does_not_exist(self, path: str) -> None:
-        ...
 
+class Presenter(ABC):
     @abstractmethod
-    def line_skipped(self, line_number: int, text: str, reason: str) -> None:
+    def not_authorized(self) -> None:
         ...
 
     @abstractmethod
-    def book_already_exists(self, book: Book) -> None:
+    def bad_request(self, errors: Errors) -> None:
         ...
 
     @abstractmethod
-    def book_info_not_found(self, isbn: Isbn) -> None:
+    def book_not_found(self, isbn: Isbn) -> None:
         ...
 
     @abstractmethod
-    def book_added(self, book: Book) -> None:
+    def book_updated(self, book: Book) -> None:
         ...
 
 
 @dataclass(frozen=True)
 class Interactor:
-    """
-    **WARNING:** This use case is not specified, for it is not trivial!
-    It is also not a use case that should actually be used! It might even be removed.
-    It might be better to implement it by wireing the other commands together.
-    This would solve the problem of the commit of the data. For the time being
-    the commit only happens once at the end of the command, even if thousands of books
-    have to be imported!?
-    """
-
     presenter: Presenter
-    info_provider: BookInfoProvider
     books: Books
+    calendar: Calendar
+    permissions: Permissions
 
     def execute(self, request: Request) -> None:
-        path = Path(request.path)
-        if not path.is_file():
-            return self.presenter.file_does_not_exist(request.path)
-
-        for isbn in self.__extract_isbn_from_file(path):
-            if book := self.books.by_isbn(isbn):
-                self.presenter.book_already_exists(book)
-                continue
-            if not (book := self.info_provider.look_up(isbn)):
-                self.presenter.book_info_not_found(isbn)
-                continue
-            self.books.add(book)
-            self.presenter.book_added(book)
-
-    def __extract_isbn_from_file(self, path: Path) -> list[Isbn]:
-        return [
-            isbn
-            for number, text in enumerate(path.read_text().splitlines())
-            if (isbn := self.__extract_isbn_from_line(number, text))
-        ]
-
-    def __extract_isbn_from_line(self, number: int, text: str) -> Optional[Isbn]:
-        _text = text.strip()
-        if "#" in _text:
-            if _text.startswith("#"):
-                return None
-            _text = text.split("#", 1)[0]
-
-        try:
-            return Isbn.instanciate(_text)
-        except Exception as exc:
-            return self.presenter.line_skipped(number, text, str(exc))
+        if not self.__is_authorized(request.user_id):
+            return self.presenter.not_authorized()
+
+        if errors := self.__validate_request(request):
+            return self.presenter.bad_request(errors)
+
+        isbn = Isbn.instanciate(request.isbn)
+        if not (original_book := self.books.by_isbn(isbn=isbn)):
+            return self.presenter.book_not_found(isbn)
+
+        # There's no business logic to apply when updating a book.
+        book = Book.instanciate(
+            original_book.added_on,
+            self.calendar.today(),
+            isbn,
+            Title.instanciate(request.title),
+            Year.instanciate(request.year),
+            [Author.instanciate(a) for a in request.authors if a],
+            [Genre.instanciate(g) for g in request.genres if g],
+            Cover.instanciate(request.cover) if request.cover else None,
+        )
+
+        self.books.update(book)
+        self.presenter.book_updated(book)
+
+    def __is_authorized(self, user_id: str) -> bool:
+        return self.permissions.is_authorized_to(UserId(user_id), P.UPDATE_BOOK)
+
+    def __validate_request(self, request: Request) -> Errors:
+        return Errors(
+            title=validators.title(request.title),
+            year=validators.year(request.year),
+            authors=validators.authors(request.authors),
+        )
```

### Comparing `bl_hector-0.1.0a7/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.1.0a8/bl_hector/application/use_cases/look_up_book.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.exceptions import IncorrectValue
+from bl_hector.domain.collection_management.errors import IncorrectValue
 from bl_hector.domain.collection_management.services import (
     BookInfoProvider,
     CoverProvider,
 )
 from bl_hector.domain.collection_management.value_objects import Isbn
```

### Comparing `bl_hector-0.1.0a7/bl_hector/application/use_cases/search_books.py` & `bl_hector-0.1.0a8/bl_hector/application/use_cases/search_books.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, fields
 from typing import Optional
 
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.exceptions import IncorrectValue
+from bl_hector.domain.collection_management.errors import IncorrectValue
 from bl_hector.domain.collection_management.repositories import Books
 from bl_hector.domain.collection_management.value_objects import (
     Author,
     Genre,
     Isbn,
     Title,
     Year,
```

### Comparing `bl_hector-0.1.0a7/bl_hector/configuration/__init__.py` & `bl_hector-0.1.0a8/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/configuration/cli.py` & `bl_hector-0.1.0a8/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/configuration/wsgi.py` & `bl_hector-0.1.0a8/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/__init__.py` & `bl_hector-0.1.0a8/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/administration/__init__.py` & `bl_hector-0.1.0a8/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/administration/entities.py` & `bl_hector-0.1.0a8/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/administration/enumerations.py` & `bl_hector-0.1.0a8/bl_hector/domain/administration/enumerations.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/administration/repositories.py` & `bl_hector-0.1.0a8/bl_hector/domain/administration/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/administration/services.py` & `bl_hector-0.1.0a8/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.1.0a8/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.1.0a8/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.1.0a8/bl_hector/domain/collection_management/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 from typing import Optional
 
-from .exceptions import IncorrectValue
+from .errors import IncorrectValue
 from .value_objects import Author, Cover, Date, Genre, Isbn, Title, Year
 
 
 @dataclass
 class Book:
     added_on: Date
     updated_on: Date
```

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/collection_management/exceptions.py` & `bl_hector-0.1.0a8/bl_hector/domain/collection_management/errors.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.1.0a8/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/collection_management/services.py` & `bl_hector-0.1.0a8/bl_hector/domain/collection_management/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/collection_management/validators.py` & `bl_hector-0.1.0a8/bl_hector/domain/collection_management/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Optional
 
-from .exceptions import IncorrectValue
+from .errors import IncorrectValue
 from .value_objects import Author, Isbn, Title, Year
 
 
 def isbn(value: str) -> Optional[IncorrectValue]:
     try:
         Isbn.instanciate(value)
     except IncorrectValue as exc:
```

### Comparing `bl_hector-0.1.0a7/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.1.0a8/bl_hector/domain/collection_management/value_objects.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,47 +16,41 @@
 
 import datetime
 from typing import Type
 
 import bl3d
 from isbnlib import is_isbn13, mask
 
-from bl_hector.domain.collection_management.exceptions import IncorrectValue
+from bl_hector.domain.collection_management.errors import IncorrectValue
 
 
 class String(bl3d.String):
     @classmethod
     def instanciate(cls: Type[bl3d.TypeString], value: str) -> bl3d.TypeString:
         try:
             return super().instanciate(value)
         except bl3d.InvalidValue as exc:
-            # TODO use the `bl3d.StringXxxYyy` exceptions when available.
-            #      let them pass or recast them!?
             raise IncorrectValue(cls.__name__, str(exc).split(":", 1)[1])
 
 
 class Integer(bl3d.Integer):
     @classmethod
     def instanciate(cls: Type[bl3d.TypeInteger], value: int) -> bl3d.TypeInteger:
         try:
             return super().instanciate(value)
         except bl3d.InvalidValue as exc:
-            # TODO use the `bl3d.NumberXxxYyy` exceptions when available.
-            #      let them pass or recast them!?
             raise IncorrectValue(cls.__name__, str(exc).split(":", 1)[1])
 
 
 class Date(bl3d.Date):
     @classmethod
     def instanciate(cls: Type[bl3d.TypeDate], value: datetime.date) -> bl3d.TypeDate:
         try:
             return super().instanciate(value)
         except bl3d.InvalidValue as exc:
-            # TODO use the `bl3d.DateXxxYyy` exceptions when available.
-            #      let them pass or recast them!?
             raise IncorrectValue(cls.__name__, str(exc).split(":", 1)[1])
 
 
 class Isbn(String):
     """
     The International Standard Book Number (ISBN) of a book,
     for instance 978-0-7653-9277-0.
@@ -71,15 +65,14 @@
 
         super().instanciate(__value)
         if is_isbn13(__value):
             return cls(__value)
 
         raise IncorrectValue(cls.__name__, "This value doesn't look like an ISBN-13.")
 
-    # TODO use the one from `bl3d` when available
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(value={self})"
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Isbn):
             return NotImplemented
         # Isbn built with `__init__` might still contain `-`,
```

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/__init__.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 from bl_hector import __version__
 from bl_hector.infrastructure.flask import services
 from bl_hector.infrastructure.flask.aliases import blueprint as aliases
 from bl_hector.infrastructure.flask.auth import blueprint as auth
 from bl_hector.infrastructure.flask.books import blueprint as books
 from bl_hector.infrastructure.flask.utils import presenter_to_response
 from bl_hector.infrastructure.settings import WsgiSettings
-from bl_hector.interfaces import exceptions, l10n
+from bl_hector.interfaces import l10n
+from bl_hector.interfaces.exceptions import BadRequest
 from bl_hector.interfaces.to_http.as_html import JinjaPresenter
 
 
 def build_app(settings: WsgiSettings) -> Flask:
     services.define_settings(settings)
 
     app = Flask(__name__)
@@ -52,15 +53,15 @@
 
     @app.before_request
     def guess_locale() -> None:
         g.locale = (
             request.accept_languages.best_match(l10n.LOCALES) or l10n.DEFAULT_LOCALE
         )
 
-    @app.errorhandler(exceptions.BadRequest)  # type: ignore[type-var]
+    @app.errorhandler(BadRequest)  # type: ignore[type-var]
     @presenter_to_response
     def handle_bad_request(e: Exception) -> Any:
         presenter = JinjaPresenter(
             "error",
             message="You submitted a bad request! This should have never happened!?",
         )
         presenter.set_status_code(HTTP.BAD_REQUEST)
```

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/auth/__init__.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/hector.css` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/css/hector.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/totp/__init__.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/totp/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,40 +10,45 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Any
+from typing import Any, cast
 from uuid import uuid4
 
 import pyotp
 from flask import Blueprint, flash, request, session, url_for
 
 from bl_hector.domain.administration.entities import User
 from bl_hector.domain.administration.value_objects import UserId
 from bl_hector.infrastructure import ONLY_USER
 from bl_hector.infrastructure.flask import services
 from bl_hector.infrastructure.flask.utils import presenter_to_response
+from bl_hector.infrastructure.settings import TotpSettings
 from bl_hector.interfaces.to_http import Redirection, as_html
 
 blueprint = Blueprint("totp", __name__)
 
 
 @blueprint.get("/login")
 @presenter_to_response
 def login() -> Any:
     return as_html.JinjaPresenter("totp/login", user=services.get_user())
 
 
 @blueprint.post("/login")
 @presenter_to_response
 def login_POST() -> Any:
-    totp = pyotp.TOTP(services.get_settings().TOTP)
+    # TOTP settings must be defined for this route to be accessible.
+    # Other alternatives: 1) check presence with `if` or 2) ignore type.
+    TOTP = cast(TotpSettings, services.get_settings().TOTP)
+
+    totp = pyotp.TOTP(TOTP.SECRET)
     if not totp.verify(request.form.get("password", "")):
         flash("Error authenticating with TOTP.", "error")
         return Redirection(url_for("totp.login"))
 
     if not (user := services.get_users().by_login(ONLY_USER)):
         user = User(UserId(str(uuid4())), ONLY_USER, "The only user")
         services.get_users().add(user)
```

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/requests/__init__.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/settings.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,47 +11,64 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
+from typing import Optional
 
 import bl_seth
 
 
 @dataclass(frozen=True)
+class TotpSettings(bl_seth.Settings):
+    SECRET: str
+    """The secret key.
+    It can be generated with `pyotp.random_base32()`.
+    """
+
+
+@dataclass(frozen=True)
+class WebAuthnSettings(bl_seth.Settings):
+    # Could have been done with a simple `WEBAUTHN: bool = False`,
+    # but this way it's similar to TOTP configuration.
+    ENABLED: bool = False
+    """To enable WebAuthn authentication."""
+
+
+@dataclass(frozen=True)
 class WsgiSettings(bl_seth.Settings):
     SECRET_KEY: str
     """The secret key for Flask sessions.
     See: <https://flask.palletsprojects.com/en/2.3.x/quickstart/#sessions>."""
 
     DSN: str
     """The data source name to access the database.
     See: <https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls>."""
 
-    DEBUG_SQL: bool = False
-    """To enable SqlAlchemy logging.
-    See: <https://docs.sqlalchemy.org/en/20/core/engines.html#configuring-logging>."""
-
     PROXIED: bool = False
     """To let Flask know that it runs behind a proxy.
     See: <https://flask.palletsprojects.com/en/2.3.x/deploying/proxy_fix/>.
     """
 
-    WEBAUTHN: bool = False
-    """To enable WebAuthn authentication.
-    Extra dependencies must be installed: `bl-hector[webauthn]`.
-    """
+    DEBUG_SQL: bool = False
+    """To enable SqlAlchemy logging.
+    See: <https://docs.sqlalchemy.org/en/20/core/engines.html#configuring-logging>."""
 
-    TOTP: str = ""
-    """The secret key for TOTP authentication.
+    # Authentication mechanisms
 
+    TOTP: Optional[TotpSettings] = None
+    """To configure time-based one-time password.
     Extra dependencies must be installed: `bl-hector[totp]`.
-    It can be generated with `pyotp.random_base32()`.
+    """
+
+    WEBAUTHN: Optional[WebAuthnSettings] = None
+    """To enable WebAuthn authentication.
+    Extra dependencies must be installed: `bl-hector[webauthn]`.
     """
 
 
 @dataclass(frozen=True)
 class CliSettings(bl_seth.Settings):
     DSN: str
     """The data source name to access the database.
```

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from bl_hector.domain.administration.repositories import Users as IUsers
 from bl_hector.domain.administration.value_objects import (
     ChallengeId,
     ChallengeValue,
     UserId,
 )
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.exceptions import UnknownBook
+from bl_hector.domain.collection_management.errors import UnknownBook
 from bl_hector.domain.collection_management.repositories import Books as IBooks
 from bl_hector.domain.collection_management.value_objects import (
     Author,
     Cover,
     Date,
     Genre,
     Isbn,
```

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/typer/books.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import sys
 
 import typer
 from typing_extensions import Annotated
 
-from bl_hector.application.use_cases import add_book, import_books, look_up_book
+from bl_hector.application.use_cases import add_book, look_up_book
 from bl_hector.infrastructure import ONLY_USER, DummyPermissions, SystemCalendar
 from bl_hector.infrastructure.typer import services
 from bl_hector.interfaces import from_json as controllers
 from bl_hector.interfaces.to_terminal import LookUpBookInterface, as_json, as_text
 
 cmd = typer.Typer()
 
@@ -58,21 +58,7 @@
         presenter = as_text.AddBook(
             lambda m: typer.echo(m), translator=services.get_translator()
         )
         interactor = add_book.Interactor(presenter, books, calendar, permissions)
         controller = controllers.AddBook(sys.stdin.readline(), ONLY_USER)
         controller.call(interactor)
         raise typer.Exit(presenter.exit_code())
-
-
-@cmd.command("import")
-def import_(ctx: typer.Context, path: str) -> None:
-    """Import a list of books to the collection."""
-    with services.get_books(ctx.obj) as books:
-        presenter = as_text.ImportBooks(
-            lambda m: typer.echo(m), translator=services.get_translator()
-        )
-        interactor = import_books.Interactor(
-            presenter, services.get_book_info_provider(), books
-        )
-        interactor.execute(import_books.Request(path))
-        raise typer.Exit(presenter.exit_code())
```

### Comparing `bl_hector-0.1.0a7/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.1.0a8/bl_hector/infrastructure/typer/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/__init__.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
-from typing import Any
+from typing import Any, Optional
 
 from bl_hector.domain.administration.enumerations import Permissions
+from bl_hector.domain.collection_management import errors
+from bl_hector.interfaces.l10n import Translator
 
 
 @dataclass
 class User:
     id: str
     locale: str
     permissions: list[Permissions]
@@ -35,7 +37,19 @@
     def has_permission(self, permission: str) -> bool:
         if not self.id:
             return False
         try:
             return Permissions[permission] in self.permissions
         except KeyError:
             return False
+
+
+def translate_error(
+    translator: Translator, error: Optional[errors.IncorrectValue] = None
+) -> str:
+    if not error:
+        return ""
+
+    # Dispatching errors based on class is not very LSP!?
+    if isinstance(error, errors.IncorrectValue):
+        return translator("incorrect-value")
+    return translator("unknown-error")
```

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/exceptions.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/from_dict.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/from_dict.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/from_json.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/from_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.1.0a8/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.1.0a8/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,18 @@
 from bl_hector.application.use_cases import (
     add_book,
     display_book,
     look_up_book,
     search_books,
     update_book,
 )
-from bl_hector.domain.collection_management import exceptions as errors
-from bl_hector.domain.collection_management import validators
+from bl_hector.domain.collection_management import errors, validators
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.value_objects import Isbn
-from bl_hector.interfaces import User, l10n
+from bl_hector.interfaces import User, l10n, translate_error
 from bl_hector.interfaces.to_http import HttpPresenter
 
 ENVIRONMENT = Environment(
     loader=FileSystemLoader([Path(__file__).parent / "templates"]),
     autoescape=select_autoescape(),
     extensions=["bl_hector.interfaces.utils.PatchedPyPugJSExtension"],
 )
@@ -78,21 +77,15 @@
         locale = user.locale if (user and user.locale) else l10n.DEFAULT_LOCALE
         self.__localization = l10n.localization(locale)
 
     def _(self, message_id: str, **kwargs: Any) -> str:
         return str(self.__localization.format_value(message_id, kwargs))
 
     def translate_error(self, error: Optional[errors.IncorrectValue] = None) -> str:
-        if not error:
-            return ""
-
-        # FIXME: Dispatching errors based on class is not very LSP!?
-        if isinstance(error, errors.IncorrectValue):
-            return self._("incorrect-value")
-        return self._("unknown-error")
+        return translate_error(self._, error)
 
     def status_code(self) -> int:
         return int(self.__status_code)
 
     def headers(self) -> dict[str, str]:
         return self.__headers
```

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files 7% similar despite different names*

```diff
@@ -23,13 +23,14 @@
   section.section
     .container
       h1.title.is-3.has-text-centered= _("auth-login-title")
 
       .columns
         .column
         .column
-          .buttons
+          //- Webauthn requires the page to be "properly" loaded.
+          .buttons(hx-boost="false")
             each link in links
               a.button.is-fullwidth(href="#{url_for(link.route)}")
                 span.icon: i.fas(class="fa-#{link.icon}")
                 span= _("auth-login-method", method=link.label)
         .column
```

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       if error
         - var classes = "is-danger"
       elif value
         - var classes = "is-success"
       else
         - var classes = ""
 
-      //- TODO find a better way to set required!
+      //- Find a better way to set required!
       if required
         input.input(
           type="text"
           id="isbn"
           name="isbn"
           class=classes
           value=value
```

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
                   each book in books
                     article.book.card(
                       hx-get="#{next_page_url if loop.last else ''}"
                       hx-trigger="#{'revealed' if loop.last else ''}"
                       hx-swap="#{'beforeend' if loop.last else ''}"
                       hx-target="#books"
                       hx-indicator="#indicator"
+                      hx-boost="false"
                     )
                       .card-content
                         .media
                           .media-left(style="width: 5em")
                             figure.image.cover.is-2by3
                               img(src="#{book.cover or url_for('static', filename='img/placeholders/320x480.png')}" alt="Book cover")
                           .media-content
```

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/layout.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Files 5% similar despite different names*

```diff
@@ -18,26 +18,28 @@
 include mixins/navbar
 
 doctype html
 html
   head
     meta(charset="utf-8")
     meta(name="viewport" content="width=device-width, initial-scale=1")
+
     block title
       //- `title` tag inside the block to avoid some weird syntax highlighting problems
       title= _("hector")
 
     link(rel="icon" type="image/svg" href="#{url_for('static', filename='favicon.svg')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/bulma@0.9.4.min.css')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/font-awesome@5.14.0.css')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/hector.css')}")
     block links
+
     block head_scripts
 
-  body
+  body(hx-boost="true")
     +navbar()
 
     .page
       - var messages = get_flashed_messages(with_categories=true)
       +flash(messages)
 
       block content
```

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 mixin hidden_input(name, value)
   input(type="hidden" name=name value=value)
 
 mixin input(type, name, value, required="", icon="", placeholder="", error="")
   - var classes = "has-icons-left" if icon else ""
   p.control.has-icons-right(class=classes)
     - var classes = "is-danger" if error else ""
-    //- TODO find a better way to set required!
+    //- Find a better way to set required!
     if required
       input.input(id=name name=name type=type placeholder=placeholder value=value class=classes required)
     else
       input.input(id=name name=name type=type placeholder=placeholder value=value class=classes)
     if icon
       span.icon.is-small.is-left: i.fas(class="fa-#{icon}")
```

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/__init__.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/as_json.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/as_text.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/to_terminal/as_text.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Callable
+from typing import Callable, Optional
 
-from bl_hector.application.use_cases import add_book, import_books
+from bl_hector.application.use_cases import add_book
 from bl_hector.domain.collection_management.entities import Book
+from bl_hector.domain.collection_management.errors import IncorrectValue
 from bl_hector.domain.collection_management.value_objects import Isbn
+from bl_hector.interfaces import translate_error
 from bl_hector.interfaces.l10n import DummyTranslator, Translator
 from bl_hector.interfaces.to_terminal import ExitCodes, LookUpBookInterface
 
 
 class LookUpBook(LookUpBookInterface):
     def __init__(
         self,
@@ -72,52 +74,31 @@
         self._ = translator
 
     def not_authorized(self) -> None:
         self.__exit_code = ExitCodes.USAGE
         self.__printer(self._("access-not-authorized"))
 
     def bad_request(self, errors: add_book.Errors) -> None:
-        # TODO: display errors.
         self.__exit_code = ExitCodes.BAD_REQUEST
         self.__printer(self._("book-cannot-be-added"))
+        self.__print_error("book-isbn", errors.isbn)
+        self.__print_error("book-title", errors.title)
+        self.__print_error("book-year", errors.year)
+        self.__print_error("book-authors", errors.authors)
+
+    def __print_error(self, name: str, error: Optional[IncorrectValue]) -> None:
+        if not error:
+            return
+        self.__printer(
+            self._("info-line", name=self._(name), value=translate_error(self._, error))
+        )
 
     def book_already_exists(self, book: Book) -> None:
         self.__exit_code = ExitCodes.BAD_REQUEST
         self.__printer(self._("book-already-exists"))
 
     def book_added(self, book: Book) -> None:
         self.__exit_code = ExitCodes.OK
         self.__printer(self._("book-added"))
 
     def exit_code(self) -> int:
         return self.__exit_code.value
-
-
-class ImportBooks(import_books.Presenter):
-    def __init__(
-        self,
-        printer: Callable[[str], None],
-        # Not l10n… because it might soon be removed!
-        translator: Translator = DummyTranslator(),
-    ) -> None:
-        self.__printer = printer
-        self.__exit_code = ExitCodes.OK
-
-    def file_does_not_exist(self, path: str) -> None:
-        self.__exit_code = ExitCodes.USAGE
-        self.__printer(f"File does not exist: {path}.")
-
-    def line_skipped(self, line_number: int, text: str, reason: str) -> None:
-        self.__exit_code = ExitCodes.USAGE
-        self.__printer(f"Line {line_number} skipped for '{reason}' was '{text}'.")
-
-    def book_already_exists(self, book: Book) -> None:
-        self.__printer(f"Book already in the collection: {book.isbn}.")
-
-    def book_info_not_found(self, isbn: Isbn) -> None:
-        self.__printer(f"No info could be found for '{isbn}'.")
-
-    def book_added(self, book: Book) -> None:
-        self.__printer(f"Book '{book.isbn}' added: \"{book.title}\".")
-
-    def exit_code(self) -> int:
-        return self.__exit_code.value
```

### Comparing `bl_hector-0.1.0a7/bl_hector/interfaces/utils.py` & `bl_hector-0.1.0a8/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a7/pyproject.toml` & `bl_hector-0.1.0a8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.1.0-alpha.7"
+version = "0.1.0-alpha.8"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 exclude = [
     "**/*_spec.py",
```

### Comparing `bl_hector-0.1.0a7/setup.py` & `bl_hector-0.1.0a8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,17 +59,17 @@
 {'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.1.0a7',
+    'version': '0.1.0a8',
     'description': 'A collection manager.',
-    'long_description': '# Hector — a collection manager\n\n## Install\n\nFor the time being, Hector cannot be installed from PyPI.\nSee [CONTRIBUTING.md]() to set up a development environment.\n\n\n## Configure\n\nHector is configured using environment variables.\nAll the variable names are prefixed with `HECTOR_`.\n\n```console\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\nThe secret can be generated using the `token_hex()` function from\nthe Python\'s `secrets` module.\n\nAdditional Python database drivers might be required depending on the DSN.\n\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN=1\n```\n\nTo enable TOTP authentication, you must install extra dependencies (`bl-hector[totp]`)\nand enable it explicitly by setting a base32 random secret (`pyotp.random_base32()`):\n\n```console\n$ export HECTOR_TOTP=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\n```\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n',
+    'long_description': '# Hector — a collection manager\n\n## Install\n\nHector is available on PyPI under the name `bl_hector`.\nTo install, just run `python -m pip install bl_hector`.\n\n\n## Configure\n\nHector is configured using environment variables.\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\nAll the variable names must be prefixed with `HECTOR_`. For instance\xa0:\n\n```console\n# The secret can be generated using the `secrets.token_hex()` function.\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n\n# Additional Python database drivers might be required depending on the DSN.\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN_ENABLED=1\n```\n\nTOTP authentication is provided to be able to login on servers that do not (yet) support\nthe `cryptography` module. You must install extra dependencies (`bl-hector[totp]`)\nand enable it explicitly by setting a base32 random secret:\n\n```console\n# The secret can be generated using the `pyotp.random_base32()` function.\n$ export HECTOR_TOTP_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\n```\n\nNote that it is a highly insecure way of authenticating, as anyone gaining access to your\nOTP generator would be able to login.\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n\n\n## Contributing\n\nSee [CONTRIBUTING.md]() to set up a development environment.\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bl_hector-0.1.0a7/PKG-INFO` & `bl_hector-0.1.0a8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: A collection manager.
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -26,53 +26,57 @@
 Requires-Dist: webauthn (>=1.8.1,<2.0.0); extra == "webauthn"
 Description-Content-Type: text/markdown
 
 # Hector — a collection manager
 
 ## Install
 
-For the time being, Hector cannot be installed from PyPI.
-See [CONTRIBUTING.md]() to set up a development environment.
+Hector is available on PyPI under the name `bl_hector`.
+To install, just run `python -m pip install bl_hector`.
 
 
 ## Configure
 
 Hector is configured using environment variables.
-All the variable names are prefixed with `HECTOR_`.
+See [the `settings` module](bl_hector/infrastructure/settings.py) for
+a comprehensive list of configuration variables.
+
+All the variable names must be prefixed with `HECTOR_`. For instance :
 
 ```console
+# The secret can be generated using the `secrets.token_hex()` function.
 $ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
+
+# Additional Python database drivers might be required depending on the DSN.
 $ export HECTOR_DSN="sqlite:///data.sqlite"
 ```
 
-The secret can be generated using the `token_hex()` function from
-the Python's `secrets` module.
-
-Additional Python database drivers might be required depending on the DSN.
-
-See [the `settings` module](bl_hector/infrastructure/settings.py) for
-a comprehensive list of configuration variables.
-
 
 ## Authentication
 
 To enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)
 and enable it explicitly:
 
 ```console
-$ export HECTOR_WEBAUTHN=1
+$ export HECTOR_WEBAUTHN_ENABLED=1
 ```
 
-To enable TOTP authentication, you must install extra dependencies (`bl-hector[totp]`)
-and enable it explicitly by setting a base32 random secret (`pyotp.random_base32()`):
+TOTP authentication is provided to be able to login on servers that do not (yet) support
+the `cryptography` module. You must install extra dependencies (`bl-hector[totp]`)
+and enable it explicitly by setting a base32 random secret:
 
 ```console
-$ export HECTOR_TOTP=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
+# The secret can be generated using the `pyotp.random_base32()` function.
+$ export HECTOR_TOTP_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
 ```
 
+Note that it is a highly insecure way of authenticating, as anyone gaining access to your
+OTP generator would be able to login.
+
+
 ## Initialise
 
 Once configured, you must initialise Hector's database with the dedicated command:
 
 ```console
 $ hector init-db
 ```
@@ -83,7 +87,12 @@
 Hector being a Flask application, it can be run using any WSGI server,
 for instance, with [Gunicorn](https://gunicorn.org):
 
 ```console
 $ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"
 ```
 
+
+## Contributing
+
+See [CONTRIBUTING.md]() to set up a development environment.
+
```

