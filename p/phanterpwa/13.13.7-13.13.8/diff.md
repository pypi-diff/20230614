# Comparing `tmp/phanterpwa-13.13.7.tar.gz` & `tmp/phanterpwa-13.13.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\phanterpwa-13.13.7.tar", last modified: Fri May 26 19:42:54 2023, max compression
+gzip compressed data, was "dist\phanterpwa-13.13.8.tar", last modified: Wed Jun 14 01:54:18 2023, max compression
```

## Comparing `phanterpwa-13.13.7.tar` & `phanterpwa-13.13.8.tar`

### file list

```diff
@@ -1,568 +1,568 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.506457 phanterpwa-13.13.7/
--rw-rw-rw-   0        0        0     1087 2021-03-14 22:53:21.000000 phanterpwa-13.13.7/LICENSE
--rw-rw-rw-   0        0        0    19227 2023-05-26 19:42:50.000000 phanterpwa-13.13.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1712 2023-05-26 19:42:54.505457 phanterpwa-13.13.7/PKG-INFO
--rw-rw-rw-   0        0        0      456 2021-03-14 22:53:21.000000 phanterpwa-13.13.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.992433 phanterpwa-13.13.7/phanterpwa/
--rw-rw-rw-   0        0        0      397 2023-05-26 13:24:41.000000 phanterpwa-13.13.7/phanterpwa/__init__.py
--rw-rw-rw-   0        0        0     4017 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.041435 phanterpwa-13.13.7/phanterpwa/backend/
--rw-rw-rw-   0        0        0       68 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/backend/__init__.py
--rw-rw-rw-   0        0        0    64543 2023-05-11 14:16:36.000000 phanterpwa-13.13.7/phanterpwa/backend/dataforms.py
--rw-rw-rw-   0        0        0    55413 2023-05-26 13:21:32.000000 phanterpwa-13.13.7/phanterpwa/backend/decorators.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.058428 phanterpwa-13.13.7/phanterpwa/backend/pydal/
--rw-rw-rw-   0        0        0       55 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/backend/pydal/__init__.py
--rw-rw-rw-   0        0        0     8365 2022-05-09 18:31:57.000000 phanterpwa-13.13.7/phanterpwa/backend/pydal/auth.py
--rw-rw-rw-   0        0        0     1581 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/backend/pydal/cas.py
--rw-rw-rw-   0        0        0     2234 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/backend/pydal/credentials.py
--rw-rw-rw-   0        0        0     1919 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/backend/pydal/extra_validations.py
--rw-rw-rw-   0        0        0      870 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/backend/pydal/gallery.py
--rw-rw-rw-   0        0        0     1379 2022-05-11 18:10:28.000000 phanterpwa-13.13.7/phanterpwa/backend/pydal/internal_messages.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.091456 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/__init__.py
--rw-rw-rw-   0        0        0    59625 2023-05-18 13:27:09.000000 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/admin.py
--rw-rw-rw-   0        0        0   167192 2023-05-26 13:10:51.000000 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/auth.py
--rw-rw-rw-   0        0        0    24299 2022-07-06 19:20:32.000000 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/cas.py
--rw-rw-rw-   0        0        0    46299 2022-07-06 19:14:19.000000 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/credentials.py
--rw-rw-rw-   0        0        0     3775 2022-07-06 18:58:48.000000 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/errors.py
--rw-rw-rw-   0        0        0     2490 2021-05-26 06:53:02.000000 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/i18n_server.py
--rw-rw-rw-   0        0        0    15986 2022-07-06 19:19:25.000000 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/internal_messages.py
--rw-rw-rw-   0        0        0    44555 2022-07-06 19:18:59.000000 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/oauth.py
--rw-rw-rw-   0        0        0     5716 2023-05-10 02:32:48.000000 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/websocket.py
--rw-rw-rw-   0        0        0      723 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/backend/request_handlers/welcome.py
--rw-rw-rw-   0        0        0     1300 2022-07-06 19:19:45.000000 phanterpwa-13.13.7/phanterpwa/backend/security.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.494434 phanterpwa-13.13.7/phanterpwa/captchasvg/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/__init__.py
--rw-rw-rw-   0        0        0    12359 2022-07-06 19:12:56.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/captcha.py
--rw-rw-rw-   0        0        0   133091 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/captchadata.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.511435 phanterpwa-13.13.7/phanterpwa/captchasvg/recipes/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/recipes/__init__.py
--rw-rw-rw-   0        0        0       55 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/recipes/circle.recs
--rw-rw-rw-   0        0        0      294 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/recipes/heart.recs
--rw-rw-rw-   0        0        0      131 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/recipes/octagon.recs
--rw-rw-rw-   0        0        0       77 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/recipes/square.recs
--rw-rw-rw-   0        0        0      191 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/recipes/star.recs
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.513435 phanterpwa-13.13.7/phanterpwa/captchasvg/sass/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/sass/__init__.py
--rw-rw-rw-   0        0        0     1137 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/sass/captcha.sass
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.101432 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/
--rw-rw-rw-   0        0        0       71 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.525452 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/animal/
--rw-rw-rw-   0        0        0     1445 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/animal/butterfly.recs
--rw-rw-rw-   0        0        0     3131 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/animal/crab.recs
--rw-rw-rw-   0        0        0     2662 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/animal/pig.recs
--rw-rw-rw-   0        0        0     1424 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/animal/rabbit.recs
--rw-rw-rw-   0        0        0     2968 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/animal/rooster.recs
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.538454 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/arrow/
--rw-rw-rw-   0        0        0      133 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/arrow/down.recs
--rw-rw-rw-   0        0        0      135 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/arrow/left.recs
--rw-rw-rw-   0        0        0      135 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/arrow/right.recs
--rw-rw-rw-   0        0        0      133 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/arrow/up.recs
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.548456 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/letter/
--rw-rw-rw-   0        0        0     1570 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/letter/a.recs
--rw-rw-rw-   0        0        0     1966 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/letter/b.recs
--rw-rw-rw-   0        0        0     1254 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/letter/c.recs
--rw-rw-rw-   0        0        0     1377 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/letter/d.recs
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.559434 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/mean_of_transport/
--rw-rw-rw-   0        0        0     1064 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/mean_of_transport/airplane.recs
--rw-rw-rw-   0        0        0     1863 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/mean_of_transport/car.recs
--rw-rw-rw-   0        0        0     2914 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/mean_of_transport/motorcycle.recs
--rw-rw-rw-   0        0        0      688 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/mean_of_transport/ship.recs
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.571454 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/number/
--rw-rw-rw-   0        0        0     2263 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/number/four.recs
--rw-rw-rw-   0        0        0     1231 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/number/one.recs
--rw-rw-rw-   0        0        0     1940 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/number/three.recs
--rw-rw-rw-   0        0        0     1758 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/number/two.recs
--rw-rw-rw-   0        0        0    47478 2022-04-28 00:32:01.000000 phanterpwa-13.13.7/phanterpwa/compiler.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.118435 phanterpwa-13.13.7/phanterpwa/components/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/__init__.py
--rw-rw-rw-   0        0        0    14007 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/inputs.py
--rw-rw-rw-   0        0        0     6111 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/left_bar.py
--rw-rw-rw-   0        0        0    25523 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/materialize.py
--rw-rw-rw-   0        0        0    19016 2022-02-21 15:44:58.000000 phanterpwa-13.13.7/phanterpwa/components/phanterpwagallery.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.589435 phanterpwa-13.13.7/phanterpwa/components/preloaders/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/__init__.py
--rw-rw-rw-   0        0        0     3584 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/android.py
--rw-rw-rw-   0        0        0     7879 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/android.sass
--rw-rw-rw-   0        0        0     1483 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/discs.py
--rw-rw-rw-   0        0        0     3448 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/discs.sass
--rw-rw-rw-   0        0        0     1116 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/explosion.py
--rw-rw-rw-   0        0        0     5013 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/explosion.sass
--rw-rw-rw-   0        0        0     1460 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/run_points.py
--rw-rw-rw-   0        0        0     3367 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/run_points.sass
--rw-rw-rw-   0        0        0      620 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/square.py
--rw-rw-rw-   0        0        0     1348 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/square.sass
--rw-rw-rw-   0        0        0      828 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/squares.py
--rw-rw-rw-   0        0        0     3862 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/components/preloaders/squares.sass
--rw-rw-rw-   0        0        0    26327 2022-07-06 20:17:07.000000 phanterpwa-13.13.7/phanterpwa/configer.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.185440 phanterpwa-13.13.7/phanterpwa/frontend/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/frontend/__init__.py
--rw-rw-rw-   0        0        0    56787 2023-03-13 15:33:52.000000 phanterpwa-13.13.7/phanterpwa/frontend/application.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.224429 phanterpwa-13.13.7/phanterpwa/frontend/components/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/__init__.py
--rw-rw-rw-   0        0        0    69794 2023-04-16 16:07:37.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/admin.py
--rw-rw-rw-   0        0        0   172952 2023-04-14 17:18:15.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/auth_user.py
--rw-rw-rw-   0        0        0    57394 2022-04-04 10:57:28.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/datetimepicker.py
--rw-rw-rw-   0        0        0     3726 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/events.py
--rw-rw-rw-   0        0        0    34075 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/gallery.py
--rw-rw-rw-   0        0        0    55112 2021-12-06 00:44:42.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/left_bar.py
--rw-rw-rw-   0        0        0     9100 2022-12-05 02:22:50.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/modal.py
--rw-rw-rw-   0        0        0      791 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/pagination.py
--rw-rw-rw-   0        0        0     4060 2021-11-21 02:57:14.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/snippets.py
--rw-rw-rw-   0        0        0     3175 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/top_slide.py
--rw-rw-rw-   0        0        0   231156 2023-04-14 17:13:15.000000 phanterpwa-13.13.7/phanterpwa/frontend/components/widgets.py
--rw-rw-rw-   0        0        0     4042 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/frontend/decorators.py
--rw-rw-rw-   0        0        0    31267 2021-08-01 05:39:42.000000 phanterpwa-13.13.7/phanterpwa/frontend/fmasks.py
--rw-rw-rw-   0        0        0    42583 2023-04-13 14:03:07.000000 phanterpwa-13.13.7/phanterpwa/frontend/forms.py
--rw-rw-rw-   0        0        0    33833 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/frontend/gallery.py
--rw-rw-rw-   0        0        0    14753 2022-04-30 16:30:51.000000 phanterpwa-13.13.7/phanterpwa/frontend/gatehandler.py
--rw-rw-rw-   0        0        0     9861 2023-05-10 01:18:10.000000 phanterpwa-13.13.7/phanterpwa/frontend/helpers.py
--rw-rw-rw-   0        0        0     4593 2022-04-04 10:57:28.000000 phanterpwa-13.13.7/phanterpwa/frontend/i18n.py
--rw-rw-rw-   0        0        0    41699 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/frontend/initializer.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.228432 phanterpwa-13.13.7/phanterpwa/frontend/plugins/
--rw-rw-rw-   0        0        0    27481 2022-11-26 15:07:06.000000 phanterpwa-13.13.7/phanterpwa/frontend/plugins/client.py
--rw-rw-rw-   0        0        0     4927 2022-08-19 19:22:51.000000 phanterpwa-13.13.7/phanterpwa/frontend/preloaders.py
--rw-rw-rw-   0        0        0     1798 2021-11-17 18:30:18.000000 phanterpwa-13.13.7/phanterpwa/frontend/progressbar.py
--rw-rw-rw-   0        0        0     5467 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/frontend/selects.py
--rw-rw-rw-   0        0        0    20671 2023-05-17 17:21:11.000000 phanterpwa-13.13.7/phanterpwa/frontend/server.py
--rw-rw-rw-   0        0        0    10504 2021-11-30 01:36:21.000000 phanterpwa-13.13.7/phanterpwa/frontend/validations.py
--rw-rw-rw-   0        0        0     4381 2022-04-29 11:22:51.000000 phanterpwa-13.13.7/phanterpwa/frontend/websocket.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.241454 phanterpwa-13.13.7/phanterpwa/gallery/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/gallery/__init__.py
--rw-rw-rw-   0        0        0     7220 2022-02-21 15:44:58.000000 phanterpwa-13.13.7/phanterpwa/gallery/cutter.py
--rw-rw-rw-   0        0        0     8578 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/gallery/integrationDAL.py
--rw-rw-rw-   0        0        0    12138 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.244431 phanterpwa-13.13.7/phanterpwa/i18n/
--rw-rw-rw-   0        0        0     8670 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.254435 phanterpwa-13.13.7/phanterpwa/interface/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.591436 phanterpwa-13.13.7/phanterpwa/interface/Admin/
--rw-rw-rw-   0        0        0     1066 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/LICENSE
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.874456 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.269434 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.277432 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/controllers/
--rw-rw-rw-   0        0        0      206 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/controllers/__init__.py
--rw-rw-rw-   0        0        0    29445 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/controllers/developer.py
--rw-rw-rw-   0        0        0      294 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/controllers/welcome.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.639452 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/
--rw-rw-rw-   0        0        0      682 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_activity.table
--rw-rw-rw-   0        0        0      487 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_group.table
--rw-rw-rw-   0        0        0      536 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_membership.table
--rw-rw-rw-   0        0        0     2572 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table
--rw-rw-rw-   0        0        0      793 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user_phanterpwagallery.table
--rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_captcha.table
--rw-rw-rw-   0        0        0      842 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_client.table
--rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_csrf.table
--rw-rw-rw-   0        0        0      597 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_email_user_list.table
--rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_google_captcha.table
--rw-rw-rw-   0        0        0      590 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_phanterpwagallery.table
--rw-rw-rw-   0        0        0      714 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_social_auth.table
--rw-rw-rw-   0        0        0      733 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_two_factor_login.table
--rw-rw-rw-   0        0        0       35 2022-04-26 23:50:37.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/readme.txt
--rw-rw-rw-   0        0        0     4285 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/sql.log
--rw-rw-rw-   0        0        0    81920 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/storage.sqlite
--rw-rw-rw-   0        0        0     6349 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/handlers.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.646451 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.653435 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/admin/
--rw-rw-rw-   0        0        0      807 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/admin/entries.json
--rw-rw-rw-   0        0        0     1541 2021-09-06 05:54:07.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/admin/pt-BR.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.658457 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/captcha/
--rw-rw-rw-   0        0        0      497 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/captcha/entries.json
--rw-rw-rw-   0        0        0     1124 2021-09-06 05:54:07.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/captcha/pt-BR.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.662457 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/email/
--rw-rw-rw-   0        0        0     1577 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/email/entries.json
--rw-rw-rw-   0        0        0     3117 2021-09-06 05:54:07.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/email/pt-BR.json
--rw-rw-rw-   0        0        0     3108 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/entries.json
--rw-rw-rw-   0        0        0     6164 2021-09-06 05:54:07.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/pt-BR.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.279436 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/models/
--rw-rw-rw-   0        0        0      996 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.908456 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/statics/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.668435 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/statics/images/
--rw-rw-rw-   0        0        0    21718 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/statics/images/user.png
--rw-rw-rw-   0        0        0    13499 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/statics/images/warning.png
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.671451 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/uploads/
--rw-rw-rw-   0        0        0       28 2022-04-27 00:31:13.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/uploads/readme.txt
--rw-rw-rw-   0        0        0     2812 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/core.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.281456 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.285457 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/__init__.py
--rw-rw-rw-   0        0        0     1121 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/handlers.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.677453 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/languages/
--rw-rw-rw-   0        0        0     1266 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/languages/entries.json
--rw-rw-rw-   0        0        0     2403 2021-09-06 05:54:07.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/languages/pt-BR.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.909456 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.679458 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/
--rw-rw-rw-   0        0        0     8390 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/application.sass
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.693435 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/
--rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/capcha_preload.sass
--rw-rw-rw-   0        0        0      393 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/logo.sass
--rw-rw-rw-   0        0        0      870 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/phanterpwa-logo.sass
--rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/run_points.sass
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.701434 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/
--rw-rw-rw-   0        0        0     1177 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/components.sass
--rw-rw-rw-   0        0        0      121 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/developer.sass
--rw-rw-rw-   0        0        0      564 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/main.sass
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.293433 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.703436 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/__init__.py
--rw-rw-rw-   0        0        0      785 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/button_preloader.py
--rw-rw-rw-   0        0        0      675 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/captcha_preload.py
--rw-rw-rw-   0        0        0      747 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/css_head.py
--rw-rw-rw-   0        0        0      963 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/favicons.py
--rw-rw-rw-   0        0        0    38183 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/fontawesome.py
--rw-rw-rw-   0        0        0     1272 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/javascript_head.py
--rw-rw-rw-   0        0        0     7459 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/logo.svg
--rw-rw-rw-   0        0        0      158 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/svg_logo.py
--rw-rw-rw-   0        0        0     3267 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/index.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.336436 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/
--rw-rw-rw-   0        0        0    38395 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/fontawesome.py
--rw-rw-rw-   0        0        0     1122 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/phanterpwa_logo.py
--rw-rw-rw-   0        0        0    20765 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/svg_logo.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.340431 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/
--rw-rw-rw-   0        0        0     1363 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/application.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.343434 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/
--rw-rw-rw-   0        0        0      932 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/config.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.374435 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/__init__.py
--rw-rw-rw-   0        0        0     2543 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/cmps.py
--rw-rw-rw-   0        0        0    12805 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/developer.py
--rw-rw-rw-   0        0        0     4692 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/errors.py
--rw-rw-rw-   0        0        0    19789 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/examples.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.390464 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/__init__.py
--rw-rw-rw-   0        0        0    17986 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/inputs.py
--rw-rw-rw-   0        0        0     9456 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/menus.py
--rw-rw-rw-   0        0        0    46491 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/selects.py
--rw-rw-rw-   0        0        0    46731 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/fontawesome.py
--rw-rw-rw-   0        0        0     2600 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/home.py
--rw-rw-rw-   0        0        0    16739 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/project.py
--rw-rw-rw-   0        0        0     5783 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/reqs.py
--rw-rw-rw-   0        0        0     5528 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/testsp.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.395454 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/
--rw-rw-rw-   0        0        0     1502 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/codemirror.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.920458 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.712436 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/css/
--rw-rw-rw-   0        0        0    57333 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/css/all.min.css
--rw-rw-rw-   0        0        0     6138 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/css/normalize.css
--rw-rw-rw-   0        0        0   444223 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/css/phanterpwa.css
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.766452 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/
--rw-rw-rw-   0        0        0    11462 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-144x144.png
--rw-rw-rw-   0        0        0     7107 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-192x192.png
--rw-rw-rw-   0        0        0    19743 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-256x256.png
--rw-rw-rw-   0        0        0    19618 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-512x512.png
--rw-rw-rw-   0        0        0     6233 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/apple-touch-icon.png
--rw-rw-rw-   0        0        0      246 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/browserconfig.xml
--rw-rw-rw-   0        0        0     1209 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-16x16.png
--rw-rw-rw-   0        0        0     1865 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-32x32.png
--rw-rw-rw-   0        0        0    15086 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon.ico
--rw-rw-rw-   0        0        0      268 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/manifest.json
--rw-rw-rw-   0        0        0     5185 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/mstile-150x150.png
--rw-rw-rw-   0        0        0      426 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/site.webmanifest
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.847454 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/
--rw-rw-rw-   0        0        0    46822 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.eot
--rw-rw-rw-   0        0        0    57097 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.svg
--rw-rw-rw-   0        0        0    46592 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.ttf
--rw-rw-rw-   0        0        0    30204 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff
--rw-rw-rw-   0        0        0    25040 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff2
--rw-rw-rw-   0        0        0    12376 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhFq3-OXg.woff2
--rw-rw-rw-   0        0        0    16028 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhLq38.woff2
--rw-rw-rw-   0        0        0    21659 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.eot
--rw-rw-rw-   0        0        0   127584 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0    61628 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff
--rw-rw-rw-   0        0        0    48524 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff2
--rw-rw-rw-   0        0        0    18004 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SQvzA.woff2
--rw-rw-rw-   0        0        0    36060 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SovzAbt.woff2
--rw-rw-rw-   0        0        0    49240 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNc.woff2
--rw-rw-rw-   0        0        0    17854 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.eot
--rw-rw-rw-   0        0        0    48974 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.svg
--rw-rw-rw-   0        0        0    36176 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.ttf
--rw-rw-rw-   0        0        0    20268 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff
--rw-rw-rw-   0        0        0    15736 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.865431 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/images/
--rw-rw-rw-   0        0        0   104800 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/images/background.jpg
--rw-rw-rw-   0        0        0    21718 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/images/user.png
--rw-rw-rw-   0        0        0    13499 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/images/warning.png
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.890431 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/
--rw-rw-rw-   0        0        0    45781 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js
--rw-rw-rw-   0        0        0    43028 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js.map
--rw-rw-rw-   0        0        0      988 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.hammer.js
--rw-rw-rw-   0        0        0    97163 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.js
--rw-rw-rw-   0        0        0   143947 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.map
--rw-rw-rw-   0        0        0    11272 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/touch-emulator.js
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.896453 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/json/
--rw-rw-rw-   0        0        0      517 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.json
--rw-rw-rw-   0        0        0      517 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.webmanifest
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.903447 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/lib/
--rw-rw-rw-   0        0        0     8705 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.css
--rw-rw-rw-   0        0        0   397228 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.js
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.919453 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/mode/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.915435 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/
--rw-rw-rw-   0        0        0     6268 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/index.html
--rw-rw-rw-   0        0        0    14676 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/python.js
--rw-rw-rw-   0        0        0     2014 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/test.js
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.971456 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/
--rw-rw-rw-   0        0        0   133034 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.eot
--rw-rw-rw-   0        0        0   132728 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0        0        0    89824 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff
--rw-rw-rw-   0        0        0    76548 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    34390 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.eot
--rw-rw-rw-   0        0        0    34092 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    16800 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff
--rw-rw-rw-   0        0        0    13600 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   194078 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.eot
--rw-rw-rw-   0        0        0   193792 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0        0        0    99004 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff
--rw-rw-rw-   0        0        0    76120 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff2
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.980451 phanterpwa-13.13.7/phanterpwa/interface/Admin/logs/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/logs/api.log
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/logs/app.log
--rw-rw-rw-   0        0        0       23 2022-04-26 23:49:53.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/logs/readme.txt
--rw-rw-rw-   0        0        0      286 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/production.py
--rw-rw-rw-   0        0        0      145 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/run.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.041433 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/
--rw-rw-rw-   0        0        0     9893 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/_compiler_sass_temp_file.sass
--rw-rw-rw-   0        0        0     1228 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/extends_mtime_admin.json
--rw-rw-rw-   0        0        0      731 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/extends_mtime_components.json
--rw-rw-rw-   0        0        0      865 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/extends_mtime_scaffold_app.json
--rw-rw-rw-   0        0        0      731 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/extends_mtime_sindfa.json
--rw-rw-rw-   0        0        0      221 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/phanterpwa_modules_mtime.json
--rw-rw-rw-   0        0        0        0 2022-04-26 23:56:37.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/readme.txt
--rw-rw-rw-   0        0        0    11082 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/statics_mtime_admin.json
--rw-rw-rw-   0        0        0     8222 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/statics_mtime_components.json
--rw-rw-rw-   0        0        0     8119 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/statics_mtime_scaffold_app.json
--rw-rw-rw-   0        0        0     6140 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/statics_mtime_sindfa.json
--rw-rw-rw-   0        0        0     1369 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/styles_mtime_admin.json
--rw-rw-rw-   0        0        0      592 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/styles_mtime_components.json
--rw-rw-rw-   0        0        0     1075 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/styles_mtime_scaffold_app.json
--rw-rw-rw-   0        0        0     3682 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/styles_mtime_sindfa.json
--rw-rw-rw-   0        0        0      681 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/templates_mtime_admin.json
--rw-rw-rw-   0        0        0      338 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/templates_mtime_components.json
--rw-rw-rw-   0        0        0      474 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/templates_mtime_scaffold_app.json
--rw-rw-rw-   0        0        0      190 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/templates_mtime_sindfa.json
--rw-rw-rw-   0        0        0     2676 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/transcrypts_mtime_admin.json
--rw-rw-rw-   0        0        0      810 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/transcrypts_mtime_components.json
--rw-rw-rw-   0        0        0     1342 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/transcrypts_mtime_scaffold_app.json
--rw-rw-rw-   0        0        0     1127 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/transcrypts_mtime_sindfa.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.043434 phanterpwa-13.13.7/phanterpwa/interface/Admin/trash/
--rw-rw-rw-   0        0        0       20 2022-04-26 23:53:12.000000 phanterpwa-13.13.7/phanterpwa/interface/Admin/trash/readme.txt
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/__init__.py
--rw-rw-rw-   0        0        0     7015 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/admin_tk.py
--rw-rw-rw-   0        0        0    50861 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.049430 phanterpwa-13.13.7/phanterpwa/interface/grafics/
--rw-rw-rw-   0        0        0    15086 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/grafics/icon.ico
--rw-rw-rw-   0        0        0      634 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/grafics/on.jpg
--rw-rw-rw-   0        0        0   140200 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/graphic.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.062429 phanterpwa-13.13.7/phanterpwa/interface/langs/
--rw-rw-rw-   0        0        0     5309 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/langs/English.json
--rw-rw-rw-   0        0        0     5339 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/langs/Portuguese.json
--rw-rw-rw-   0        0        0     2800 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/interface/langs/entries.json
--rw-rw-rw-   0        0        0     5741 2021-09-05 00:25:27.000000 phanterpwa-13.13.7/phanterpwa/mail.py
--rw-rw-rw-   0        0        0    10764 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/reversexml.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.076428 phanterpwa-13.13.7/phanterpwa/samples/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/samples/__init__.py
--rw-rw-rw-   0        0        0      372 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/samples/about_cli
--rw-rw-rw-   0        0        0      269 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/samples/about_graphic
--rw-rw-rw-   0        0        0      533 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/samples/art
--rw-rw-rw-   0        0        0      408 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/samples/art_cli
--rw-rw-rw-   0        0        0     2183 2022-07-06 20:15:09.000000 phanterpwa-13.13.7/phanterpwa/samples/config.json
--rw-rw-rw-   0        0        0     4996 2022-11-26 15:08:21.000000 phanterpwa-13.13.7/phanterpwa/samples/email.sass
--rw-rw-rw-   0        0        0     6072 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/samples/email_activation_code.py
--rw-rw-rw-   0        0        0     5840 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/samples/email_password.py
--rw-rw-rw-   0        0        0     9137 2021-09-05 04:01:49.000000 phanterpwa-13.13.7/phanterpwa/samples/email_two_factor_code.py
--rw-rw-rw-   0        0        0     1879 2022-07-06 20:14:49.000000 phanterpwa-13.13.7/phanterpwa/samples/project_config_sample.py
--rw-rw-rw-   0        0        0      236 2021-09-05 03:59:44.000000 phanterpwa-13.13.7/phanterpwa/samples/sms_activation_code.py
--rw-rw-rw-   0        0        0      245 2021-09-04 16:15:07.000000 phanterpwa-13.13.7/phanterpwa/samples/sms_password.py
--rw-rw-rw-   0        0        0      241 2021-09-04 16:33:02.000000 phanterpwa-13.13.7/phanterpwa/samples/sms_two_factor_code.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.079432 phanterpwa-13.13.7/phanterpwa/scaffolds/
--rw-rw-rw-   0        0        0  2214300 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/scaffolds/Scaffold_PhanterPWA_TM.ppwa
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/scaffolds/__init__.py
--rw-rw-rw-   0        0        0    12247 2022-09-23 00:15:14.000000 phanterpwa-13.13.7/phanterpwa/server.py
--rw-rw-rw-   0        0        0     1313 2021-09-05 16:25:04.000000 phanterpwa-13.13.7/phanterpwa/sms.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.446455 phanterpwa-13.13.7/phanterpwa/tests/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.172452 phanterpwa-13.13.7/phanterpwa/tests/helpers_out/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/helpers_out/__init__.py
--rw-rw-rw-   0        0        0      331 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/helpers_out/my_sass.sass
--rw-rw-rw-   0        0        0      352 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/helpers_out/new_sass.sass
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.184452 phanterpwa-13.13.7/phanterpwa/tests/path_of_languages/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/path_of_languages/__init__.py
--rw-rw-rw-   0        0        0      456 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/path_of_languages/entries.json
--rw-rw-rw-   0        0        0      854 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/path_of_languages/es.json
--rw-rw-rw-   0        0        0      852 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/path_of_languages/fr.json
--rw-rw-rw-   0        0        0      860 2021-09-06 05:54:07.000000 phanterpwa-13.13.7/phanterpwa/tests/path_of_languages/pt-BR.json
--rw-rw-rw-   0        0        0      851 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/path_of_languages/pt-PT.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.202458 phanterpwa-13.13.7/phanterpwa/tests/preloaders/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/preloaders/__init__.py
--rw-rw-rw-   0        0        0     9764 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_android.html
--rw-rw-rw-   0        0        0     3489 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_discs.html
--rw-rw-rw-   0        0        0     5956 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_explosion.html
--rw-rw-rw-   0        0        0     4451 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_run_points.html
--rw-rw-rw-   0        0        0     1752 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_square.html
--rw-rw-rw-   0        0        0     4231 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_squares.html
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.211481 phanterpwa-13.13.7/phanterpwa/tests/static/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/static/__init__.py
--rw-rw-rw-   0        0        0    97163 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/static/jquery.min.js
--rw-rw-rw-   0        0        0   143947 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/static/jquery.min.map
--rw-rw-rw-   0        0        0     2117 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_cli.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.455458 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.217435 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/not_project/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/not_project/__init__.py
--rw-rw-rw-   0        0        0       40 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/not_project/config.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.219443 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/project-invalid-name/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/project-invalid-name/__init__.py
--rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/project-invalid-name/config.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.221452 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/project01/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/project01/__init__.py
--rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/project01/config.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.223458 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/project02/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/project02/__init__.py
--rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/project02/config.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.467436 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/without_configjson/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_cli_projects/without_configjson/__init__.py
--rw-rw-rw-   0        0        0     4079 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_components_preloaders.py
--rw-rw-rw-   0        0        0    12208 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.469434 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.226430 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/fake_project/
--rw-rw-rw-   0        0        0       40 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/fake_project/config.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.228429 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project-invalid-name/
--rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project-invalid-name/config.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.235435 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.926464 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/backapps/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.237434 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/backapps/api/
--rw-rw-rw-   0        0        0      629 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/backapps/api/app.ini
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.927466 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/backend/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.239434 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/backend/api/
--rw-rw-rw-   0        0        0      629 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/backend/api/app.ini
--rw-rw-rw-   0        0        0     2618 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/config.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.931471 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/frontapps/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.242433 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/frontapps/app01/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/frontapps/app01/app.ini
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.244432 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/frontapps/app02/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/frontapps/app02/app.ini
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.933457 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/frontend/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.246435 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/frontend/app01/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/frontend/app01/app.ini
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.248430 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/frontend/app02/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/frontend/app02/app.ini
--rw-rw-rw-   0        0        0      189 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/project.ini
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.252436 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project02/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project02/__init__.py
--rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project02/config.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.259435 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.934454 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.261440 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/
--rw-rw-rw-   0        0        0      843 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/app.ini
--rw-rw-rw-   0        0        0     2143 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/config.json
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.936466 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.263432 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app01/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app01/app.ini
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.266455 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app02/
--rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app02/app.ini
--rw-rw-rw-   0        0        0      149 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/project.ini
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.270452 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_ini/
--rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_ini/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:52.937456 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_ini/backend/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.272454 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/
--rw-rw-rw-   0        0        0      843 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/app.ini
--rw-rw-rw-   0        0        0     2640 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_ini/config.json
--rw-rw-rw-   0        0        0      149 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_ini/project.ini
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.279432 phanterpwa-13.13.7/phanterpwa/tests/test_folder/
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_folder/cfg.json
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_folder/cfgij.json
--rw-rw-rw-   0        0        0       23 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_folder/config.json
--rw-rw-rw-   0        0        0    80202 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.288453 phanterpwa-13.13.7/phanterpwa/tests/test_helpers_languages/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_helpers_languages/__init__.py
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_helpers_languages/en-US.json
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_helpers_languages/entries.json
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_helpers_languages/glingon.json
--rw-rw-rw-   0        0        0        2 2021-09-06 05:54:07.000000 phanterpwa-13.13.7/phanterpwa/tests/test_helpers_languages/pt-BR.json
--rw-rw-rw-   0        0        0     3729 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_i18n.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.297428 phanterpwa-13.13.7/phanterpwa/tests/test_i18n_languages/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_i18n_languages/__init__.py
--rw-rw-rw-   0        0        0       65 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_i18n_languages/en-US.json
--rw-rw-rw-   0        0        0       36 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_i18n_languages/entries.json
--rw-rw-rw-   0        0        0       63 2021-09-06 05:54:07.000000 phanterpwa-13.13.7/phanterpwa/tests/test_i18n_languages/pt-BR.json
--rw-rw-rw-   0        0        0       63 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_i18n_languages/pt-PT.json
--rw-rw-rw-   0        0        0     4212 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_reversexml.py
--rw-rw-rw-   0        0        0    11521 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_tools.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.301428 phanterpwa-13.13.7/phanterpwa/tests/test_tools_humanize_seconds/
--rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/test_tools_humanize_seconds/entries.json
--rw-rw-rw-   0        0        0        2 2021-09-06 05:54:07.000000 phanterpwa-13.13.7/phanterpwa/tests/test_tools_humanize_seconds/pt-BR.json
--rw-rw-rw-   0        0        0     1386 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/tests/tests.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.492435 phanterpwa-13.13.7/phanterpwa/third_parties/
--rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/third_parties/__init__.py
--rw-rw-rw-   0        0        0     5857 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/third_parties/xss.py
--rw-rw-rw-   0        0        0    45683 2022-04-27 18:34:47.000000 phanterpwa-13.13.7/phanterpwa/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.303453 phanterpwa-13.13.7/phanterpwa/trash/
--rw-rw-rw-   0        0        0       20 2022-04-26 23:53:12.000000 phanterpwa-13.13.7/phanterpwa/trash/readme.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.308455 phanterpwa-13.13.7/phanterpwa/usual_sass/
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.423431 phanterpwa-13.13.7/phanterpwa/usual_sass/components/
--rw-rw-rw-   0        0        0     1794 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/alert_top_activation.sass
--rw-rw-rw-   0        0        0     1551 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/breascrumbs.sass
--rw-rw-rw-   0        0        0     2741 2021-07-27 18:35:01.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/buttons.sass
--rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/capcha_preload.sass
--rw-rw-rw-   0        0        0     7323 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/captcha.sass
--rw-rw-rw-   0        0        0     5213 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/captcha_preload_image_3x4.sass
--rw-rw-rw-   0        0        0      643 2022-11-25 21:37:56.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/card.sass
--rw-rw-rw-   0        0        0    13548 2022-04-04 10:57:28.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/cmp_auth_user.sass
--rw-rw-rw-   0        0        0     6615 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/datetimepicker.sass
--rw-rw-rw-   0        0        0     1741 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/developer.sass
--rw-rw-rw-   0        0        0     3154 2022-06-07 17:05:55.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/easy.sass
--rw-rw-rw-   0        0        0     1067 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/flash.sass
--rw-rw-rw-   0        0        0     2937 2022-04-27 17:07:49.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/forms.sass
--rw-rw-rw-   0        0        0     1888 2022-05-17 18:44:18.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/messages.sass
--rw-rw-rw-   0        0        0     3190 2022-04-04 10:57:28.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/modal.sass
--rw-rw-rw-   0        0        0     1694 2021-09-05 18:33:48.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/modal_login.sass
--rw-rw-rw-   0        0        0      649 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/phanterpwa_gallery.sass
--rw-rw-rw-   0        0        0     4103 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/phanterpwa_gallery_cutter.sass
--rw-rw-rw-   0        0        0     1450 2021-08-13 03:26:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/phanterpwa_panel_control.sass
--rw-rw-rw-   0        0        0     2959 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/progressbar.sass
--rw-rw-rw-   0        0        0      660 2022-02-03 09:45:15.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/pseudomodal.sass
--rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/run_points.sass
--rw-rw-rw-   0        0        0     1536 2021-06-17 02:27:21.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/sections.sass
--rw-rw-rw-   0        0        0      811 2021-05-25 20:28:47.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/snippet.sass
--rw-rw-rw-   0        0        0    79319 2023-01-26 13:45:09.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/widgets.sass
--rw-rw-rw-   0        0        0     4968 2021-06-15 20:39:00.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/components/xtable.sass
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.435457 phanterpwa-13.13.7/phanterpwa/usual_sass/display/
--rw-rw-rw-   0        0        0    42388 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/display/grid.sass
--rw-rw-rw-   0        0        0     3962 2021-12-14 21:24:18.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/display/media_print.sass
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.441430 phanterpwa-13.13.7/phanterpwa/usual_sass/events/
--rw-rw-rw-   0        0        0      238 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/events/waves.sass
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.457439 phanterpwa-13.13.7/phanterpwa/usual_sass/extends/
--rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/extends/capcha_preload.sass
--rw-rw-rw-   0        0        0      393 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/extends/logo.sass
--rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/extends/run_points.sass
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.466457 phanterpwa-13.13.7/phanterpwa/usual_sass/gates/
--rw-rw-rw-   0        0        0      865 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/gates/componentes.sass
--rw-rw-rw-   0        0        0      631 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/gates/main.sass
--rw-rw-rw-   0        0        0     9456 2023-01-22 22:50:53.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/phanterpwa.sass
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.470435 phanterpwa-13.13.7/phanterpwa/usual_sass/plugins/
--rw-rw-rw-   0        0        0      153 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/plugins/codemirror.sass
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:54.499455 phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/
--rw-rw-rw-   0        0        0     7879 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/android.sass
--rw-rw-rw-   0        0        0     3448 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/discs.sass
--rw-rw-rw-   0        0        0     5013 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/explosion.sass
--rw-rw-rw-   0        0        0      954 2022-08-19 19:22:51.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/indefined_text.sass
--rw-rw-rw-   0        0        0     3367 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/run_points.sass
--rw-rw-rw-   0        0        0     1348 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/square.sass
--rw-rw-rw-   0        0        0     3862 2021-05-19 23:34:10.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/squares.sass
--rw-rw-rw-   0        0        0     8645 2022-04-27 17:07:49.000000 phanterpwa-13.13.7/phanterpwa/usual_sass/variables.sass
--rw-rw-rw-   0        0        0   162695 2023-02-02 15:14:57.000000 phanterpwa-13.13.7/phanterpwa/xmlconstructor.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:42:53.008440 phanterpwa-13.13.7/phanterpwa.egg-info/
--rw-rw-rw-   0        0        0     1712 2023-05-26 19:42:51.000000 phanterpwa-13.13.7/phanterpwa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    25133 2023-05-26 19:42:52.000000 phanterpwa-13.13.7/phanterpwa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2023-05-26 19:42:51.000000 phanterpwa-13.13.7/phanterpwa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-26 19:42:51.000000 phanterpwa-13.13.7/phanterpwa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-26 19:42:51.000000 phanterpwa-13.13.7/phanterpwa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      122 2023-05-26 19:42:52.000000 phanterpwa-13.13.7/phanterpwa.egg-info/requires.txt
--rw-rw-rw-   0        0        0     5319 2023-05-26 19:42:52.000000 phanterpwa-13.13.7/phanterpwa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 19:42:54.506457 phanterpwa-13.13.7/setup.cfg
--rw-rw-rw-   0        0        0     4419 2022-07-15 11:22:48.000000 phanterpwa-13.13.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.866434 phanterpwa-13.13.8/
+-rw-rw-rw-   0        0        0     1087 2021-03-14 22:53:21.000000 phanterpwa-13.13.8/LICENSE
+-rw-rw-rw-   0        0        0    19227 2023-06-14 01:54:12.000000 phanterpwa-13.13.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1712 2023-06-14 01:54:18.865431 phanterpwa-13.13.8/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2021-03-14 22:53:21.000000 phanterpwa-13.13.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.647432 phanterpwa-13.13.8/phanterpwa/
+-rw-rw-rw-   0        0        0      397 2023-06-14 01:52:32.000000 phanterpwa-13.13.8/phanterpwa/__init__.py
+-rw-rw-rw-   0        0        0     4017 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.688432 phanterpwa-13.13.8/phanterpwa/backend/
+-rw-rw-rw-   0        0        0       68 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/backend/__init__.py
+-rw-rw-rw-   0        0        0    64543 2023-05-11 14:16:36.000000 phanterpwa-13.13.8/phanterpwa/backend/dataforms.py
+-rw-rw-rw-   0        0        0    55413 2023-05-26 13:21:32.000000 phanterpwa-13.13.8/phanterpwa/backend/decorators.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.712430 phanterpwa-13.13.8/phanterpwa/backend/pydal/
+-rw-rw-rw-   0        0        0       55 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/backend/pydal/__init__.py
+-rw-rw-rw-   0        0        0     8365 2022-05-09 18:31:57.000000 phanterpwa-13.13.8/phanterpwa/backend/pydal/auth.py
+-rw-rw-rw-   0        0        0     1581 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/backend/pydal/cas.py
+-rw-rw-rw-   0        0        0     2234 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/backend/pydal/credentials.py
+-rw-rw-rw-   0        0        0     1919 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/backend/pydal/extra_validations.py
+-rw-rw-rw-   0        0        0      870 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/backend/pydal/gallery.py
+-rw-rw-rw-   0        0        0     1379 2022-05-11 18:10:28.000000 phanterpwa-13.13.8/phanterpwa/backend/pydal/internal_messages.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.755431 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/__init__.py
+-rw-rw-rw-   0        0        0    59625 2023-05-18 13:27:09.000000 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/admin.py
+-rw-rw-rw-   0        0        0   167192 2023-05-26 13:10:51.000000 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/auth.py
+-rw-rw-rw-   0        0        0    24299 2022-07-06 19:20:32.000000 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/cas.py
+-rw-rw-rw-   0        0        0    46299 2022-07-06 19:14:19.000000 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/credentials.py
+-rw-rw-rw-   0        0        0     3775 2022-07-06 18:58:48.000000 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/errors.py
+-rw-rw-rw-   0        0        0     2490 2021-05-26 06:53:02.000000 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/i18n_server.py
+-rw-rw-rw-   0        0        0    15986 2022-07-06 19:19:25.000000 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/internal_messages.py
+-rw-rw-rw-   0        0        0    44555 2022-07-06 19:18:59.000000 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/oauth.py
+-rw-rw-rw-   0        0        0     5716 2023-05-10 02:32:48.000000 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/websocket.py
+-rw-rw-rw-   0        0        0      723 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/backend/request_handlers/welcome.py
+-rw-rw-rw-   0        0        0     1300 2022-07-06 19:19:45.000000 phanterpwa-13.13.8/phanterpwa/backend/security.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.259433 phanterpwa-13.13.8/phanterpwa/captchasvg/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/__init__.py
+-rw-rw-rw-   0        0        0    12359 2022-07-06 19:12:56.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/captcha.py
+-rw-rw-rw-   0        0        0   133091 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/captchadata.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.289431 phanterpwa-13.13.8/phanterpwa/captchasvg/recipes/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/recipes/__init__.py
+-rw-rw-rw-   0        0        0       55 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/recipes/circle.recs
+-rw-rw-rw-   0        0        0      294 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/recipes/heart.recs
+-rw-rw-rw-   0        0        0      131 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/recipes/octagon.recs
+-rw-rw-rw-   0        0        0       77 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/recipes/square.recs
+-rw-rw-rw-   0        0        0      191 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/recipes/star.recs
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.293444 phanterpwa-13.13.8/phanterpwa/captchasvg/sass/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/sass/__init__.py
+-rw-rw-rw-   0        0        0     1137 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/sass/captcha.sass
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.774404 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/
+-rw-rw-rw-   0        0        0       71 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.331431 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/animal/
+-rw-rw-rw-   0        0        0     1445 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/animal/butterfly.recs
+-rw-rw-rw-   0        0        0     3131 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/animal/crab.recs
+-rw-rw-rw-   0        0        0     2662 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/animal/pig.recs
+-rw-rw-rw-   0        0        0     1424 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/animal/rabbit.recs
+-rw-rw-rw-   0        0        0     2968 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/animal/rooster.recs
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.353409 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/arrow/
+-rw-rw-rw-   0        0        0      133 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/arrow/down.recs
+-rw-rw-rw-   0        0        0      135 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/arrow/left.recs
+-rw-rw-rw-   0        0        0      135 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/arrow/right.recs
+-rw-rw-rw-   0        0        0      133 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/arrow/up.recs
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.382405 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/letter/
+-rw-rw-rw-   0        0        0     1570 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/letter/a.recs
+-rw-rw-rw-   0        0        0     1966 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/letter/b.recs
+-rw-rw-rw-   0        0        0     1254 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/letter/c.recs
+-rw-rw-rw-   0        0        0     1377 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/letter/d.recs
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.421430 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/mean_of_transport/
+-rw-rw-rw-   0        0        0     1064 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/mean_of_transport/airplane.recs
+-rw-rw-rw-   0        0        0     1863 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/mean_of_transport/car.recs
+-rw-rw-rw-   0        0        0     2914 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/mean_of_transport/motorcycle.recs
+-rw-rw-rw-   0        0        0      688 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/mean_of_transport/ship.recs
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.453405 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/number/
+-rw-rw-rw-   0        0        0     2263 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/number/four.recs
+-rw-rw-rw-   0        0        0     1231 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/number/one.recs
+-rw-rw-rw-   0        0        0     1940 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/number/three.recs
+-rw-rw-rw-   0        0        0     1758 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/number/two.recs
+-rw-rw-rw-   0        0        0    47478 2022-04-28 00:32:01.000000 phanterpwa-13.13.8/phanterpwa/compiler.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.792405 phanterpwa-13.13.8/phanterpwa/components/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/__init__.py
+-rw-rw-rw-   0        0        0    14007 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/inputs.py
+-rw-rw-rw-   0        0        0     6111 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/left_bar.py
+-rw-rw-rw-   0        0        0    25523 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/materialize.py
+-rw-rw-rw-   0        0        0    19016 2022-02-21 15:44:58.000000 phanterpwa-13.13.8/phanterpwa/components/phanterpwagallery.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.475406 phanterpwa-13.13.8/phanterpwa/components/preloaders/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/__init__.py
+-rw-rw-rw-   0        0        0     3584 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/android.py
+-rw-rw-rw-   0        0        0     7879 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/android.sass
+-rw-rw-rw-   0        0        0     1483 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/discs.py
+-rw-rw-rw-   0        0        0     3448 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/discs.sass
+-rw-rw-rw-   0        0        0     1116 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/explosion.py
+-rw-rw-rw-   0        0        0     5013 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/explosion.sass
+-rw-rw-rw-   0        0        0     1460 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/run_points.py
+-rw-rw-rw-   0        0        0     3367 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/run_points.sass
+-rw-rw-rw-   0        0        0      620 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/square.py
+-rw-rw-rw-   0        0        0     1348 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/square.sass
+-rw-rw-rw-   0        0        0      828 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/squares.py
+-rw-rw-rw-   0        0        0     3862 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/components/preloaders/squares.sass
+-rw-rw-rw-   0        0        0    26327 2022-07-06 20:17:07.000000 phanterpwa-13.13.8/phanterpwa/configer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.878433 phanterpwa-13.13.8/phanterpwa/frontend/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/frontend/__init__.py
+-rw-rw-rw-   0        0        0    56787 2023-03-13 15:33:52.000000 phanterpwa-13.13.8/phanterpwa/frontend/application.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.924405 phanterpwa-13.13.8/phanterpwa/frontend/components/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/__init__.py
+-rw-rw-rw-   0        0        0    69794 2023-04-16 16:07:37.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/admin.py
+-rw-rw-rw-   0        0        0   172952 2023-04-14 17:18:15.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/auth_user.py
+-rw-rw-rw-   0        0        0    57394 2022-04-04 10:57:28.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/datetimepicker.py
+-rw-rw-rw-   0        0        0     3726 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/events.py
+-rw-rw-rw-   0        0        0    34075 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/gallery.py
+-rw-rw-rw-   0        0        0    55112 2021-12-06 00:44:42.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/left_bar.py
+-rw-rw-rw-   0        0        0     9100 2022-12-05 02:22:50.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/modal.py
+-rw-rw-rw-   0        0        0      791 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/pagination.py
+-rw-rw-rw-   0        0        0     4060 2021-11-21 02:57:14.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/snippets.py
+-rw-rw-rw-   0        0        0     3175 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/top_slide.py
+-rw-rw-rw-   0        0        0   231206 2023-06-14 01:51:48.000000 phanterpwa-13.13.8/phanterpwa/frontend/components/widgets.py
+-rw-rw-rw-   0        0        0     4042 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/frontend/decorators.py
+-rw-rw-rw-   0        0        0    31267 2021-08-01 05:39:42.000000 phanterpwa-13.13.8/phanterpwa/frontend/fmasks.py
+-rw-rw-rw-   0        0        0    42588 2023-06-14 01:51:48.000000 phanterpwa-13.13.8/phanterpwa/frontend/forms.py
+-rw-rw-rw-   0        0        0    33833 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/frontend/gallery.py
+-rw-rw-rw-   0        0        0    14753 2022-04-30 16:30:51.000000 phanterpwa-13.13.8/phanterpwa/frontend/gatehandler.py
+-rw-rw-rw-   0        0        0     9861 2023-05-10 01:18:10.000000 phanterpwa-13.13.8/phanterpwa/frontend/helpers.py
+-rw-rw-rw-   0        0        0     4593 2022-04-04 10:57:28.000000 phanterpwa-13.13.8/phanterpwa/frontend/i18n.py
+-rw-rw-rw-   0        0        0    41699 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/frontend/initializer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.928434 phanterpwa-13.13.8/phanterpwa/frontend/plugins/
+-rw-rw-rw-   0        0        0    27481 2022-11-26 15:07:06.000000 phanterpwa-13.13.8/phanterpwa/frontend/plugins/client.py
+-rw-rw-rw-   0        0        0     4927 2022-08-19 19:22:51.000000 phanterpwa-13.13.8/phanterpwa/frontend/preloaders.py
+-rw-rw-rw-   0        0        0     1798 2021-11-17 18:30:18.000000 phanterpwa-13.13.8/phanterpwa/frontend/progressbar.py
+-rw-rw-rw-   0        0        0     5467 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/frontend/selects.py
+-rw-rw-rw-   0        0        0    20671 2023-05-17 17:21:11.000000 phanterpwa-13.13.8/phanterpwa/frontend/server.py
+-rw-rw-rw-   0        0        0    10504 2021-11-30 01:36:21.000000 phanterpwa-13.13.8/phanterpwa/frontend/validations.py
+-rw-rw-rw-   0        0        0     4381 2022-04-29 11:22:51.000000 phanterpwa-13.13.8/phanterpwa/frontend/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.939432 phanterpwa-13.13.8/phanterpwa/gallery/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/gallery/__init__.py
+-rw-rw-rw-   0        0        0     7220 2022-02-21 15:44:58.000000 phanterpwa-13.13.8/phanterpwa/gallery/cutter.py
+-rw-rw-rw-   0        0        0     8578 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/gallery/integrationDAL.py
+-rw-rw-rw-   0        0        0    12138 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.943409 phanterpwa-13.13.8/phanterpwa/i18n/
+-rw-rw-rw-   0        0        0     8670 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.959433 phanterpwa-13.13.8/phanterpwa/interface/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.484426 phanterpwa-13.13.8/phanterpwa/interface/Admin/
+-rw-rw-rw-   0        0        0     1066 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/LICENSE
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.475411 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.982432 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.992405 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/controllers/
+-rw-rw-rw-   0        0        0      206 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/controllers/__init__.py
+-rw-rw-rw-   0        0        0    29445 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/controllers/developer.py
+-rw-rw-rw-   0        0        0      294 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/controllers/welcome.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.585404 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/
+-rw-rw-rw-   0        0        0      682 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_activity.table
+-rw-rw-rw-   0        0        0      487 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_group.table
+-rw-rw-rw-   0        0        0      536 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_membership.table
+-rw-rw-rw-   0        0        0     2572 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table
+-rw-rw-rw-   0        0        0      793 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user_phanterpwagallery.table
+-rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_captcha.table
+-rw-rw-rw-   0        0        0      842 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_client.table
+-rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_csrf.table
+-rw-rw-rw-   0        0        0      597 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_email_user_list.table
+-rw-rw-rw-   0        0        0      847 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_google_captcha.table
+-rw-rw-rw-   0        0        0      590 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_phanterpwagallery.table
+-rw-rw-rw-   0        0        0      714 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_social_auth.table
+-rw-rw-rw-   0        0        0      733 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_two_factor_login.table
+-rw-rw-rw-   0        0        0       35 2022-04-26 23:50:37.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/readme.txt
+-rw-rw-rw-   0        0        0     4285 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/sql.log
+-rw-rw-rw-   0        0        0    81920 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/storage.sqlite
+-rw-rw-rw-   0        0        0     6349 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.593430 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.601430 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/admin/
+-rw-rw-rw-   0        0        0      807 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/admin/entries.json
+-rw-rw-rw-   0        0        0     1541 2021-09-06 05:54:07.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/admin/pt-BR.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.608405 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/captcha/
+-rw-rw-rw-   0        0        0      497 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/captcha/entries.json
+-rw-rw-rw-   0        0        0     1124 2021-09-06 05:54:07.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/captcha/pt-BR.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.615429 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/email/
+-rw-rw-rw-   0        0        0     1577 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/email/entries.json
+-rw-rw-rw-   0        0        0     3117 2021-09-06 05:54:07.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/email/pt-BR.json
+-rw-rw-rw-   0        0        0     3108 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/entries.json
+-rw-rw-rw-   0        0        0     6164 2021-09-06 05:54:07.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/pt-BR.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.996432 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/models/
+-rw-rw-rw-   0        0        0      996 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.528429 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/statics/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.629405 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/statics/images/
+-rw-rw-rw-   0        0        0    21718 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/statics/images/user.png
+-rw-rw-rw-   0        0        0    13499 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/statics/images/warning.png
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.634405 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/uploads/
+-rw-rw-rw-   0        0        0       28 2022-04-27 00:31:13.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/uploads/readme.txt
+-rw-rw-rw-   0        0        0     2812 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/core.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.999432 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.007406 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/__init__.py
+-rw-rw-rw-   0        0        0     1121 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.642430 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/languages/
+-rw-rw-rw-   0        0        0     1266 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/languages/entries.json
+-rw-rw-rw-   0        0        0     2403 2021-09-06 05:54:07.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/languages/pt-BR.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.531431 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.646405 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/
+-rw-rw-rw-   0        0        0     8390 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/application.sass
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.660431 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/
+-rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/capcha_preload.sass
+-rw-rw-rw-   0        0        0      393 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/logo.sass
+-rw-rw-rw-   0        0        0      870 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/phanterpwa-logo.sass
+-rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/run_points.sass
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.671430 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/
+-rw-rw-rw-   0        0        0     1177 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/components.sass
+-rw-rw-rw-   0        0        0      121 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/developer.sass
+-rw-rw-rw-   0        0        0      564 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/main.sass
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.014405 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.674428 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/__init__.py
+-rw-rw-rw-   0        0        0      785 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/button_preloader.py
+-rw-rw-rw-   0        0        0      675 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/captcha_preload.py
+-rw-rw-rw-   0        0        0      747 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/css_head.py
+-rw-rw-rw-   0        0        0      963 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/favicons.py
+-rw-rw-rw-   0        0        0    38183 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/fontawesome.py
+-rw-rw-rw-   0        0        0     1272 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/javascript_head.py
+-rw-rw-rw-   0        0        0     7459 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/logo.svg
+-rw-rw-rw-   0        0        0      158 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/svg_logo.py
+-rw-rw-rw-   0        0        0     3267 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.055431 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/
+-rw-rw-rw-   0        0        0    38395 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/fontawesome.py
+-rw-rw-rw-   0        0        0     1122 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/phanterpwa_logo.py
+-rw-rw-rw-   0        0        0    20765 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/svg_logo.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.060431 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/
+-rw-rw-rw-   0        0        0     1363 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/application.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.063434 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/
+-rw-rw-rw-   0        0        0      932 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/config.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.102403 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/__init__.py
+-rw-rw-rw-   0        0        0     2543 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/cmps.py
+-rw-rw-rw-   0        0        0    12805 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/developer.py
+-rw-rw-rw-   0        0        0     4692 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/errors.py
+-rw-rw-rw-   0        0        0    19789 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/examples.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.118404 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/__init__.py
+-rw-rw-rw-   0        0        0    17986 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/inputs.py
+-rw-rw-rw-   0        0        0     9456 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/menus.py
+-rw-rw-rw-   0        0        0    46491 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/selects.py
+-rw-rw-rw-   0        0        0    46731 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/fontawesome.py
+-rw-rw-rw-   0        0        0     2600 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/home.py
+-rw-rw-rw-   0        0        0    16739 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/project.py
+-rw-rw-rw-   0        0        0     5783 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/reqs.py
+-rw-rw-rw-   0        0        0     5528 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/testsp.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.122405 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/
+-rw-rw-rw-   0        0        0     1502 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/codemirror.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.547431 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.687430 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/
+-rw-rw-rw-   0        0        0    57333 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/all.min.css
+-rw-rw-rw-   0        0        0     6138 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/normalize.css
+-rw-rw-rw-   0        0        0   444223 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/phanterpwa.css
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.775405 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/
+-rw-rw-rw-   0        0        0    11462 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-144x144.png
+-rw-rw-rw-   0        0        0     7107 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-192x192.png
+-rw-rw-rw-   0        0        0    19743 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-256x256.png
+-rw-rw-rw-   0        0        0    19618 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-512x512.png
+-rw-rw-rw-   0        0        0     6233 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      246 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/browserconfig.xml
+-rw-rw-rw-   0        0        0     1209 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-16x16.png
+-rw-rw-rw-   0        0        0     1865 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-32x32.png
+-rw-rw-rw-   0        0        0    15086 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon.ico
+-rw-rw-rw-   0        0        0      268 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/manifest.json
+-rw-rw-rw-   0        0        0     5185 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/mstile-150x150.png
+-rw-rw-rw-   0        0        0      426 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/site.webmanifest
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.938432 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/
+-rw-rw-rw-   0        0        0    46822 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.eot
+-rw-rw-rw-   0        0        0    57097 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.svg
+-rw-rw-rw-   0        0        0    46592 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.ttf
+-rw-rw-rw-   0        0        0    30204 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff
+-rw-rw-rw-   0        0        0    25040 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff2
+-rw-rw-rw-   0        0        0    12376 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhFq3-OXg.woff2
+-rw-rw-rw-   0        0        0    16028 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhLq38.woff2
+-rw-rw-rw-   0        0        0    21659 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.eot
+-rw-rw-rw-   0        0        0   127584 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0    61628 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff
+-rw-rw-rw-   0        0        0    48524 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff2
+-rw-rw-rw-   0        0        0    18004 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SQvzA.woff2
+-rw-rw-rw-   0        0        0    36060 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SovzAbt.woff2
+-rw-rw-rw-   0        0        0    49240 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNc.woff2
+-rw-rw-rw-   0        0        0    17854 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.eot
+-rw-rw-rw-   0        0        0    48974 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.svg
+-rw-rw-rw-   0        0        0    36176 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.ttf
+-rw-rw-rw-   0        0        0    20268 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff
+-rw-rw-rw-   0        0        0    15736 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.965404 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/
+-rw-rw-rw-   0        0        0   104800 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/background.jpg
+-rw-rw-rw-   0        0        0    21718 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/user.png
+-rw-rw-rw-   0        0        0    13499 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/warning.png
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.003434 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/
+-rw-rw-rw-   0        0        0    45781 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js
+-rw-rw-rw-   0        0        0    43028 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js.map
+-rw-rw-rw-   0        0        0      988 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.hammer.js
+-rw-rw-rw-   0        0        0    97163 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.js
+-rw-rw-rw-   0        0        0   143947 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.map
+-rw-rw-rw-   0        0        0    11272 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/touch-emulator.js
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.012404 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/json/
+-rw-rw-rw-   0        0        0      517 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.json
+-rw-rw-rw-   0        0        0      517 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.webmanifest
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.020427 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/lib/
+-rw-rw-rw-   0        0        0     8705 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.css
+-rw-rw-rw-   0        0        0   397228 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.js
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.546431 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.032431 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/
+-rw-rw-rw-   0        0        0     6268 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/index.html
+-rw-rw-rw-   0        0        0    14676 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/python.js
+-rw-rw-rw-   0        0        0     2014 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/test.js
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.149403 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/
+-rw-rw-rw-   0        0        0   133034 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0        0        0   132728 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0    89824 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0        0        0    76548 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    34390 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0        0        0    34092 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    16800 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0        0        0    13600 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   194078 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0        0        0   193792 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0    99004 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0        0        0    76120 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff2
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.164404 phanterpwa-13.13.8/phanterpwa/interface/Admin/logs/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/logs/api.log
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/logs/app.log
+-rw-rw-rw-   0        0        0       23 2022-04-26 23:49:53.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/logs/readme.txt
+-rw-rw-rw-   0        0        0      286 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/production.py
+-rw-rw-rw-   0        0        0      145 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/run.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.254405 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/
+-rw-rw-rw-   0        0        0     9893 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/_compiler_sass_temp_file.sass
+-rw-rw-rw-   0        0        0     1228 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/extends_mtime_admin.json
+-rw-rw-rw-   0        0        0      731 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/extends_mtime_components.json
+-rw-rw-rw-   0        0        0      865 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/extends_mtime_scaffold_app.json
+-rw-rw-rw-   0        0        0      731 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/extends_mtime_sindfa.json
+-rw-rw-rw-   0        0        0      221 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/phanterpwa_modules_mtime.json
+-rw-rw-rw-   0        0        0        0 2022-04-26 23:56:37.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/readme.txt
+-rw-rw-rw-   0        0        0    11082 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/statics_mtime_admin.json
+-rw-rw-rw-   0        0        0     8222 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/statics_mtime_components.json
+-rw-rw-rw-   0        0        0     8119 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/statics_mtime_scaffold_app.json
+-rw-rw-rw-   0        0        0     6140 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/statics_mtime_sindfa.json
+-rw-rw-rw-   0        0        0     1369 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/styles_mtime_admin.json
+-rw-rw-rw-   0        0        0      592 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/styles_mtime_components.json
+-rw-rw-rw-   0        0        0     1075 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/styles_mtime_scaffold_app.json
+-rw-rw-rw-   0        0        0     3682 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/styles_mtime_sindfa.json
+-rw-rw-rw-   0        0        0      681 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/templates_mtime_admin.json
+-rw-rw-rw-   0        0        0      338 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/templates_mtime_components.json
+-rw-rw-rw-   0        0        0      474 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/templates_mtime_scaffold_app.json
+-rw-rw-rw-   0        0        0      190 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/templates_mtime_sindfa.json
+-rw-rw-rw-   0        0        0     2676 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_admin.json
+-rw-rw-rw-   0        0        0      810 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_components.json
+-rw-rw-rw-   0        0        0     1342 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_scaffold_app.json
+-rw-rw-rw-   0        0        0     1127 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_sindfa.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.261405 phanterpwa-13.13.8/phanterpwa/interface/Admin/trash/
+-rw-rw-rw-   0        0        0       20 2022-04-26 23:53:12.000000 phanterpwa-13.13.8/phanterpwa/interface/Admin/trash/readme.txt
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/__init__.py
+-rw-rw-rw-   0        0        0     7015 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/admin_tk.py
+-rw-rw-rw-   0        0        0    50861 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.274405 phanterpwa-13.13.8/phanterpwa/interface/grafics/
+-rw-rw-rw-   0        0        0    15086 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/grafics/icon.ico
+-rw-rw-rw-   0        0        0      634 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/grafics/on.jpg
+-rw-rw-rw-   0        0        0   140200 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/graphic.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.286433 phanterpwa-13.13.8/phanterpwa/interface/langs/
+-rw-rw-rw-   0        0        0     5309 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/langs/English.json
+-rw-rw-rw-   0        0        0     5339 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/langs/Portuguese.json
+-rw-rw-rw-   0        0        0     2800 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/interface/langs/entries.json
+-rw-rw-rw-   0        0        0     5741 2021-09-05 00:25:27.000000 phanterpwa-13.13.8/phanterpwa/mail.py
+-rw-rw-rw-   0        0        0    10764 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/reversexml.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.325405 phanterpwa-13.13.8/phanterpwa/samples/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/samples/__init__.py
+-rw-rw-rw-   0        0        0      372 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/samples/about_cli
+-rw-rw-rw-   0        0        0      269 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/samples/about_graphic
+-rw-rw-rw-   0        0        0      533 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/samples/art
+-rw-rw-rw-   0        0        0      408 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/samples/art_cli
+-rw-rw-rw-   0        0        0     2183 2022-07-06 20:15:09.000000 phanterpwa-13.13.8/phanterpwa/samples/config.json
+-rw-rw-rw-   0        0        0     4996 2022-11-26 15:08:21.000000 phanterpwa-13.13.8/phanterpwa/samples/email.sass
+-rw-rw-rw-   0        0        0     6072 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/samples/email_activation_code.py
+-rw-rw-rw-   0        0        0     5840 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/samples/email_password.py
+-rw-rw-rw-   0        0        0     9137 2021-09-05 04:01:49.000000 phanterpwa-13.13.8/phanterpwa/samples/email_two_factor_code.py
+-rw-rw-rw-   0        0        0     1879 2022-07-06 20:14:49.000000 phanterpwa-13.13.8/phanterpwa/samples/project_config_sample.py
+-rw-rw-rw-   0        0        0      236 2021-09-05 03:59:44.000000 phanterpwa-13.13.8/phanterpwa/samples/sms_activation_code.py
+-rw-rw-rw-   0        0        0      245 2021-09-04 16:15:07.000000 phanterpwa-13.13.8/phanterpwa/samples/sms_password.py
+-rw-rw-rw-   0        0        0      241 2021-09-04 16:33:02.000000 phanterpwa-13.13.8/phanterpwa/samples/sms_two_factor_code.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.394404 phanterpwa-13.13.8/phanterpwa/scaffolds/
+-rw-rw-rw-   0        0        0  2214300 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/scaffolds/Scaffold_PhanterPWA_TM.ppwa
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/scaffolds/__init__.py
+-rw-rw-rw-   0        0        0    12247 2022-09-23 00:15:14.000000 phanterpwa-13.13.8/phanterpwa/server.py
+-rw-rw-rw-   0        0        0     1313 2021-09-05 16:25:04.000000 phanterpwa-13.13.8/phanterpwa/sms.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.188434 phanterpwa-13.13.8/phanterpwa/tests/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.417405 phanterpwa-13.13.8/phanterpwa/tests/helpers_out/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/helpers_out/__init__.py
+-rw-rw-rw-   0        0        0      331 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/helpers_out/my_sass.sass
+-rw-rw-rw-   0        0        0      352 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/helpers_out/new_sass.sass
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.436404 phanterpwa-13.13.8/phanterpwa/tests/path_of_languages/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/path_of_languages/__init__.py
+-rw-rw-rw-   0        0        0      456 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/path_of_languages/entries.json
+-rw-rw-rw-   0        0        0      854 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/path_of_languages/es.json
+-rw-rw-rw-   0        0        0      852 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/path_of_languages/fr.json
+-rw-rw-rw-   0        0        0      860 2021-09-06 05:54:07.000000 phanterpwa-13.13.8/phanterpwa/tests/path_of_languages/pt-BR.json
+-rw-rw-rw-   0        0        0      851 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/path_of_languages/pt-PT.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.460404 phanterpwa-13.13.8/phanterpwa/tests/preloaders/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/preloaders/__init__.py
+-rw-rw-rw-   0        0        0     9764 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_android.html
+-rw-rw-rw-   0        0        0     3489 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_discs.html
+-rw-rw-rw-   0        0        0     5956 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_explosion.html
+-rw-rw-rw-   0        0        0     4451 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_run_points.html
+-rw-rw-rw-   0        0        0     1752 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_square.html
+-rw-rw-rw-   0        0        0     4231 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_squares.html
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.474407 phanterpwa-13.13.8/phanterpwa/tests/static/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/static/__init__.py
+-rw-rw-rw-   0        0        0    97163 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/static/jquery.min.js
+-rw-rw-rw-   0        0        0   143947 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/static/jquery.min.map
+-rw-rw-rw-   0        0        0     2117 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.205431 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.478407 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/not_project/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/not_project/__init__.py
+-rw-rw-rw-   0        0        0       40 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/not_project/config.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.482405 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/project-invalid-name/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/project-invalid-name/__init__.py
+-rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/project-invalid-name/config.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.486403 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/project01/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/project01/__init__.py
+-rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/project01/config.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.491405 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/project02/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/project02/__init__.py
+-rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/project02/config.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.223403 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/without_configjson/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_cli_projects/without_configjson/__init__.py
+-rw-rw-rw-   0        0        0     4079 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_components_preloaders.py
+-rw-rw-rw-   0        0        0    12208 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.227431 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.495403 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/fake_project/
+-rw-rw-rw-   0        0        0       40 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/fake_project/config.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.498404 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project-invalid-name/
+-rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project-invalid-name/config.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.511405 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.560433 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/backapps/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.519403 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/backapps/api/
+-rw-rw-rw-   0        0        0      629 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/backapps/api/app.ini
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.561425 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/backend/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.529404 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/backend/api/
+-rw-rw-rw-   0        0        0      629 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/backend/api/app.ini
+-rw-rw-rw-   0        0        0     2618 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/config.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.565409 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/frontapps/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.538407 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/frontapps/app01/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/frontapps/app01/app.ini
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.547403 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/frontapps/app02/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/frontapps/app02/app.ini
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.568427 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/frontend/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.555405 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/frontend/app01/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/frontend/app01/app.ini
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.564405 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/frontend/app02/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/frontend/app02/app.ini
+-rw-rw-rw-   0        0        0      189 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/project.ini
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.568404 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project02/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project02/__init__.py
+-rw-rw-rw-   0        0        0       44 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project02/config.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.581404 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.571443 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.591405 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/
+-rw-rw-rw-   0        0        0      843 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/app.ini
+-rw-rw-rw-   0        0        0     2143 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/config.json
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.574432 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.599433 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app01/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app01/app.ini
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.608405 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app02/
+-rw-rw-rw-   0        0        0      142 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/frontend/app02/app.ini
+-rw-rw-rw-   0        0        0      149 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/project.ini
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.623403 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_ini/
+-rw-rw-rw-   0        0        0      262 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_ini/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.576429 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_ini/backend/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.631431 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/
+-rw-rw-rw-   0        0        0      843 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/app.ini
+-rw-rw-rw-   0        0        0     2640 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_ini/config.json
+-rw-rw-rw-   0        0        0      149 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_ini/project.ini
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.642432 phanterpwa-13.13.8/phanterpwa/tests/test_folder/
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_folder/cfg.json
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_folder/cfgij.json
+-rw-rw-rw-   0        0        0       23 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_folder/config.json
+-rw-rw-rw-   0        0        0    80202 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.659431 phanterpwa-13.13.8/phanterpwa/tests/test_helpers_languages/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_helpers_languages/__init__.py
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_helpers_languages/en-US.json
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_helpers_languages/entries.json
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_helpers_languages/glingon.json
+-rw-rw-rw-   0        0        0        2 2021-09-06 05:54:07.000000 phanterpwa-13.13.8/phanterpwa/tests/test_helpers_languages/pt-BR.json
+-rw-rw-rw-   0        0        0     3729 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_i18n.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.677405 phanterpwa-13.13.8/phanterpwa/tests/test_i18n_languages/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_i18n_languages/__init__.py
+-rw-rw-rw-   0        0        0       65 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_i18n_languages/en-US.json
+-rw-rw-rw-   0        0        0       36 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_i18n_languages/entries.json
+-rw-rw-rw-   0        0        0       63 2021-09-06 05:54:07.000000 phanterpwa-13.13.8/phanterpwa/tests/test_i18n_languages/pt-BR.json
+-rw-rw-rw-   0        0        0       63 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_i18n_languages/pt-PT.json
+-rw-rw-rw-   0        0        0     4212 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_reversexml.py
+-rw-rw-rw-   0        0        0    11521 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.684404 phanterpwa-13.13.8/phanterpwa/tests/test_tools_humanize_seconds/
+-rw-rw-rw-   0        0        0        2 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/test_tools_humanize_seconds/entries.json
+-rw-rw-rw-   0        0        0        2 2021-09-06 05:54:07.000000 phanterpwa-13.13.8/phanterpwa/tests/test_tools_humanize_seconds/pt-BR.json
+-rw-rw-rw-   0        0        0     1386 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:17.255431 phanterpwa-13.13.8/phanterpwa/third_parties/
+-rw-rw-rw-   0        0        0        0 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/third_parties/__init__.py
+-rw-rw-rw-   0        0        0     5857 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/third_parties/xss.py
+-rw-rw-rw-   0        0        0    45683 2022-04-27 18:34:47.000000 phanterpwa-13.13.8/phanterpwa/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.692404 phanterpwa-13.13.8/phanterpwa/trash/
+-rw-rw-rw-   0        0        0       20 2022-04-26 23:53:12.000000 phanterpwa-13.13.8/phanterpwa/trash/readme.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.699431 phanterpwa-13.13.8/phanterpwa/usual_sass/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.802451 phanterpwa-13.13.8/phanterpwa/usual_sass/components/
+-rw-rw-rw-   0        0        0     1794 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/alert_top_activation.sass
+-rw-rw-rw-   0        0        0     1551 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/breascrumbs.sass
+-rw-rw-rw-   0        0        0     2741 2021-07-27 18:35:01.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/buttons.sass
+-rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/capcha_preload.sass
+-rw-rw-rw-   0        0        0     7323 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/captcha.sass
+-rw-rw-rw-   0        0        0     5213 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/captcha_preload_image_3x4.sass
+-rw-rw-rw-   0        0        0      643 2022-11-25 21:37:56.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/card.sass
+-rw-rw-rw-   0        0        0    13548 2022-04-04 10:57:28.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/cmp_auth_user.sass
+-rw-rw-rw-   0        0        0     6615 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/datetimepicker.sass
+-rw-rw-rw-   0        0        0     1741 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/developer.sass
+-rw-rw-rw-   0        0        0     3154 2022-06-07 17:05:55.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/easy.sass
+-rw-rw-rw-   0        0        0     1067 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/flash.sass
+-rw-rw-rw-   0        0        0     2937 2022-04-27 17:07:49.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/forms.sass
+-rw-rw-rw-   0        0        0     1888 2022-05-17 18:44:18.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/messages.sass
+-rw-rw-rw-   0        0        0     3190 2022-04-04 10:57:28.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/modal.sass
+-rw-rw-rw-   0        0        0     1694 2021-09-05 18:33:48.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/modal_login.sass
+-rw-rw-rw-   0        0        0      649 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/phanterpwa_gallery.sass
+-rw-rw-rw-   0        0        0     4103 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/phanterpwa_gallery_cutter.sass
+-rw-rw-rw-   0        0        0     1450 2021-08-13 03:26:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/phanterpwa_panel_control.sass
+-rw-rw-rw-   0        0        0     2959 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/progressbar.sass
+-rw-rw-rw-   0        0        0      660 2022-02-03 09:45:15.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/pseudomodal.sass
+-rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/run_points.sass
+-rw-rw-rw-   0        0        0     1536 2021-06-17 02:27:21.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/sections.sass
+-rw-rw-rw-   0        0        0      811 2021-05-25 20:28:47.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/snippet.sass
+-rw-rw-rw-   0        0        0    79319 2023-01-26 13:45:09.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/widgets.sass
+-rw-rw-rw-   0        0        0     4968 2021-06-15 20:39:00.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/components/xtable.sass
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.810405 phanterpwa-13.13.8/phanterpwa/usual_sass/display/
+-rw-rw-rw-   0        0        0    42388 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/display/grid.sass
+-rw-rw-rw-   0        0        0     3962 2021-12-14 21:24:18.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/display/media_print.sass
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.814429 phanterpwa-13.13.8/phanterpwa/usual_sass/events/
+-rw-rw-rw-   0        0        0      238 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/events/waves.sass
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.824442 phanterpwa-13.13.8/phanterpwa/usual_sass/extends/
+-rw-rw-rw-   0        0        0     8191 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/extends/capcha_preload.sass
+-rw-rw-rw-   0        0        0      393 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/extends/logo.sass
+-rw-rw-rw-   0        0        0     3491 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/extends/run_points.sass
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.831432 phanterpwa-13.13.8/phanterpwa/usual_sass/gates/
+-rw-rw-rw-   0        0        0      865 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/gates/componentes.sass
+-rw-rw-rw-   0        0        0      631 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/gates/main.sass
+-rw-rw-rw-   0        0        0     9456 2023-01-22 22:50:53.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/phanterpwa.sass
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.835436 phanterpwa-13.13.8/phanterpwa/usual_sass/plugins/
+-rw-rw-rw-   0        0        0      153 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/plugins/codemirror.sass
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:18.861433 phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/
+-rw-rw-rw-   0        0        0     7879 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/android.sass
+-rw-rw-rw-   0        0        0     3448 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/discs.sass
+-rw-rw-rw-   0        0        0     5013 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/explosion.sass
+-rw-rw-rw-   0        0        0      954 2022-08-19 19:22:51.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/indefined_text.sass
+-rw-rw-rw-   0        0        0     3367 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/run_points.sass
+-rw-rw-rw-   0        0        0     1348 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/square.sass
+-rw-rw-rw-   0        0        0     3862 2021-05-19 23:34:10.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/squares.sass
+-rw-rw-rw-   0        0        0     8645 2022-04-27 17:07:49.000000 phanterpwa-13.13.8/phanterpwa/usual_sass/variables.sass
+-rw-rw-rw-   0        0        0   162695 2023-02-02 15:14:57.000000 phanterpwa-13.13.8/phanterpwa/xmlconstructor.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:54:16.673403 phanterpwa-13.13.8/phanterpwa.egg-info/
+-rw-rw-rw-   0        0        0     1712 2023-06-14 01:54:14.000000 phanterpwa-13.13.8/phanterpwa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    25133 2023-06-14 01:54:16.000000 phanterpwa-13.13.8/phanterpwa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-06-14 01:54:14.000000 phanterpwa-13.13.8/phanterpwa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-14 01:54:15.000000 phanterpwa-13.13.8/phanterpwa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 01:54:14.000000 phanterpwa-13.13.8/phanterpwa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      122 2023-06-14 01:54:15.000000 phanterpwa-13.13.8/phanterpwa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     5319 2023-06-14 01:54:15.000000 phanterpwa-13.13.8/phanterpwa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 01:54:18.866434 phanterpwa-13.13.8/setup.cfg
+-rw-rw-rw-   0        0        0     4419 2022-07-15 11:22:48.000000 phanterpwa-13.13.8/setup.py
```

### Comparing `phanterpwa-13.13.7/LICENSE` & `phanterpwa-13.13.8/LICENSE`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/MANIFEST.in` & `phanterpwa-13.13.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/PKG-INFO` & `phanterpwa-13.13.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phanterpwa
-Version: 13.13.7
+Version: 13.13.8
 Summary: Tools for the phanterpwadeveloper framework
 Home-page: https://github.com/PhanterJR/phanterpwa
 Author: PhanterJR
 Author-email: phanterjr@conexaodidata.com.br
 Maintainer: PhanterJR
 Maintainer-email: phanterjr@conexaodidata.com.br
 License: MIT
```

### Comparing `phanterpwa-13.13.7/phanterpwa/__main__.py` & `phanterpwa-13.13.8/phanterpwa/__main__.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/dataforms.py` & `phanterpwa-13.13.8/phanterpwa/backend/dataforms.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/decorators.py` & `phanterpwa-13.13.8/phanterpwa/backend/decorators.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/pydal/auth.py` & `phanterpwa-13.13.8/phanterpwa/backend/pydal/auth.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/pydal/cas.py` & `phanterpwa-13.13.8/phanterpwa/backend/pydal/cas.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/pydal/credentials.py` & `phanterpwa-13.13.8/phanterpwa/backend/pydal/credentials.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/pydal/extra_validations.py` & `phanterpwa-13.13.8/phanterpwa/backend/pydal/extra_validations.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/pydal/gallery.py` & `phanterpwa-13.13.8/phanterpwa/backend/pydal/gallery.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/pydal/internal_messages.py` & `phanterpwa-13.13.8/phanterpwa/backend/pydal/internal_messages.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/request_handlers/admin.py` & `phanterpwa-13.13.8/phanterpwa/backend/request_handlers/admin.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/request_handlers/auth.py` & `phanterpwa-13.13.8/phanterpwa/backend/request_handlers/auth.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/request_handlers/cas.py` & `phanterpwa-13.13.8/phanterpwa/backend/request_handlers/cas.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/request_handlers/credentials.py` & `phanterpwa-13.13.8/phanterpwa/backend/request_handlers/credentials.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/request_handlers/errors.py` & `phanterpwa-13.13.8/phanterpwa/backend/request_handlers/errors.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/request_handlers/i18n_server.py` & `phanterpwa-13.13.8/phanterpwa/backend/request_handlers/i18n_server.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/request_handlers/internal_messages.py` & `phanterpwa-13.13.8/phanterpwa/backend/request_handlers/internal_messages.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/request_handlers/oauth.py` & `phanterpwa-13.13.8/phanterpwa/backend/request_handlers/oauth.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/request_handlers/websocket.py` & `phanterpwa-13.13.8/phanterpwa/backend/request_handlers/websocket.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/request_handlers/welcome.py` & `phanterpwa-13.13.8/phanterpwa/backend/request_handlers/welcome.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/backend/security.py` & `phanterpwa-13.13.8/phanterpwa/backend/security.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/captcha.py` & `phanterpwa-13.13.8/phanterpwa/captchasvg/captcha.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/captchadata.json` & `phanterpwa-13.13.8/phanterpwa/captchasvg/captchadata.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/sass/captcha.sass` & `phanterpwa-13.13.8/phanterpwa/captchasvg/sass/captcha.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/animal/butterfly.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/animal/butterfly.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/animal/crab.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/animal/crab.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/animal/pig.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/animal/pig.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/animal/rabbit.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/animal/rabbit.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/animal/rooster.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/animal/rooster.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/letter/a.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/letter/a.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/letter/b.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/letter/b.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/letter/c.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/letter/c.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/letter/d.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/letter/d.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/mean_of_transport/airplane.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/mean_of_transport/airplane.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/mean_of_transport/car.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/mean_of_transport/car.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/mean_of_transport/motorcycle.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/mean_of_transport/motorcycle.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/mean_of_transport/ship.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/mean_of_transport/ship.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/number/four.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/number/four.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/number/one.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/number/one.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/number/three.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/number/three.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/captchasvg/vectors/number/two.recs` & `phanterpwa-13.13.8/phanterpwa/captchasvg/vectors/number/two.recs`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/compiler.py` & `phanterpwa-13.13.8/phanterpwa/compiler.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/inputs.py` & `phanterpwa-13.13.8/phanterpwa/components/inputs.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/left_bar.py` & `phanterpwa-13.13.8/phanterpwa/components/left_bar.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/materialize.py` & `phanterpwa-13.13.8/phanterpwa/components/materialize.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/phanterpwagallery.py` & `phanterpwa-13.13.8/phanterpwa/components/phanterpwagallery.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/android.py` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/android.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/android.sass` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/android.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/discs.py` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/discs.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/discs.sass` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/discs.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/explosion.py` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/explosion.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/explosion.sass` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/explosion.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/run_points.py` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/run_points.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/run_points.sass` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/run_points.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/square.py` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/square.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/square.sass` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/square.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/squares.py` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/squares.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/components/preloaders/squares.sass` & `phanterpwa-13.13.8/phanterpwa/components/preloaders/squares.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/configer.py` & `phanterpwa-13.13.8/phanterpwa/configer.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/application.py` & `phanterpwa-13.13.8/phanterpwa/frontend/application.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/components/admin.py` & `phanterpwa-13.13.8/phanterpwa/frontend/components/admin.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/components/auth_user.py` & `phanterpwa-13.13.8/phanterpwa/frontend/components/auth_user.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/components/datetimepicker.py` & `phanterpwa-13.13.8/phanterpwa/frontend/components/datetimepicker.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/components/events.py` & `phanterpwa-13.13.8/phanterpwa/frontend/components/events.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/components/gallery.py` & `phanterpwa-13.13.8/phanterpwa/frontend/components/gallery.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/components/left_bar.py` & `phanterpwa-13.13.8/phanterpwa/frontend/components/left_bar.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/components/modal.py` & `phanterpwa-13.13.8/phanterpwa/frontend/components/modal.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/components/pagination.py` & `phanterpwa-13.13.8/phanterpwa/frontend/components/pagination.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/components/snippets.py` & `phanterpwa-13.13.8/phanterpwa/frontend/components/snippets.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/components/top_slide.py` & `phanterpwa-13.13.8/phanterpwa/frontend/components/top_slide.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/components/widgets.py` & `phanterpwa-13.13.8/phanterpwa/frontend/components/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -3024,14 +3024,16 @@
             }),
             HR(_class="material-widgets-animation-offfocus"),
             label,
             **wrapper_attr
         )
         Widget.__init__(self, identifier, html, **parameters)
 
+    def value(self):
+        return self._value
 
 class CheckBox(Widget):
     def __init__(self, identifier, **parameters):
         self._label = parameters.get("label", None)
         self._name = parameters.get("name", None)
         self._value = parameters.get("value", False)
         self._can_empty = parameters.get("can_empty", False)
```

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/decorators.py` & `phanterpwa-13.13.8/phanterpwa/frontend/decorators.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/fmasks.py` & `phanterpwa-13.13.8/phanterpwa/frontend/fmasks.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/forms.py` & `phanterpwa-13.13.8/phanterpwa/frontend/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,15 @@
                     form=self.table_name,
                 )
             elif self._widget_type == "hidden":
                 w = widgets.Inert(
                     "{0}-{1}".format(self.table_name, self.input_name),
                     label=self.json_widget['label'],
                     name=self.input_name,
-                    value=dvalue,
+                    value=self._value,
                     wear="shadows",
                     _class="data_view",
                     kind="hidden",
                     form=self.table_name,
                 )
 
             elif self._widget_type == "image":
```

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/gallery.py` & `phanterpwa-13.13.8/phanterpwa/frontend/gallery.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/gatehandler.py` & `phanterpwa-13.13.8/phanterpwa/frontend/gatehandler.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/helpers.py` & `phanterpwa-13.13.8/phanterpwa/frontend/helpers.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/i18n.py` & `phanterpwa-13.13.8/phanterpwa/frontend/i18n.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/initializer.py` & `phanterpwa-13.13.8/phanterpwa/frontend/initializer.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/plugins/client.py` & `phanterpwa-13.13.8/phanterpwa/frontend/plugins/client.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/preloaders.py` & `phanterpwa-13.13.8/phanterpwa/frontend/preloaders.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/progressbar.py` & `phanterpwa-13.13.8/phanterpwa/frontend/progressbar.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/selects.py` & `phanterpwa-13.13.8/phanterpwa/frontend/selects.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/server.py` & `phanterpwa-13.13.8/phanterpwa/frontend/server.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/validations.py` & `phanterpwa-13.13.8/phanterpwa/frontend/validations.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/frontend/websocket.py` & `phanterpwa-13.13.8/phanterpwa/frontend/websocket.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/gallery/cutter.py` & `phanterpwa-13.13.8/phanterpwa/gallery/cutter.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/gallery/integrationDAL.py` & `phanterpwa-13.13.8/phanterpwa/gallery/integrationDAL.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/helpers.py` & `phanterpwa-13.13.8/phanterpwa/helpers.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/i18n/__init__.py` & `phanterpwa-13.13.8/phanterpwa/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/LICENSE` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/LICENSE`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/controllers/developer.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/controllers/developer.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_activity.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_activity.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_membership.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_membership.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user_phanterpwagallery.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_auth_user_phanterpwagallery.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_captcha.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_captcha.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_client.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_client.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_csrf.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_csrf.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_email_user_list.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_email_user_list.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_google_captcha.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_google_captcha.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_phanterpwagallery.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_phanterpwagallery.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_social_auth.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_social_auth.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_two_factor_login.table` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/c8b669d15150d7109e5f7ab36744a5b7_two_factor_login.table`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/sql.log` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/sql.log`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/databases/storage.sqlite` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/databases/storage.sqlite`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/handlers.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/handlers.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/admin/entries.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/admin/entries.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/admin/pt-BR.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/admin/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/captcha/pt-BR.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/captcha/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/email/entries.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/email/entries.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/email/pt-BR.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/email/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/entries.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/entries.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/languages/pt-BR.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/languages/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/models/__init__.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/statics/images/user.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/statics/images/user.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/backapps/api/statics/images/warning.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/backapps/api/statics/images/warning.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/core.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/core.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/handlers.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/handlers.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/languages/entries.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/languages/entries.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/languages/pt-BR.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/languages/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/application.sass` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/application.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/capcha_preload.sass` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/capcha_preload.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/phanterpwa-logo.sass` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/phanterpwa-logo.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/run_points.sass` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/extends/run_points.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/components.sass` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/components.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/main.sass` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/styles/gates/main.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/button_preloader.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/button_preloader.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/captcha_preload.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/captcha_preload.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/css_head.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/css_head.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/favicons.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/favicons.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/fontawesome.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/fontawesome.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/javascript_head.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/javascript_head.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/logo.svg` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/extends/logo.svg`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/index.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/index.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/fontawesome.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/fontawesome.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/phanterpwa_logo.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/phanterpwa_logo.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/svg_logo.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/templates/loads/svg_logo.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/application.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/application.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/config.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/auto/config.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/cmps.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/cmps.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/developer.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/developer.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/errors.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/errors.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/examples.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/examples.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/inputs.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/inputs.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/menus.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/menus.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/selects.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/ext_examples/selects.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/fontawesome.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/fontawesome.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/home.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/home.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/project.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/project.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/reqs.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/reqs.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/testsp.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/gatehandlers/testsp.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/codemirror.py` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/sources/transcrypts/plugins/codemirror.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/css/all.min.css` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/all.min.css`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/css/normalize.css` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/normalize.css`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/css/phanterpwa.css` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/css/phanterpwa.css`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-144x144.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-144x144.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-192x192.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-256x256.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-256x256.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-512x512.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/apple-touch-icon.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-16x16.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-32x32.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon.ico` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/mstile-150x150.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/favicons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.eot` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.svg` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.svg`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.ttf` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff2` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/88bdc70ec292cc29451932f9875b378a.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhFq3-OXg.woff2` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhFq3-OXg.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhLq38.woff2` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/L0x5DF4xlVMF-BfR8bXMIjhLq38.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.eot` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.ttf` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff2` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/Roboto-Thin.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SQvzA.woff2` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SQvzA.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SovzAbt.woff2` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/d6lIkaiiRdih4SpP_SovzAbt.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNc.woff2` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNc.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.eot` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.svg` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.ttf` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff2` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/fonts/roboto-v20-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/images/background.jpg` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/background.jpg`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/images/user.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/user.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/images/warning.png` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/images/warning.png`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js.map` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/hammer.min.js.map`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.hammer.js` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.hammer.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.js` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.map` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/jquery.min.map`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/js/touch-emulator.js` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/js/touch-emulator.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.webmanifest` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/json/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.css` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.css`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.js` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/lib/codemirror.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/index.html` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/index.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/python.js` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/python.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/test.js` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/mode/python/test.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.eot` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.ttf` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff2` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.eot` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.ttf` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff2` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.eot` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.ttf` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff2` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/frontapps/admin/statics/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/_compiler_sass_temp_file.sass` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/_compiler_sass_temp_file.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/extends_mtime_admin.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/extends_mtime_admin.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/extends_mtime_components.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/extends_mtime_components.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/extends_mtime_scaffold_app.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/extends_mtime_scaffold_app.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/extends_mtime_sindfa.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/extends_mtime_sindfa.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/statics_mtime_admin.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/statics_mtime_admin.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/statics_mtime_components.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/statics_mtime_components.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/statics_mtime_scaffold_app.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/statics_mtime_scaffold_app.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/statics_mtime_sindfa.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/statics_mtime_sindfa.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/styles_mtime_admin.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/styles_mtime_admin.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/styles_mtime_components.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/styles_mtime_components.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/styles_mtime_scaffold_app.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/styles_mtime_scaffold_app.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/styles_mtime_sindfa.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/styles_mtime_sindfa.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/templates_mtime_admin.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/templates_mtime_admin.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/transcrypts_mtime_admin.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_admin.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/transcrypts_mtime_components.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_components.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/transcrypts_mtime_scaffold_app.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_scaffold_app.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/Admin/temp/transcrypts_mtime_sindfa.json` & `phanterpwa-13.13.8/phanterpwa/interface/Admin/temp/transcrypts_mtime_sindfa.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/admin_tk.py` & `phanterpwa-13.13.8/phanterpwa/interface/admin_tk.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/cli.py` & `phanterpwa-13.13.8/phanterpwa/interface/cli.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/grafics/icon.ico` & `phanterpwa-13.13.8/phanterpwa/interface/grafics/icon.ico`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/grafics/on.jpg` & `phanterpwa-13.13.8/phanterpwa/interface/grafics/on.jpg`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/graphic.py` & `phanterpwa-13.13.8/phanterpwa/interface/graphic.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/langs/English.json` & `phanterpwa-13.13.8/phanterpwa/interface/langs/English.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/langs/Portuguese.json` & `phanterpwa-13.13.8/phanterpwa/interface/langs/Portuguese.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/interface/langs/entries.json` & `phanterpwa-13.13.8/phanterpwa/interface/langs/entries.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/mail.py` & `phanterpwa-13.13.8/phanterpwa/mail.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/reversexml.py` & `phanterpwa-13.13.8/phanterpwa/reversexml.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/samples/art` & `phanterpwa-13.13.8/phanterpwa/samples/art`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/samples/config.json` & `phanterpwa-13.13.8/phanterpwa/samples/config.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/samples/email.sass` & `phanterpwa-13.13.8/phanterpwa/samples/email.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/samples/email_activation_code.py` & `phanterpwa-13.13.8/phanterpwa/samples/email_activation_code.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/samples/email_password.py` & `phanterpwa-13.13.8/phanterpwa/samples/email_password.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/samples/email_two_factor_code.py` & `phanterpwa-13.13.8/phanterpwa/samples/email_two_factor_code.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/samples/project_config_sample.py` & `phanterpwa-13.13.8/phanterpwa/samples/project_config_sample.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/scaffolds/Scaffold_PhanterPWA_TM.ppwa` & `phanterpwa-13.13.8/phanterpwa/scaffolds/Scaffold_PhanterPWA_TM.ppwa`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/server.py` & `phanterpwa-13.13.8/phanterpwa/server.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/sms.py` & `phanterpwa-13.13.8/phanterpwa/sms.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/path_of_languages/es.json` & `phanterpwa-13.13.8/phanterpwa/tests/path_of_languages/es.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/path_of_languages/fr.json` & `phanterpwa-13.13.8/phanterpwa/tests/path_of_languages/fr.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/path_of_languages/pt-BR.json` & `phanterpwa-13.13.8/phanterpwa/tests/path_of_languages/pt-BR.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/path_of_languages/pt-PT.json` & `phanterpwa-13.13.8/phanterpwa/tests/path_of_languages/pt-PT.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_android.html` & `phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_android.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_discs.html` & `phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_discs.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_explosion.html` & `phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_explosion.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_run_points.html` & `phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_run_points.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_square.html` & `phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_square.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/preloaders/test_components_preloaders_squares.html` & `phanterpwa-13.13.8/phanterpwa/tests/preloaders/test_components_preloaders_squares.html`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/static/jquery.min.js` & `phanterpwa-13.13.8/phanterpwa/tests/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/static/jquery.min.map` & `phanterpwa-13.13.8/phanterpwa/tests/static/jquery.min.map`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_cli.py` & `phanterpwa-13.13.8/phanterpwa/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_components_preloaders.py` & `phanterpwa-13.13.8/phanterpwa/tests/test_components_preloaders.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_configer.py` & `phanterpwa-13.13.8/phanterpwa/tests/test_configer.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/backapps/api/app.ini` & `phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/backapps/api/app.ini`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/backend/api/app.ini` & `phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/backend/api/app.ini`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project01/config.json` & `phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project01/config.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/app.ini` & `phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/backend/api/app.ini`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/config.json` & `phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_confgjson_and_with_ini/config.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/app.ini` & `phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_ini/backend/api/app.ini`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_configer_path/project_without_ini/config.json` & `phanterpwa-13.13.8/phanterpwa/tests/test_configer_path/project_without_ini/config.json`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_helpers.py` & `phanterpwa-13.13.8/phanterpwa/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_i18n.py` & `phanterpwa-13.13.8/phanterpwa/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_reversexml.py` & `phanterpwa-13.13.8/phanterpwa/tests/test_reversexml.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/test_tools.py` & `phanterpwa-13.13.8/phanterpwa/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tests/tests.py` & `phanterpwa-13.13.8/phanterpwa/tests/tests.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/third_parties/xss.py` & `phanterpwa-13.13.8/phanterpwa/third_parties/xss.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/tools.py` & `phanterpwa-13.13.8/phanterpwa/tools.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/alert_top_activation.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/alert_top_activation.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/breascrumbs.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/breascrumbs.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/buttons.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/buttons.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/capcha_preload.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/capcha_preload.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/captcha.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/captcha.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/captcha_preload_image_3x4.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/captcha_preload_image_3x4.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/card.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/card.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/cmp_auth_user.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/cmp_auth_user.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/datetimepicker.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/datetimepicker.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/developer.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/developer.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/easy.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/easy.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/flash.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/flash.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/forms.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/forms.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/messages.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/messages.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/modal.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/modal.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/modal_login.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/modal_login.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/phanterpwa_gallery.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/phanterpwa_gallery.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/phanterpwa_gallery_cutter.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/phanterpwa_gallery_cutter.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/phanterpwa_panel_control.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/phanterpwa_panel_control.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/progressbar.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/progressbar.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/pseudomodal.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/pseudomodal.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/run_points.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/run_points.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/sections.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/sections.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/snippet.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/snippet.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/widgets.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/widgets.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/components/xtable.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/components/xtable.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/display/grid.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/display/grid.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/display/media_print.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/display/media_print.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/extends/capcha_preload.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/extends/capcha_preload.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/extends/run_points.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/extends/run_points.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/gates/componentes.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/gates/componentes.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/gates/main.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/gates/main.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/phanterpwa.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/phanterpwa.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/android.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/android.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/discs.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/discs.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/explosion.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/explosion.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/indefined_text.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/indefined_text.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/run_points.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/run_points.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/square.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/square.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/preloaders/squares.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/preloaders/squares.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/usual_sass/variables.sass` & `phanterpwa-13.13.8/phanterpwa/usual_sass/variables.sass`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa/xmlconstructor.py` & `phanterpwa-13.13.8/phanterpwa/xmlconstructor.py`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa.egg-info/PKG-INFO` & `phanterpwa-13.13.8/phanterpwa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phanterpwa
-Version: 13.13.7
+Version: 13.13.8
 Summary: Tools for the phanterpwadeveloper framework
 Home-page: https://github.com/PhanterJR/phanterpwa
 Author: PhanterJR
 Author-email: phanterjr@conexaodidata.com.br
 Maintainer: PhanterJR
 Maintainer-email: phanterjr@conexaodidata.com.br
 License: MIT
```

### Comparing `phanterpwa-13.13.7/phanterpwa.egg-info/SOURCES.txt` & `phanterpwa-13.13.8/phanterpwa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/phanterpwa.egg-info/top_level.txt` & `phanterpwa-13.13.8/phanterpwa.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `phanterpwa-13.13.7/setup.py` & `phanterpwa-13.13.8/setup.py`

 * *Files identical despite different names*

