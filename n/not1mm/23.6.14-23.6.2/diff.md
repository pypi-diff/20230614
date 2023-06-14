# Comparing `tmp/not1mm-23.6.14.tar.gz` & `tmp/not1mm-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.6.14.tar", last modified: Wed Jun 14 19:29:47 2023, max compression
+gzip compressed data, was "not1mm-23.6.2.tar", last modified: Fri Jun  2 14:44:35 2023, max compression
```

## Comparing `not1mm-23.6.14.tar` & `not1mm-23.6.2.tar`

### file list

```diff
@@ -1,144 +1,142 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-14 19:29:47.107348 not1mm-23.6.14/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.6.14/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30223 2023-06-14 19:29:47.107348 not1mm-23.6.14/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29476 2023-06-14 19:27:02.000000 not1mm-23.6.14/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-14 19:29:46.956351 not1mm-23.6.14/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.14/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    90337 2023-06-14 19:21:21.000000 not1mm-23.6.14/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    25525 2023-06-01 00:41:28.000000 not1mm-23.6.14/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-14 19:29:47.000350 not1mm-23.6.14/not1mm/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.6.14/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.6.14/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2023-05-18 23:48:17.000000 not1mm-23.6.14/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.6.14/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.6.14/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.6.14/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    41522 2023-05-23 20:03:51.000000 not1mm-23.6.14/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.6.14/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4635080 2023-06-02 13:47:30.000000 not1mm-23.6.14/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-06-02 13:43:39.000000 not1mm-23.6.14/not1mm/data/cty_old.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.6.14/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       78 2023-05-19 04:25:57.000000 not1mm-23.6.14/not1mm/data/donors.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.6.14/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.6.14/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.6.14/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.6.14/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.6.14/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.6.14/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.6.14/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.6.14/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44315 2023-06-12 21:04:40.000000 not1mm-23.6.14/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      865 2023-06-06 18:28:20.000000 not1mm-23.6.14/not1mm/data/map.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.6.14/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.6.14/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-14 19:29:47.091348 not1mm-23.6.14/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.6.14/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.6.14/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.6.14/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.6.14/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.6.14/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.6.14/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.6.14/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.6.14/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.6.14/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.6.14/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.6.14/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.6.14/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.6.14/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.6.14/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.6.14/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.6.14/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.6.14/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.6.14/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.6.14/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.6.14/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.6.14/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.6.14/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.6.14/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.6.14/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.6.14/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.6.14/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.6.14/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.6.14/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.6.14/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.6.14/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.6.14/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.6.14/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.6.14/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.6.14/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.6.14/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.6.14/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.6.14/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.6.14/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.6.14/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.6.14/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.6.14/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.6.14/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.6.14/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.6.14/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.6.14/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.6.14/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.6.14/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.6.14/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.6.14/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.6.14/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.6.14/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.6.14/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-14 19:29:47.101348 not1mm-23.6.14/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.14/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.6.14/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15676 2023-05-22 20:40:03.000000 not1mm-23.6.14/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3123 2023-05-11 20:24:55.000000 not1mm-23.6.14/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34356 2023-05-24 20:24:28.000000 not1mm-23.6.14/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.6.14/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.6.14/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.6.14/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.6.14/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.6.14/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.6.14/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1761 2023-05-12 16:20:09.000000 not1mm-23.6.14/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5713 2023-05-24 14:24:14.000000 not1mm-23.6.14/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.6.14/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.6.14/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6885 2023-05-23 19:07:39.000000 not1mm-23.6.14/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-06-14 19:28:27.000000 not1mm-23.6.14/not1mm/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2023-05-19 19:40:38.000000 not1mm-23.6.14/not1mm/lib/versiontest.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    33732 2023-05-30 16:14:11.000000 not1mm-23.6.14/not1mm/logwindow.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-06-06 19:25:20.000000 not1mm-23.6.14/not1mm/map.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-14 19:29:47.105348 not1mm-23.6.14/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13883 2023-05-29 18:30:11.000000 not1mm-23.6.14/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13888 2023-05-29 18:30:48.000000 not1mm-23.6.14/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-29 18:31:29.000000 not1mm-23.6.14/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13898 2023-05-29 18:31:57.000000 not1mm-23.6.14/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.6.14/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14684 2023-05-29 18:32:51.000000 not1mm-23.6.14/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14687 2023-05-29 18:33:05.000000 not1mm-23.6.14/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13125 2023-05-29 18:33:21.000000 not1mm-23.6.14/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.6.14/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16077 2023-05-29 18:33:47.000000 not1mm-23.6.14/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16082 2023-05-29 18:34:01.000000 not1mm-23.6.14/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15301 2023-05-29 18:25:56.000000 not1mm-23.6.14/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15323 2023-05-29 18:34:21.000000 not1mm-23.6.14/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14031 2023-05-29 18:34:36.000000 not1mm-23.6.14/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14035 2023-05-29 18:34:53.000000 not1mm-23.6.14/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14890 2023-05-29 18:35:16.000000 not1mm-23.6.14/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.6.14/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.6.14/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.6.14/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.6.14/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-14 19:29:47.106348 not1mm-23.6.14/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2083 2023-05-19 23:10:32.000000 not1mm-23.6.14/not1mm/testing/fakeflrig.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1658 2023-05-19 17:23:54.000000 not1mm-23.6.14/not1mm/testing/flrigclient.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1099 2023-05-24 18:38:16.000000 not1mm-23.6.14/not1mm/testing/n1mm_listener.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1660 2023-05-14 06:26:14.000000 not1mm-23.6.14/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-14 19:29:46.957351 not1mm-23.6.14/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30223 2023-06-14 19:29:46.000000 not1mm-23.6.14/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3615 2023-06-14 19:29:46.000000 not1mm-23.6.14/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-14 19:29:46.000000 not1mm-23.6.14/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-06-14 19:29:46.000000 not1mm-23.6.14/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       83 2023-06-14 19:29:46.000000 not1mm-23.6.14/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-06-14 19:29:46.000000 not1mm-23.6.14/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1262 2023-06-14 19:28:36.000000 not1mm-23.6.14/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-14 19:29:47.107348 not1mm-23.6.14/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-14 19:29:47.107348 not1mm-23.6.14/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      176 2023-05-31 20:52:45.000000 not1mm-23.6.14/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.521264 not1mm-23.6.2/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.6.2/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29969 2023-06-02 14:44:35.521264 not1mm-23.6.2/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29223 2023-06-02 14:30:06.000000 not1mm-23.6.2/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.467265 not1mm-23.6.2/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.2/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89811 2023-06-02 13:41:52.000000 not1mm-23.6.2/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    25525 2023-06-01 00:41:28.000000 not1mm-23.6.2/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.486265 not1mm-23.6.2/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.6.2/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.6.2/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2023-05-18 23:48:17.000000 not1mm-23.6.2/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.6.2/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.6.2/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.6.2/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    41522 2023-05-23 20:03:51.000000 not1mm-23.6.2/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.6.2/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4635080 2023-06-02 13:47:30.000000 not1mm-23.6.2/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-06-02 13:43:39.000000 not1mm-23.6.2/not1mm/data/cty_old.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.6.2/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       78 2023-05-19 04:25:57.000000 not1mm-23.6.2/not1mm/data/donors.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.6.2/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.6.2/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.6.2/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.6.2/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.6.2/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.6.2/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.6.2/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.6.2/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44138 2023-05-31 18:11:05.000000 not1mm-23.6.2/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.6.2/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.6.2/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.513264 not1mm-23.6.2/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.6.2/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.6.2/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.6.2/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.6.2/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.6.2/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.6.2/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.6.2/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.6.2/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.6.2/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.6.2/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.6.2/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.6.2/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.6.2/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.6.2/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.6.2/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.6.2/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.6.2/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.6.2/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.6.2/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.6.2/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.6.2/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.6.2/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.6.2/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.6.2/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.6.2/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.6.2/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.6.2/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.6.2/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.6.2/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.6.2/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.6.2/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.6.2/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.6.2/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.6.2/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.6.2/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.6.2/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.6.2/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.6.2/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.6.2/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.6.2/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.6.2/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.6.2/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.6.2/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.6.2/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.6.2/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.6.2/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.6.2/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.6.2/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.6.2/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.6.2/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.6.2/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.6.2/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.516264 not1mm-23.6.2/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.2/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.6.2/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15676 2023-05-22 20:40:03.000000 not1mm-23.6.2/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3123 2023-05-11 20:24:55.000000 not1mm-23.6.2/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34356 2023-05-24 20:24:28.000000 not1mm-23.6.2/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.6.2/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.6.2/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.6.2/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.6.2/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.6.2/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.6.2/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1761 2023-05-12 16:20:09.000000 not1mm-23.6.2/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5713 2023-05-24 14:24:14.000000 not1mm-23.6.2/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.6.2/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.6.2/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6885 2023-05-23 19:07:39.000000 not1mm-23.6.2/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-06-02 14:26:27.000000 not1mm-23.6.2/not1mm/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2023-05-19 19:40:38.000000 not1mm-23.6.2/not1mm/lib/versiontest.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    33732 2023-05-30 16:14:11.000000 not1mm-23.6.2/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.519264 not1mm-23.6.2/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13883 2023-05-29 18:30:11.000000 not1mm-23.6.2/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13888 2023-05-29 18:30:48.000000 not1mm-23.6.2/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-29 18:31:29.000000 not1mm-23.6.2/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13898 2023-05-29 18:31:57.000000 not1mm-23.6.2/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.6.2/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14684 2023-05-29 18:32:51.000000 not1mm-23.6.2/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14687 2023-05-29 18:33:05.000000 not1mm-23.6.2/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13125 2023-05-29 18:33:21.000000 not1mm-23.6.2/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.6.2/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16077 2023-05-29 18:33:47.000000 not1mm-23.6.2/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16082 2023-05-29 18:34:01.000000 not1mm-23.6.2/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15301 2023-05-29 18:25:56.000000 not1mm-23.6.2/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15323 2023-05-29 18:34:21.000000 not1mm-23.6.2/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14031 2023-05-29 18:34:36.000000 not1mm-23.6.2/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14035 2023-05-29 18:34:53.000000 not1mm-23.6.2/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14890 2023-05-29 18:35:16.000000 not1mm-23.6.2/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.6.2/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.6.2/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.6.2/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.6.2/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.519264 not1mm-23.6.2/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2083 2023-05-19 23:10:32.000000 not1mm-23.6.2/not1mm/testing/fakeflrig.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1658 2023-05-19 17:23:54.000000 not1mm-23.6.2/not1mm/testing/flrigclient.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1099 2023-05-24 18:38:16.000000 not1mm-23.6.2/not1mm/testing/n1mm_listener.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1660 2023-05-14 06:26:14.000000 not1mm-23.6.2/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.468265 not1mm-23.6.2/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29969 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3582 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       83 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-06-02 14:44:35.000000 not1mm-23.6.2/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1261 2023-06-02 14:26:13.000000 not1mm-23.6.2/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-02 14:44:35.522264 not1mm-23.6.2/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:44:35.520264 not1mm-23.6.2/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      176 2023-05-31 20:52:45.000000 not1mm-23.6.2/testing/test.py
```

### Comparing `not1mm-23.6.14/LICENSE` & `not1mm-23.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/PKG-INFO` & `not1mm-23.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.6.14
+Version: 23.6.2
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,15 +15,14 @@
 Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Not1MM
 
-[![PyPI](https://img.shields.io/pypi/v/not1mm)](https://pypi.org/project/not1mm/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Python: 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
 [![Made With:PyQt5](https://img.shields.io/badge/Made%20with-PyQt5-red)](https://pypi.org/project/PyQt5/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/not1mm)](https://pypi.org/project/not1mm/)
 
 ![logo](https://github.com/mbridak/not1mm/raw/master/not1mm/data/k6gte.not1mm.svg)
 
@@ -137,16 +136,14 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-6-14] Added check to see if your Russ and want to operate a contest thats not defined.
-- [23-6-12] Add `File->Quit` because Russ can't click an 'x' to quit program.
 - [23-6-2] Added an automated check and update of the cty.dat file. Added dependency to `notctyparser`
 
 <details>
 
 <summary>May 2023</summary>
 
 - [23-5-31] updated cty.json ( I need to automate this )
```

### Comparing `not1mm-23.6.14/README.md` & `not1mm-23.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Not1MM
 
-[![PyPI](https://img.shields.io/pypi/v/not1mm)](https://pypi.org/project/not1mm/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Python: 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
 [![Made With:PyQt5](https://img.shields.io/badge/Made%20with-PyQt5-red)](https://pypi.org/project/PyQt5/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/not1mm)](https://pypi.org/project/not1mm/)
 
 ![logo](https://github.com/mbridak/not1mm/raw/master/not1mm/data/k6gte.not1mm.svg)
 
@@ -118,16 +117,14 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-6-14] Added check to see if your Russ and want to operate a contest thats not defined.
-- [23-6-12] Add `File->Quit` because Russ can't click an 'x' to quit program.
 - [23-6-2] Added an automated check and update of the cty.dat file. Added dependency to `notctyparser`
 
 <details>
 
 <summary>May 2023</summary>
 
 - [23-5-31] updated cty.json ( I need to automate this )
```

### Comparing `not1mm-23.6.14/not1mm/__main__.py` & `not1mm-23.6.2/not1mm/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,5214 +434,5181 @@
 00001b10: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
 00001b20: 656c 662e 6564 6974 5f63 775f 6d61 6372  elf.edit_cw_macr
 00001b30: 6f73 290a 0a20 2020 2020 2020 2073 656c  os)..        sel
 00001b40: 662e 6163 7469 6f6e 4162 6f75 742e 7472  f.actionAbout.tr
 00001b50: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
 00001b60: 7365 6c66 2e73 686f 775f 6162 6f75 745f  self.show_about_
 00001b70: 6469 616c 6f67 290a 0a20 2020 2020 2020  dialog)..       
-00001b80: 2073 656c 662e 6163 7469 6f6e 5175 6974   self.actionQuit
-00001b90: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
-00001ba0: 6374 2873 656c 662e 7175 6974 5f61 7070  ct(self.quit_app
-00001bb0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00001bc0: 7261 6469 6f42 7574 746f 6e5f 7275 6e2e  radioButton_run.
-00001bd0: 636c 6963 6b65 642e 636f 6e6e 6563 7428  clicked.connect(
-00001be0: 7365 6c66 2e72 756e 5f73 705f 6275 7474  self.run_sp_butt
-00001bf0: 6f6e 735f 636c 6963 6b65 6429 0a20 2020  ons_clicked).   
-00001c00: 2020 2020 2073 656c 662e 7261 6469 6f42       self.radioB
-00001c10: 7574 746f 6e5f 7370 2e63 6c69 636b 6564  utton_sp.clicked
-00001c20: 2e63 6f6e 6e65 6374 2873 656c 662e 7275  .connect(self.ru
-00001c30: 6e5f 7370 5f62 7574 746f 6e73 5f63 6c69  n_sp_buttons_cli
-00001c40: 636b 6564 290a 2020 2020 2020 2020 7365  cked).        se
-00001c50: 6c66 2e73 636f 7265 2e73 6574 5465 7874  lf.score.setText
-00001c60: 2822 3022 290a 2020 2020 2020 2020 7365  ("0").        se
-00001c70: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
-00001c80: 4564 6974 6564 2e63 6f6e 6e65 6374 2873  Edited.connect(s
-00001c90: 656c 662e 6361 6c6c 7369 676e 5f63 6861  elf.callsign_cha
-00001ca0: 6e67 6564 290a 2020 2020 2020 2020 7365  nged).        se
-00001cb0: 6c66 2e63 616c 6c73 6967 6e2e 7265 7475  lf.callsign.retu
-00001cc0: 726e 5072 6573 7365 642e 636f 6e6e 6563  rnPressed.connec
-00001cd0: 7428 7365 6c66 2e73 6176 655f 636f 6e74  t(self.save_cont
-00001ce0: 6163 7429 0a20 2020 2020 2020 2073 656c  act).        sel
-00001cf0: 662e 7365 6e74 2e72 6574 7572 6e50 7265  f.sent.returnPre
-00001d00: 7373 6564 2e63 6f6e 6e65 6374 2873 656c  ssed.connect(sel
-00001d10: 662e 7361 7665 5f63 6f6e 7461 6374 290a  f.save_contact).
-00001d20: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
-00001d30: 6569 7665 2e72 6574 7572 6e50 7265 7373  eive.returnPress
-00001d40: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00001d50: 7361 7665 5f63 6f6e 7461 6374 290a 2020  save_contact).  
-00001d60: 2020 2020 2020 7365 6c66 2e6f 7468 6572        self.other
-00001d70: 5f31 2e72 6574 7572 6e50 7265 7373 6564  _1.returnPressed
-00001d80: 2e63 6f6e 6e65 6374 2873 656c 662e 7361  .connect(self.sa
-00001d90: 7665 5f63 6f6e 7461 6374 290a 2020 2020  ve_contact).    
-00001da0: 2020 2020 7365 6c66 2e6f 7468 6572 5f32      self.other_2
-00001db0: 2e72 6574 7572 6e50 7265 7373 6564 2e63  .returnPressed.c
-00001dc0: 6f6e 6e65 6374 2873 656c 662e 7361 7665  onnect(self.save
-00001dd0: 5f63 6f6e 7461 6374 290a 2020 2020 2020  _contact).      
-00001de0: 2020 7365 6c66 2e6f 7468 6572 5f32 2e74    self.other_2.t
-00001df0: 6578 7445 6469 7465 642e 636f 6e6e 6563  extEdited.connec
-00001e00: 7428 7365 6c66 2e6f 7468 6572 5f32 5f63  t(self.other_2_c
-00001e10: 6861 6e67 6564 290a 0a20 2020 2020 2020  hanged)..       
-00001e20: 2073 656c 662e 7365 6e74 2e73 6574 5465   self.sent.setTe
-00001e30: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
-00001e40: 2073 656c 662e 7265 6365 6976 652e 7365   self.receive.se
-00001e50: 7454 6578 7428 2235 3922 290a 2020 2020  tText("59").    
-00001e60: 2020 2020 6963 6f6e 5f70 6174 6820 3d20      icon_path = 
-00001e70: 574f 524b 494e 475f 5041 5448 202b 2022  WORKING_PATH + "
-00001e80: 2f64 6174 612f 220a 2020 2020 2020 2020  /data/".        
-00001e90: 7365 6c66 2e67 7265 656e 646f 7420 3d20  self.greendot = 
-00001ea0: 5174 4775 692e 5150 6978 6d61 7028 6963  QtGui.QPixmap(ic
-00001eb0: 6f6e 5f70 6174 6820 2b20 2267 7265 656e  on_path + "green
-00001ec0: 646f 742e 706e 6722 290a 2020 2020 2020  dot.png").      
-00001ed0: 2020 7365 6c66 2e72 6564 646f 7420 3d20    self.reddot = 
-00001ee0: 5174 4775 692e 5150 6978 6d61 7028 6963  QtGui.QPixmap(ic
-00001ef0: 6f6e 5f70 6174 6820 2b20 2272 6564 646f  on_path + "reddo
-00001f00: 742e 706e 6722 290a 2020 2020 2020 2020  t.png").        
-00001f10: 7365 6c66 2e6c 6566 7464 6f74 2e73 6574  self.leftdot.set
-00001f20: 5069 786d 6170 2873 656c 662e 6772 6565  Pixmap(self.gree
-00001f30: 6e64 6f74 290a 2020 2020 2020 2020 7365  ndot).        se
-00001f40: 6c66 2e72 6967 6874 646f 742e 7365 7450  lf.rightdot.setP
-00001f50: 6978 6d61 7028 7365 6c66 2e72 6564 646f  ixmap(self.reddo
-00001f60: 7429 0a0a 2020 2020 2020 2020 7365 6c66  t)..        self
-00001f70: 2e46 312e 7365 7443 6f6e 7465 7874 4d65  .F1.setContextMe
-00001f80: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
-00001f90: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
-00001fa0: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
-00001fb0: 6c66 2e46 312e 6375 7374 6f6d 436f 6e74  lf.F1.customCont
-00001fc0: 6578 744d 656e 7552 6571 7565 7374 6564  extMenuRequested
-00001fd0: 2e63 6f6e 6e65 6374 2873 656c 662e 6564  .connect(self.ed
-00001fe0: 6974 5f46 3129 0a20 2020 2020 2020 2073  it_F1).        s
-00001ff0: 656c 662e 4631 2e63 6c69 636b 6564 2e63  elf.F1.clicked.c
-00002000: 6f6e 6e65 6374 2873 656c 662e 7365 6e64  onnect(self.send
-00002010: 6631 290a 2020 2020 2020 2020 7365 6c66  f1).        self
-00002020: 2e46 322e 7365 7443 6f6e 7465 7874 4d65  .F2.setContextMe
-00002030: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
-00002040: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
-00002050: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
-00002060: 6c66 2e46 322e 6375 7374 6f6d 436f 6e74  lf.F2.customCont
-00002070: 6578 744d 656e 7552 6571 7565 7374 6564  extMenuRequested
-00002080: 2e63 6f6e 6e65 6374 2873 656c 662e 6564  .connect(self.ed
-00002090: 6974 5f46 3229 0a20 2020 2020 2020 2073  it_F2).        s
-000020a0: 656c 662e 4632 2e63 6c69 636b 6564 2e63  elf.F2.clicked.c
-000020b0: 6f6e 6e65 6374 2873 656c 662e 7365 6e64  onnect(self.send
-000020c0: 6632 290a 2020 2020 2020 2020 7365 6c66  f2).        self
-000020d0: 2e46 332e 7365 7443 6f6e 7465 7874 4d65  .F3.setContextMe
-000020e0: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
-000020f0: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
-00002100: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
-00002110: 6c66 2e46 332e 6375 7374 6f6d 436f 6e74  lf.F3.customCont
-00002120: 6578 744d 656e 7552 6571 7565 7374 6564  extMenuRequested
-00002130: 2e63 6f6e 6e65 6374 2873 656c 662e 6564  .connect(self.ed
-00002140: 6974 5f46 3329 0a20 2020 2020 2020 2073  it_F3).        s
-00002150: 656c 662e 4633 2e63 6c69 636b 6564 2e63  elf.F3.clicked.c
-00002160: 6f6e 6e65 6374 2873 656c 662e 7365 6e64  onnect(self.send
-00002170: 6633 290a 2020 2020 2020 2020 7365 6c66  f3).        self
-00002180: 2e46 342e 7365 7443 6f6e 7465 7874 4d65  .F4.setContextMe
-00002190: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
-000021a0: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
-000021b0: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
-000021c0: 6c66 2e46 342e 6375 7374 6f6d 436f 6e74  lf.F4.customCont
-000021d0: 6578 744d 656e 7552 6571 7565 7374 6564  extMenuRequested
-000021e0: 2e63 6f6e 6e65 6374 2873 656c 662e 6564  .connect(self.ed
-000021f0: 6974 5f46 3429 0a20 2020 2020 2020 2073  it_F4).        s
-00002200: 656c 662e 4634 2e63 6c69 636b 6564 2e63  elf.F4.clicked.c
-00002210: 6f6e 6e65 6374 2873 656c 662e 7365 6e64  onnect(self.send
-00002220: 6634 290a 2020 2020 2020 2020 7365 6c66  f4).        self
-00002230: 2e46 352e 7365 7443 6f6e 7465 7874 4d65  .F5.setContextMe
-00002240: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
-00002250: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
-00002260: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
-00002270: 6c66 2e46 352e 6375 7374 6f6d 436f 6e74  lf.F5.customCont
-00002280: 6578 744d 656e 7552 6571 7565 7374 6564  extMenuRequested
-00002290: 2e63 6f6e 6e65 6374 2873 656c 662e 6564  .connect(self.ed
-000022a0: 6974 5f46 3529 0a20 2020 2020 2020 2073  it_F5).        s
-000022b0: 656c 662e 4635 2e63 6c69 636b 6564 2e63  elf.F5.clicked.c
-000022c0: 6f6e 6e65 6374 2873 656c 662e 7365 6e64  onnect(self.send
-000022d0: 6635 290a 2020 2020 2020 2020 7365 6c66  f5).        self
-000022e0: 2e46 362e 7365 7443 6f6e 7465 7874 4d65  .F6.setContextMe
-000022f0: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
-00002300: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
-00002310: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
-00002320: 6c66 2e46 362e 6375 7374 6f6d 436f 6e74  lf.F6.customCont
-00002330: 6578 744d 656e 7552 6571 7565 7374 6564  extMenuRequested
-00002340: 2e63 6f6e 6e65 6374 2873 656c 662e 6564  .connect(self.ed
-00002350: 6974 5f46 3629 0a20 2020 2020 2020 2073  it_F6).        s
-00002360: 656c 662e 4636 2e63 6c69 636b 6564 2e63  elf.F6.clicked.c
-00002370: 6f6e 6e65 6374 2873 656c 662e 7365 6e64  onnect(self.send
-00002380: 6636 290a 2020 2020 2020 2020 7365 6c66  f6).        self
-00002390: 2e46 372e 7365 7443 6f6e 7465 7874 4d65  .F7.setContextMe
-000023a0: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
-000023b0: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
-000023c0: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
-000023d0: 6c66 2e46 372e 6375 7374 6f6d 436f 6e74  lf.F7.customCont
-000023e0: 6578 744d 656e 7552 6571 7565 7374 6564  extMenuRequested
-000023f0: 2e63 6f6e 6e65 6374 2873 656c 662e 6564  .connect(self.ed
-00002400: 6974 5f46 3729 0a20 2020 2020 2020 2073  it_F7).        s
-00002410: 656c 662e 4637 2e63 6c69 636b 6564 2e63  elf.F7.clicked.c
-00002420: 6f6e 6e65 6374 2873 656c 662e 7365 6e64  onnect(self.send
-00002430: 6637 290a 2020 2020 2020 2020 7365 6c66  f7).        self
-00002440: 2e46 382e 7365 7443 6f6e 7465 7874 4d65  .F8.setContextMe
-00002450: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
-00002460: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
-00002470: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
-00002480: 6c66 2e46 382e 6375 7374 6f6d 436f 6e74  lf.F8.customCont
-00002490: 6578 744d 656e 7552 6571 7565 7374 6564  extMenuRequested
-000024a0: 2e63 6f6e 6e65 6374 2873 656c 662e 6564  .connect(self.ed
-000024b0: 6974 5f46 3829 0a20 2020 2020 2020 2073  it_F8).        s
-000024c0: 656c 662e 4638 2e63 6c69 636b 6564 2e63  elf.F8.clicked.c
-000024d0: 6f6e 6e65 6374 2873 656c 662e 7365 6e64  onnect(self.send
-000024e0: 6638 290a 2020 2020 2020 2020 7365 6c66  f8).        self
-000024f0: 2e46 392e 7365 7443 6f6e 7465 7874 4d65  .F9.setContextMe
-00002500: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
-00002510: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
-00002520: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
-00002530: 6c66 2e46 392e 6375 7374 6f6d 436f 6e74  lf.F9.customCont
-00002540: 6578 744d 656e 7552 6571 7565 7374 6564  extMenuRequested
-00002550: 2e63 6f6e 6e65 6374 2873 656c 662e 6564  .connect(self.ed
-00002560: 6974 5f46 3929 0a20 2020 2020 2020 2073  it_F9).        s
-00002570: 656c 662e 4639 2e63 6c69 636b 6564 2e63  elf.F9.clicked.c
-00002580: 6f6e 6e65 6374 2873 656c 662e 7365 6e64  onnect(self.send
-00002590: 6639 290a 2020 2020 2020 2020 7365 6c66  f9).        self
-000025a0: 2e46 3130 2e73 6574 436f 6e74 6578 744d  .F10.setContextM
-000025b0: 656e 7550 6f6c 6963 7928 5174 436f 7265  enuPolicy(QtCore
-000025c0: 2e51 742e 4375 7374 6f6d 436f 6e74 6578  .Qt.CustomContex
-000025d0: 744d 656e 7529 0a20 2020 2020 2020 2073  tMenu).        s
-000025e0: 656c 662e 4631 302e 6375 7374 6f6d 436f  elf.F10.customCo
-000025f0: 6e74 6578 744d 656e 7552 6571 7565 7374  ntextMenuRequest
-00002600: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00002610: 6564 6974 5f46 3130 290a 2020 2020 2020  edit_F10).      
-00002620: 2020 7365 6c66 2e46 3130 2e63 6c69 636b    self.F10.click
-00002630: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00002640: 7365 6e64 6631 3029 0a20 2020 2020 2020  sendf10).       
-00002650: 2073 656c 662e 4631 312e 7365 7443 6f6e   self.F11.setCon
-00002660: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-00002670: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-00002680: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-00002690: 2020 2020 7365 6c66 2e46 3131 2e63 7573      self.F11.cus
-000026a0: 746f 6d43 6f6e 7465 7874 4d65 6e75 5265  tomContextMenuRe
-000026b0: 7175 6573 7465 642e 636f 6e6e 6563 7428  quested.connect(
-000026c0: 7365 6c66 2e65 6469 745f 4631 3129 0a20  self.edit_F11). 
-000026d0: 2020 2020 2020 2073 656c 662e 4631 312e         self.F11.
-000026e0: 636c 6963 6b65 642e 636f 6e6e 6563 7428  clicked.connect(
-000026f0: 7365 6c66 2e73 656e 6466 3131 290a 2020  self.sendf11).  
-00002700: 2020 2020 2020 7365 6c66 2e46 3132 2e73        self.F12.s
-00002710: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-00002720: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-00002730: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-00002740: 0a20 2020 2020 2020 2073 656c 662e 4631  .        self.F1
-00002750: 322e 6375 7374 6f6d 436f 6e74 6578 744d  2.customContextM
-00002760: 656e 7552 6571 7565 7374 6564 2e63 6f6e  enuRequested.con
-00002770: 6e65 6374 2873 656c 662e 6564 6974 5f46  nect(self.edit_F
-00002780: 3132 290a 2020 2020 2020 2020 7365 6c66  12).        self
-00002790: 2e46 3132 2e63 6c69 636b 6564 2e63 6f6e  .F12.clicked.con
-000027a0: 6e65 6374 2873 656c 662e 7365 6e64 6631  nect(self.sendf1
-000027b0: 3229 0a0a 2020 2020 2020 2020 7365 6c66  2)..        self
-000027c0: 2e72 6561 6470 7265 6665 7265 6e63 6573  .readpreferences
-000027d0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-000027e0: 6462 6e61 6d65 203d 2044 4154 415f 5041  dbname = DATA_PA
-000027f0: 5448 202b 2022 2f22 202b 2073 656c 662e  TH + "/" + self.
-00002800: 7072 6566 2e67 6574 2822 6375 7272 656e  pref.get("curren
-00002810: 745f 6461 7461 6261 7365 222c 2022 6861  t_database", "ha
-00002820: 6d2e 6462 2229 0a20 2020 2020 2020 2073  m.db").        s
-00002830: 656c 662e 6461 7461 6261 7365 203d 2044  elf.database = D
-00002840: 6174 6142 6173 6528 7365 6c66 2e64 626e  ataBase(self.dbn
-00002850: 616d 652c 2057 4f52 4b49 4e47 5f50 4154  ame, WORKING_PAT
-00002860: 4829 0a20 2020 2020 2020 2073 656c 662e  H).        self.
-00002870: 7374 6174 696f 6e20 3d20 7365 6c66 2e64  station = self.d
-00002880: 6174 6162 6173 652e 6665 7463 685f 7374  atabase.fetch_st
-00002890: 6174 696f 6e28 290a 2020 2020 2020 2020  ation().        
-000028a0: 6966 2073 656c 662e 7374 6174 696f 6e20  if self.station 
-000028b0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000028c0: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-000028d0: 6e20 3d20 7b7d 0a20 2020 2020 2020 2020  n = {}.         
-000028e0: 2020 2073 656c 662e 6564 6974 5f73 7461     self.edit_sta
-000028f0: 7469 6f6e 5f73 6574 7469 6e67 7328 290a  tion_settings().
-00002900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002910: 2e73 7461 7469 6f6e 203d 2073 656c 662e  .station = self.
-00002920: 6461 7461 6261 7365 2e66 6574 6368 5f73  database.fetch_s
-00002930: 7461 7469 6f6e 2829 0a20 2020 2020 2020  tation().       
-00002940: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00002950: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-00002960: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00002970: 6c66 2e73 7461 7469 6f6e 203d 207b 7d0a  lf.station = {}.
-00002980: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00002990: 7461 6374 203d 2073 656c 662e 6461 7461  tact = self.data
-000029a0: 6261 7365 2e65 6d70 7479 5f63 6f6e 7461  base.empty_conta
-000029b0: 6374 0a20 2020 2020 2020 2073 656c 662e  ct.        self.
-000029c0: 6375 7272 656e 745f 6f70 203d 2073 656c  current_op = sel
-000029d0: 662e 7374 6174 696f 6e2e 6765 7428 2243  f.station.get("C
-000029e0: 616c 6c22 2c20 2222 290a 2020 2020 2020  all", "").      
-000029f0: 2020 7365 6c66 2e6d 616b 655f 6f70 5f64    self.make_op_d
-00002a00: 6972 2829 0a20 2020 2020 2020 2073 656c  ir().        sel
-00002a10: 662e 7265 6164 5f63 775f 6d61 6372 6f73  f.read_cw_macros
-00002a20: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00002a30: 636c 6561 7269 6e70 7574 7328 290a 0a20  clearinputs().. 
-00002a40: 2020 2020 2020 2073 656c 662e 6261 6e64         self.band
-00002a50: 5f69 6e64 6963 6174 6f72 735f 6377 203d  _indicators_cw =
-00002a60: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00002a70: 3136 3022 3a20 7365 6c66 2e63 775f 6261  160": self.cw_ba
-00002a80: 6e64 5f31 3630 2c0a 2020 2020 2020 2020  nd_160,.        
-00002a90: 2020 2020 2238 3022 3a20 7365 6c66 2e63      "80": self.c
-00002aa0: 775f 6261 6e64 5f38 302c 0a20 2020 2020  w_band_80,.     
-00002ab0: 2020 2020 2020 2022 3430 223a 2073 656c         "40": sel
-00002ac0: 662e 6377 5f62 616e 645f 3430 2c0a 2020  f.cw_band_40,.  
-00002ad0: 2020 2020 2020 2020 2020 2232 3022 3a20            "20": 
-00002ae0: 7365 6c66 2e63 775f 6261 6e64 5f32 302c  self.cw_band_20,
-00002af0: 0a20 2020 2020 2020 2020 2020 2022 3135  .            "15
-00002b00: 223a 2073 656c 662e 6377 5f62 616e 645f  ": self.cw_band_
-00002b10: 3135 2c0a 2020 2020 2020 2020 2020 2020  15,.            
-00002b20: 2231 3022 3a20 7365 6c66 2e63 775f 6261  "10": self.cw_ba
-00002b30: 6e64 5f31 302c 0a20 2020 2020 2020 207d  nd_10,.        }
-00002b40: 0a0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
-00002b50: 616e 645f 696e 6469 6361 746f 7273 5f73  and_indicators_s
-00002b60: 7362 203d 207b 0a20 2020 2020 2020 2020  sb = {.         
-00002b70: 2020 2022 3136 3022 3a20 7365 6c66 2e73     "160": self.s
-00002b80: 7362 5f62 616e 645f 3136 302c 0a20 2020  sb_band_160,.   
-00002b90: 2020 2020 2020 2020 2022 3830 223a 2073           "80": s
-00002ba0: 656c 662e 7373 625f 6261 6e64 5f38 302c  elf.ssb_band_80,
-00002bb0: 0a20 2020 2020 2020 2020 2020 2022 3430  .            "40
-00002bc0: 223a 2073 656c 662e 7373 625f 6261 6e64  ": self.ssb_band
-00002bd0: 5f34 302c 0a20 2020 2020 2020 2020 2020  _40,.           
-00002be0: 2022 3230 223a 2073 656c 662e 7373 625f   "20": self.ssb_
-00002bf0: 6261 6e64 5f32 302c 0a20 2020 2020 2020  band_20,.       
-00002c00: 2020 2020 2022 3135 223a 2073 656c 662e       "15": self.
-00002c10: 7373 625f 6261 6e64 5f31 352c 0a20 2020  ssb_band_15,.   
-00002c20: 2020 2020 2020 2020 2022 3130 223a 2073           "10": s
-00002c30: 656c 662e 7373 625f 6261 6e64 5f31 302c  elf.ssb_band_10,
-00002c40: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00002c50: 2020 2020 7365 6c66 2e62 616e 645f 696e      self.band_in
-00002c60: 6469 6361 746f 7273 5f72 7474 7920 3d20  dicators_rtty = 
-00002c70: 7b0a 2020 2020 2020 2020 2020 2020 2231  {.            "1
-00002c80: 3630 223a 2073 656c 662e 7274 7479 5f62  60": self.rtty_b
-00002c90: 616e 645f 3136 302c 0a20 2020 2020 2020  and_160,.       
-00002ca0: 2020 2020 2022 3830 223a 2073 656c 662e       "80": self.
-00002cb0: 7274 7479 5f62 616e 645f 3830 2c0a 2020  rtty_band_80,.  
-00002cc0: 2020 2020 2020 2020 2020 2234 3022 3a20            "40": 
-00002cd0: 7365 6c66 2e72 7474 795f 6261 6e64 5f34  self.rtty_band_4
-00002ce0: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
-00002cf0: 3230 223a 2073 656c 662e 7274 7479 5f62  20": self.rtty_b
-00002d00: 616e 645f 3230 2c0a 2020 2020 2020 2020  and_20,.        
-00002d10: 2020 2020 2231 3522 3a20 7365 6c66 2e72      "15": self.r
-00002d20: 7474 795f 6261 6e64 5f31 352c 0a20 2020  tty_band_15,.   
-00002d30: 2020 2020 2020 2020 2022 3130 223a 2073           "10": s
-00002d40: 656c 662e 7274 7479 5f62 616e 645f 3130  elf.rtty_band_10
-00002d50: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
-00002d60: 2020 2020 2073 656c 662e 616c 6c5f 6d6f       self.all_mo
-00002d70: 6465 5f69 6e64 6963 6174 6f72 7320 3d20  de_indicators = 
-00002d80: 7b0a 2020 2020 2020 2020 2020 2020 2243  {.            "C
-00002d90: 5722 3a20 7365 6c66 2e62 616e 645f 696e  W": self.band_in
-00002da0: 6469 6361 746f 7273 5f63 772c 0a20 2020  dicators_cw,.   
-00002db0: 2020 2020 2020 2020 2022 5353 4222 3a20           "SSB": 
-00002dc0: 7365 6c66 2e62 616e 645f 696e 6469 6361  self.band_indica
-00002dd0: 746f 7273 5f73 7362 2c0a 2020 2020 2020  tors_ssb,.      
-00002de0: 2020 2020 2020 2252 5454 5922 3a20 7365        "RTTY": se
-00002df0: 6c66 2e62 616e 645f 696e 6469 6361 746f  lf.band_indicato
-00002e00: 7273 5f72 7474 792c 0a20 2020 2020 2020  rs_rtty,.       
-00002e10: 207d 0a0a 2020 2020 2020 2020 6966 2073   }..        if s
-00002e20: 656c 662e 7072 6566 2e67 6574 2822 636f  elf.pref.get("co
-00002e30: 6e74 6573 7422 293a 0a20 2020 2020 2020  ntest"):.       
-00002e40: 2020 2020 2073 656c 662e 6c6f 6164 5f63       self.load_c
-00002e50: 6f6e 7465 7374 2829 0a0a 2020 2020 2020  ontest()..      
-00002e60: 2020 6966 2056 6572 7369 6f6e 5465 7374    if VersionTest
-00002e70: 285f 5f76 6572 7369 6f6e 5f5f 292e 7465  (__version__).te
-00002e80: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00002e90: 2020 7365 6c66 2e73 686f 775f 6d65 7373    self.show_mess
-00002ea0: 6167 655f 626f 7828 0a20 2020 2020 2020  age_box(.       
-00002eb0: 2020 2020 2020 2020 2022 5468 6572 6520           "There 
-00002ec0: 6973 2061 206e 6577 6572 2076 6572 7369  is a newer versi
-00002ed0: 6f6e 206f 6620 6e6f 7431 6d6d 2061 7661  on of not1mm ava
-00002ee0: 696c 6162 6c65 2e5c 6e22 0a20 2020 2020  ilable.\n".     
-00002ef0: 2020 2020 2020 2020 2020 2022 596f 7520             "You 
-00002f00: 6361 6e20 7564 6174 6520 746f 2074 6865  can udate to the
-00002f10: 2063 7572 7265 6e74 2076 6572 7369 6f6e   current version
-00002f20: 2062 7920 7573 696e 673a 5c6e 7069 7020   by using:\npip 
-00002f30: 696e 7374 616c 6c20 2d55 206e 6f74 316d  install -U not1m
-00002f40: 6d22 0a20 2020 2020 2020 2020 2020 2029  m".            )
-00002f50: 0a0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-00002f60: 6865 636b 5f66 6f72 5f6e 6577 5f63 7479  heck_for_new_cty
-00002f70: 2829 0a0a 2020 2020 6465 6620 7175 6974  ()..    def quit
-00002f80: 5f61 7070 2873 656c 6629 3a0a 2020 2020  _app(self):.    
-00002f90: 2020 2020 2222 2264 6f63 2222 220a 2020      """doc""".  
-00002fa0: 2020 2020 2020 6170 702e 7175 6974 2829        app.quit()
-00002fb0: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00002fc0: 686f 640a 2020 2020 6465 6620 6368 6563  hod.    def chec
-00002fd0: 6b5f 7072 6f63 6573 7328 6e61 6d65 3a20  k_process(name: 
-00002fe0: 7374 7229 202d 3e20 626f 6f6c 3a0a 2020  str) -> bool:.  
-00002ff0: 2020 2020 2020 2222 2263 6865 636b 7320        """checks 
-00003000: 746f 2073 6565 2069 6620 7072 6f67 7261  to see if progra
-00003010: 6d20 6f66 206e 616d 6520 6973 2069 6e20  m of name is in 
-00003020: 7468 6520 6163 7469 7665 2070 726f 6365  the active proce
-00003030: 7373 206c 6973 7422 2222 0a20 2020 2020  ss list""".     
-00003040: 2020 2066 6f72 2070 726f 6320 696e 2070     for proc in p
-00003050: 7375 7469 6c2e 7072 6f63 6573 735f 6974  sutil.process_it
-00003060: 6572 2829 3a0a 2020 2020 2020 2020 2020  er():.          
-00003070: 2020 6966 2062 6f6f 6c28 7265 2e6d 6174    if bool(re.mat
-00003080: 6368 286e 616d 652c 2070 726f 632e 6e61  ch(name, proc.na
-00003090: 6d65 2829 2e6c 6f77 6572 2829 2929 3a0a  me().lower())):.
-000030a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030b0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-000030c0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000030d0: 0a0a 2020 2020 6465 6620 7368 6f77 5f6d  ..    def show_m
-000030e0: 6573 7361 6765 5f62 6f78 2873 656c 662c  essage_box(self,
-000030f0: 206d 6573 7361 6765 3a20 7374 7229 202d   message: str) -
-00003100: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00003110: 2222 2264 6f63 2222 220a 2020 2020 2020  """doc""".      
-00003120: 2020 6d65 7373 6167 655f 626f 7820 3d20    message_box = 
-00003130: 5174 5769 6467 6574 732e 514d 6573 7361  QtWidgets.QMessa
-00003140: 6765 426f 7828 290a 2020 2020 2020 2020  geBox().        
-00003150: 6d65 7373 6167 655f 626f 782e 7365 7449  message_box.setI
-00003160: 636f 6e28 5174 5769 6467 6574 732e 514d  con(QtWidgets.QM
-00003170: 6573 7361 6765 426f 782e 496e 666f 726d  essageBox.Inform
-00003180: 6174 696f 6e29 0a20 2020 2020 2020 206d  ation).        m
-00003190: 6573 7361 6765 5f62 6f78 2e73 6574 5465  essage_box.setTe
-000031a0: 7874 286d 6573 7361 6765 290a 2020 2020  xt(message).    
-000031b0: 2020 2020 6d65 7373 6167 655f 626f 782e      message_box.
-000031c0: 7365 7457 696e 646f 7754 6974 6c65 2822  setWindowTitle("
-000031d0: 496e 666f 726d 6174 696f 6e22 290a 2020  Information").  
-000031e0: 2020 2020 2020 6d65 7373 6167 655f 626f        message_bo
-000031f0: 782e 7365 7453 7461 6e64 6172 6442 7574  x.setStandardBut
-00003200: 746f 6e73 2851 7457 6964 6765 7473 2e51  tons(QtWidgets.Q
-00003210: 4d65 7373 6167 6542 6f78 2e4f 6b29 0a20  MessageBox.Ok). 
-00003220: 2020 2020 2020 205f 203d 206d 6573 7361         _ = messa
-00003230: 6765 5f62 6f78 2e65 7865 635f 2829 0a0a  ge_box.exec_()..
-00003240: 2020 2020 6465 6620 7368 6f77 5f61 626f      def show_abo
-00003250: 7574 5f64 6961 6c6f 6728 7365 6c66 293a  ut_dialog(self):
-00003260: 0a20 2020 2020 2020 2022 2222 5368 6f77  .        """Show
-00003270: 2061 626f 7574 2064 6961 6c6f 6722 2222   about dialog"""
-00003280: 0a20 2020 2020 2020 2073 656c 662e 6162  .        self.ab
-00003290: 6f75 745f 6469 616c 6f67 203d 2041 626f  out_dialog = Abo
-000032a0: 7574 2857 4f52 4b49 4e47 5f50 4154 4829  ut(WORKING_PATH)
-000032b0: 0a20 2020 2020 2020 2073 656c 662e 6162  .        self.ab
-000032c0: 6f75 745f 6469 616c 6f67 2e64 6f6e 6f72  out_dialog.donor
-000032d0: 732e 7365 7453 6f75 7263 6528 0a20 2020  s.setSource(.   
-000032e0: 2020 2020 2020 2020 2051 7443 6f72 652e           QtCore.
-000032f0: 5155 726c 2e66 726f 6d4c 6f63 616c 4669  QUrl.fromLocalFi
-00003300: 6c65 2857 4f52 4b49 4e47 5f50 4154 4820  le(WORKING_PATH 
-00003310: 2b20 222f 6461 7461 2f64 6f6e 6f72 732e  + "/data/donors.
-00003320: 6874 6d6c 2229 0a20 2020 2020 2020 2029  html").        )
-00003330: 0a20 2020 2020 2020 2073 656c 662e 6162  .        self.ab
-00003340: 6f75 745f 6469 616c 6f67 2e6f 7065 6e28  out_dialog.open(
-00003350: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-00003360: 636f 6e66 6967 7572 6174 696f 6e5f 7365  configuration_se
-00003370: 7474 696e 6773 2873 656c 6629 3a0a 2020  ttings(self):.  
-00003380: 2020 2020 2020 2222 2243 6f6e 6669 6775        """Configu
-00003390: 7261 7469 6f6e 2053 6574 7469 6e67 7320  ration Settings 
-000033a0: 7761 7320 636c 6963 6b65 6422 2222 0a20  was clicked""". 
-000033b0: 2020 2020 2020 2073 656c 662e 636f 6e66         self.conf
-000033c0: 6967 7572 6174 696f 6e5f 6469 616c 6f67  iguration_dialog
-000033d0: 203d 2053 6574 7469 6e67 7328 574f 524b   = Settings(WORK
-000033e0: 494e 475f 5041 5448 2c20 434f 4e46 4947  ING_PATH, CONFIG
-000033f0: 5f50 4154 482c 2073 656c 662e 7072 6566  _PATH, self.pref
-00003400: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00003410: 6f6e 6669 6775 7261 7469 6f6e 5f64 6961  onfiguration_dia
-00003420: 6c6f 672e 7573 6568 616d 6462 5f72 6164  log.usehamdb_rad
-00003430: 696f 4275 7474 6f6e 2e68 6964 6528 290a  ioButton.hide().
-00003440: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00003450: 6669 6775 7261 7469 6f6e 5f64 6961 6c6f  figuration_dialo
-00003460: 672e 7368 6f77 2829 0a20 2020 2020 2020  g.show().       
-00003470: 2073 656c 662e 636f 6e66 6967 7572 6174   self.configurat
-00003480: 696f 6e5f 6469 616c 6f67 2e61 6363 6570  ion_dialog.accep
-00003490: 7465 642e 636f 6e6e 6563 7428 7365 6c66  ted.connect(self
-000034a0: 2e65 6469 745f 636f 6e66 6967 7572 6174  .edit_configurat
-000034b0: 696f 6e5f 7265 7475 726e 290a 0a20 2020  ion_return)..   
-000034c0: 2064 6566 2065 6469 745f 636f 6e66 6967   def edit_config
-000034d0: 7572 6174 696f 6e5f 7265 7475 726e 2873  uration_return(s
-000034e0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-000034f0: 2252 6574 7572 6e73 2068 6572 6520 7768  "Returns here wh
-00003500: 656e 2063 6f6e 6669 6775 7261 7469 6f6e  en configuration
-00003510: 2064 6961 6c6f 6720 636c 6f73 6564 2077   dialog closed w
-00003520: 6974 6820 6f6b 6179 2e22 2222 0a20 2020  ith okay.""".   
-00003530: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
-00003540: 7572 6174 696f 6e5f 6469 616c 6f67 2e73  uration_dialog.s
-00003550: 6176 655f 6368 616e 6765 7328 290a 2020  ave_changes().  
-00003560: 2020 2020 2020 7365 6c66 2e77 7269 7465        self.write
-00003570: 5f70 7265 6665 7265 6e63 6528 290a 2020  _preference().  
-00003580: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00003590: 7567 2822 2573 222c 2066 227b 7365 6c66  ug("%s", f"{self
-000035a0: 2e70 7265 667d 2229 0a20 2020 2020 2020  .pref}").       
-000035b0: 2073 656c 662e 7265 6164 7072 6566 6572   self.readprefer
-000035c0: 656e 6365 7328 290a 0a20 2020 2064 6566  ences()..    def
-000035d0: 206e 6577 5f64 6174 6162 6173 6528 7365   new_database(se
-000035e0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-000035f0: 4372 6561 7465 206e 6577 2064 6174 6162  Create new datab
-00003600: 6173 652e 2222 220a 2020 2020 2020 2020  ase.""".        
-00003610: 6669 6c65 6e61 6d65 203d 2073 656c 662e  filename = self.
-00003620: 6669 6c65 7069 636b 6572 2822 6e65 7722  filepicker("new"
-00003630: 290a 2020 2020 2020 2020 6966 2066 696c  ).        if fil
-00003640: 656e 616d 653a 0a20 2020 2020 2020 2020  ename:.         
-00003650: 2020 2069 6620 6669 6c65 6e61 6d65 5b2d     if filename[-
-00003660: 333a 5d20 213d 2022 2e64 6222 3a0a 2020  3:] != ".db":.  
-00003670: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00003680: 6c65 6e61 6d65 202b 3d20 222e 6462 220a  lename += ".db".
-00003690: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000036a0: 2e70 7265 665b 2263 7572 7265 6e74 5f64  .pref["current_d
-000036b0: 6174 6162 6173 6522 5d20 3d20 6669 6c65  atabase"] = file
-000036c0: 6e61 6d65 2e73 706c 6974 2822 2f22 295b  name.split("/")[
-000036d0: 2d31 3a5d 5b30 5d0a 2020 2020 2020 2020  -1:][0].        
-000036e0: 2020 2020 7365 6c66 2e77 7269 7465 5f70      self.write_p
-000036f0: 7265 6665 7265 6e63 6528 290a 2020 2020  reference().    
-00003700: 2020 2020 2020 2020 7365 6c66 2e64 626e          self.dbn
-00003710: 616d 6520 3d20 4441 5441 5f50 4154 4820  ame = DATA_PATH 
-00003720: 2b20 222f 2220 2b20 7365 6c66 2e70 7265  + "/" + self.pre
-00003730: 662e 6765 7428 2263 7572 7265 6e74 5f64  f.get("current_d
-00003740: 6174 6162 6173 6522 2c20 2268 616d 2e64  atabase", "ham.d
-00003750: 6222 290a 2020 2020 2020 2020 2020 2020  b").            
-00003760: 7365 6c66 2e64 6174 6162 6173 6520 3d20  self.database = 
-00003770: 4461 7461 4261 7365 2873 656c 662e 6462  DataBase(self.db
-00003780: 6e61 6d65 2c20 574f 524b 494e 475f 5041  name, WORKING_PA
-00003790: 5448 290a 2020 2020 2020 2020 2020 2020  TH).            
-000037a0: 7365 6c66 2e63 6f6e 7461 6374 203d 2073  self.contact = s
-000037b0: 656c 662e 6461 7461 6261 7365 2e65 6d70  elf.database.emp
-000037c0: 7479 5f63 6f6e 7461 6374 0a20 2020 2020  ty_contact.     
-000037d0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000037e0: 696f 6e20 3d20 7365 6c66 2e64 6174 6162  ion = self.datab
-000037f0: 6173 652e 6665 7463 685f 7374 6174 696f  ase.fetch_statio
-00003800: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
-00003810: 6966 2073 656c 662e 7374 6174 696f 6e20  if self.station 
-00003820: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00003830: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-00003840: 6174 696f 6e20 3d20 7b7d 0a20 2020 2020  ation = {}.     
-00003850: 2020 2020 2020 2073 656c 662e 6375 7272         self.curr
-00003860: 656e 745f 6f70 203d 2073 656c 662e 7374  ent_op = self.st
-00003870: 6174 696f 6e2e 6765 7428 2243 616c 6c22  ation.get("Call"
-00003880: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-00003890: 2020 7365 6c66 2e6d 616b 655f 6f70 5f64    self.make_op_d
-000038a0: 6972 2829 0a20 2020 2020 2020 2020 2020  ir().           
-000038b0: 2063 6d64 203d 207b 7d0a 2020 2020 2020   cmd = {}.      
-000038c0: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
-000038d0: 203d 2022 4e45 5744 4222 0a20 2020 2020   = "NEWDB".     
-000038e0: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
-000038f0: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
-00003900: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-00003910: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
-00003920: 7374 5f69 6e74 6572 6661 6365 2e73 656e  st_interface.sen
-00003930: 645f 6173 5f6a 736f 6e28 636d 6429 0a20  d_as_json(cmd). 
-00003940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003950: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
-00003960: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-00003970: 6469 745f 7374 6174 696f 6e5f 7365 7474  dit_station_sett
-00003980: 696e 6773 2829 0a0a 2020 2020 6465 6620  ings()..    def 
-00003990: 6f70 656e 5f64 6174 6162 6173 6528 7365  open_database(se
-000039a0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-000039b0: 4f70 656e 2065 7869 7374 696e 6720 6461  Open existing da
-000039c0: 7461 6261 7365 2e22 2222 0a20 2020 2020  tabase.""".     
-000039d0: 2020 2066 696c 656e 616d 6520 3d20 7365     filename = se
-000039e0: 6c66 2e66 696c 6570 6963 6b65 7228 226f  lf.filepicker("o
-000039f0: 7065 6e22 290a 2020 2020 2020 2020 6966  pen").        if
-00003a00: 2066 696c 656e 616d 653a 0a20 2020 2020   filename:.     
-00003a10: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-00003a20: 5b22 6375 7272 656e 745f 6461 7461 6261  ["current_databa
-00003a30: 7365 225d 203d 2066 696c 656e 616d 652e  se"] = filename.
-00003a40: 7370 6c69 7428 222f 2229 5b2d 313a 5d5b  split("/")[-1:][
-00003a50: 305d 0a20 2020 2020 2020 2020 2020 2073  0].            s
-00003a60: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
-00003a70: 656e 6365 2829 0a20 2020 2020 2020 2020  ence().         
-00003a80: 2020 2073 656c 662e 6462 6e61 6d65 203d     self.dbname =
-00003a90: 2044 4154 415f 5041 5448 202b 2022 2f22   DATA_PATH + "/"
-00003aa0: 202b 2073 656c 662e 7072 6566 2e67 6574   + self.pref.get
-00003ab0: 2822 6375 7272 656e 745f 6461 7461 6261  ("current_databa
-00003ac0: 7365 222c 2022 6861 6d2e 6462 2229 0a20  se", "ham.db"). 
-00003ad0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003ae0: 6461 7461 6261 7365 203d 2044 6174 6142  database = DataB
-00003af0: 6173 6528 7365 6c66 2e64 626e 616d 652c  ase(self.dbname,
-00003b00: 2057 4f52 4b49 4e47 5f50 4154 4829 0a20   WORKING_PATH). 
-00003b10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003b20: 636f 6e74 6163 7420 3d20 7365 6c66 2e64  contact = self.d
-00003b30: 6174 6162 6173 652e 656d 7074 795f 636f  atabase.empty_co
-00003b40: 6e74 6163 740a 2020 2020 2020 2020 2020  ntact.          
-00003b50: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
-00003b60: 2073 656c 662e 6461 7461 6261 7365 2e66   self.database.f
-00003b70: 6574 6368 5f73 7461 7469 6f6e 2829 0a20  etch_station(). 
-00003b80: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00003b90: 6c66 2e73 7461 7469 6f6e 2069 7320 4e6f  lf.station is No
-00003ba0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00003bb0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-00003bc0: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
-00003bd0: 2020 6966 2073 656c 662e 7374 6174 696f    if self.statio
-00003be0: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
-00003bf0: 2920 3d3d 2022 223a 0a20 2020 2020 2020  ) == "":.       
-00003c00: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
-00003c10: 6974 5f73 7461 7469 6f6e 5f73 6574 7469  it_station_setti
-00003c20: 6e67 7328 290a 2020 2020 2020 2020 2020  ngs().          
-00003c30: 2020 7365 6c66 2e63 7572 7265 6e74 5f6f    self.current_o
-00003c40: 7020 3d20 7365 6c66 2e73 7461 7469 6f6e  p = self.station
-00003c50: 2e67 6574 2822 4361 6c6c 222c 2022 2229  .get("Call", "")
-00003c60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003c70: 662e 6d61 6b65 5f6f 705f 6469 7228 290a  f.make_op_dir().
-00003c80: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
-00003c90: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
-00003ca0: 2063 6d64 5b22 636d 6422 5d20 3d20 224e   cmd["cmd"] = "N
-00003cb0: 4557 4442 220a 2020 2020 2020 2020 2020  EWDB".          
-00003cc0: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
-00003cd0: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
-00003ce0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00003cf0: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
-00003d00: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
-00003d10: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
-00003d20: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-00003d30: 696e 7075 7473 2829 0a0a 2020 2020 6465  inputs()..    de
-00003d40: 6620 6e65 775f 636f 6e74 6573 7428 7365  f new_contest(se
-00003d50: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00003d60: 4372 6561 7465 206e 6577 2063 6f6e 7465  Create new conte
-00003d70: 7374 2069 6e20 6578 6973 7469 6e67 2064  st in existing d
-00003d80: 6174 6162 6173 652e 2222 220a 0a20 2020  atabase."""..   
-00003d90: 2064 6566 206f 7065 6e5f 636f 6e74 6573   def open_contes
-00003da0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-00003db0: 2022 2222 5377 6974 6368 2074 6f20 6120   """Switch to a 
-00003dc0: 6469 6666 6572 656e 7420 6578 6973 7469  different existi
-00003dd0: 6e67 2063 6f6e 7465 7374 2069 6e20 6578  ng contest in ex
-00003de0: 6973 7469 6e67 2064 6174 6162 6173 652e  isting database.
-00003df0: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
-00003e00: 6572 2e64 6562 7567 2822 4f70 656e 2043  er.debug("Open C
-00003e10: 6f6e 7465 7374 2073 656c 6563 7465 6422  ontest selected"
-00003e20: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-00003e30: 7473 203d 2073 656c 662e 6461 7461 6261  ts = self.databa
-00003e40: 7365 2e66 6574 6368 5f61 6c6c 5f63 6f6e  se.fetch_all_con
-00003e50: 7465 7374 7328 290a 2020 2020 2020 2020  tests().        
-00003e60: 6c6f 6767 6572 2e64 6562 7567 2822 2573  logger.debug("%s
-00003e70: 222c 2066 227b 636f 6e74 6573 7473 7d22  ", f"{contests}"
-00003e80: 290a 0a20 2020 2020 2020 2069 6620 636f  )..        if co
-00003e90: 6e74 6573 7473 3a0a 2020 2020 2020 2020  ntests:.        
-00003ea0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00003eb0: 5f64 6961 6c6f 6720 3d20 5365 6c65 6374  _dialog = Select
-00003ec0: 436f 6e74 6573 7428 574f 524b 494e 475f  Contest(WORKING_
-00003ed0: 5041 5448 290a 2020 2020 2020 2020 2020  PATH).          
-00003ee0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00003ef0: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
-00003f00: 7374 2e73 6574 526f 7743 6f75 6e74 2830  st.setRowCount(0
-00003f10: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00003f20: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00003f30: 672e 636f 6e74 6573 745f 6c69 7374 2e73  g.contest_list.s
-00003f40: 6574 436f 6c75 6d6e 436f 756e 7428 3429  etColumnCount(4)
-00003f50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003f60: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00003f70: 2e63 6f6e 7465 7374 5f6c 6973 742e 7665  .contest_list.ve
-00003f80: 7274 6963 616c 4865 6164 6572 2829 2e73  rticalHeader().s
-00003f90: 6574 5669 7369 626c 6528 4661 6c73 6529  etVisible(False)
-00003fa0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003fb0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00003fc0: 2e63 6f6e 7465 7374 5f6c 6973 742e 7365  .contest_list.se
-00003fd0: 7443 6f6c 756d 6e57 6964 7468 2831 2c20  tColumnWidth(1, 
-00003fe0: 3230 3029 0a20 2020 2020 2020 2020 2020  200).           
-00003ff0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00004000: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
-00004010: 742e 7365 7443 6f6c 756d 6e57 6964 7468  t.setColumnWidth
-00004020: 2832 2c20 3230 3029 0a20 2020 2020 2020  (2, 200).       
-00004030: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00004040: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
-00004050: 5f6c 6973 742e 7365 7448 6f72 697a 6f6e  _list.setHorizon
-00004060: 7461 6c48 6561 6465 7249 7465 6d28 0a20  talHeaderItem(. 
-00004070: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00004080: 2c20 5174 5769 6467 6574 732e 5154 6162  , QtWidgets.QTab
-00004090: 6c65 5769 6467 6574 4974 656d 2822 436f  leWidgetItem("Co
-000040a0: 6e74 6573 7420 4e72 2229 0a20 2020 2020  ntest Nr").     
-000040b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000040c0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-000040d0: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
-000040e0: 5f6c 6973 742e 7365 7448 6f72 697a 6f6e  _list.setHorizon
-000040f0: 7461 6c48 6561 6465 7249 7465 6d28 0a20  talHeaderItem(. 
-00004100: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00004110: 2c20 5174 5769 6467 6574 732e 5154 6162  , QtWidgets.QTab
-00004120: 6c65 5769 6467 6574 4974 656d 2822 436f  leWidgetItem("Co
-00004130: 6e74 6573 7420 4e61 6d65 2229 0a20 2020  ntest Name").   
-00004140: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00004150: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00004160: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
-00004170: 7374 5f6c 6973 742e 7365 7448 6f72 697a  st_list.setHoriz
-00004180: 6f6e 7461 6c48 6561 6465 7249 7465 6d28  ontalHeaderItem(
-00004190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000041a0: 2032 2c20 5174 5769 6467 6574 732e 5154   2, QtWidgets.QT
-000041b0: 6162 6c65 5769 6467 6574 4974 656d 2822  ableWidgetItem("
-000041c0: 436f 6e74 6573 7420 5374 6172 7422 290a  Contest Start").
-000041d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000041e0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000041f0: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
-00004200: 6e74 6573 745f 6c69 7374 2e73 6574 486f  ntest_list.setHo
-00004210: 7269 7a6f 6e74 616c 4865 6164 6572 4974  rizontalHeaderIt
-00004220: 656d 280a 2020 2020 2020 2020 2020 2020  em(.            
-00004230: 2020 2020 332c 2051 7457 6964 6765 7473      3, QtWidgets
-00004240: 2e51 5461 626c 6557 6964 6765 7449 7465  .QTableWidgetIte
-00004250: 6d28 224e 6f74 2055 4973 6564 2229 0a20  m("Not UIsed"). 
-00004260: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00004270: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00004280: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
-00004290: 7465 7374 5f6c 6973 742e 7365 7443 6f6c  test_list.setCol
-000042a0: 756d 6e48 6964 6465 6e28 302c 2054 7275  umnHidden(0, Tru
-000042b0: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-000042c0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-000042d0: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
-000042e0: 7365 7443 6f6c 756d 6e48 6964 6465 6e28  setColumnHidden(
-000042f0: 332c 2054 7275 6529 0a20 2020 2020 2020  3, True).       
-00004300: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00004310: 745f 6469 616c 6f67 2e61 6363 6570 7465  t_dialog.accepte
-00004320: 642e 636f 6e6e 6563 7428 7365 6c66 2e6f  d.connect(self.o
-00004330: 7065 6e5f 636f 6e74 6573 745f 7265 7475  pen_contest_retu
-00004340: 726e 290a 2020 2020 2020 2020 2020 2020  rn).            
-00004350: 666f 7220 636f 6e74 6573 7420 696e 2063  for contest in c
-00004360: 6f6e 7465 7374 733a 0a20 2020 2020 2020  ontests:.       
-00004370: 2020 2020 2020 2020 206e 756d 6265 725f           number_
-00004380: 6f66 5f72 6f77 7320 3d20 7365 6c66 2e63  of_rows = self.c
-00004390: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
-000043a0: 6e74 6573 745f 6c69 7374 2e72 6f77 436f  ntest_list.rowCo
-000043b0: 756e 7428 290a 2020 2020 2020 2020 2020  unt().          
-000043c0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-000043d0: 7374 5f64 6961 6c6f 672e 636f 6e74 6573  st_dialog.contes
-000043e0: 745f 6c69 7374 2e69 6e73 6572 7452 6f77  t_list.insertRow
-000043f0: 286e 756d 6265 725f 6f66 5f72 6f77 7329  (number_of_rows)
-00004400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004410: 2063 6f6e 7465 7374 5f69 6420 3d20 7374   contest_id = st
-00004420: 7228 636f 6e74 6573 742e 6765 7428 2243  r(contest.get("C
-00004430: 6f6e 7465 7374 4944 222c 2031 2929 0a20  ontestID", 1)). 
-00004440: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00004450: 6f6e 7465 7374 5f6e 616d 6520 3d20 636f  ontest_name = co
-00004460: 6e74 6573 742e 6765 7428 2243 6f6e 7465  ntest.get("Conte
-00004470: 7374 4e61 6d65 222c 2031 290a 2020 2020  stName", 1).    
-00004480: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00004490: 745f 6461 7465 203d 2063 6f6e 7465 7374  t_date = contest
-000044a0: 2e67 6574 2822 5374 6172 7444 6174 6522  .get("StartDate"
-000044b0: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
-000044c0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-000044d0: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
-000044e0: 5f6c 6973 742e 7365 7449 7465 6d28 0a20  _list.setItem(. 
-000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004500: 2020 206e 756d 6265 725f 6f66 5f72 6f77     number_of_row
-00004510: 732c 2030 2c20 5174 5769 6467 6574 732e  s, 0, QtWidgets.
-00004520: 5154 6162 6c65 5769 6467 6574 4974 656d  QTableWidgetItem
-00004530: 2863 6f6e 7465 7374 5f69 6429 0a20 2020  (contest_id).   
-00004540: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00004550: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004560: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004570: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
-00004580: 7365 7449 7465 6d28 0a20 2020 2020 2020  setItem(.       
-00004590: 2020 2020 2020 2020 2020 2020 206e 756d               num
-000045a0: 6265 725f 6f66 5f72 6f77 732c 2031 2c20  ber_of_rows, 1, 
-000045b0: 5174 5769 6467 6574 732e 5154 6162 6c65  QtWidgets.QTable
-000045c0: 5769 6467 6574 4974 656d 2863 6f6e 7465  WidgetItem(conte
-000045d0: 7374 5f6e 616d 6529 0a20 2020 2020 2020  st_name).       
-000045e0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000045f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004600: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
-00004610: 6f6e 7465 7374 5f6c 6973 742e 7365 7449  ontest_list.setI
-00004620: 7465 6d28 0a20 2020 2020 2020 2020 2020  tem(.           
-00004630: 2020 2020 2020 2020 206e 756d 6265 725f           number_
-00004640: 6f66 5f72 6f77 732c 2032 2c20 5174 5769  of_rows, 2, QtWi
-00004650: 6467 6574 732e 5154 6162 6c65 5769 6467  dgets.QTableWidg
-00004660: 6574 4974 656d 2873 7461 7274 5f64 6174  etItem(start_dat
-00004670: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00004680: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-00004690: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-000046a0: 2e73 686f 7728 290a 0a20 2020 2064 6566  .show()..    def
-000046b0: 206f 7065 6e5f 636f 6e74 6573 745f 7265   open_contest_re
-000046c0: 7475 726e 2873 656c 6629 3a0a 2020 2020  turn(self):.    
-000046d0: 2020 2020 2222 2243 616c 6c65 6420 6279      """Called by
-000046e0: 206f 7065 6e5f 636f 6e74 6573 7422 2222   open_contest"""
-000046f0: 0a20 2020 2020 2020 2073 656c 6563 7465  .        selecte
-00004700: 645f 726f 7720 3d20 7365 6c66 2e63 6f6e  d_row = self.con
-00004710: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
-00004720: 6573 745f 6c69 7374 2e63 7572 7265 6e74  est_list.current
-00004730: 526f 7728 290a 2020 2020 2020 2020 636f  Row().        co
-00004740: 6e74 6573 7420 3d20 7365 6c66 2e63 6f6e  ntest = self.con
-00004750: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
-00004760: 6573 745f 6c69 7374 2e69 7465 6d28 7365  est_list.item(se
-00004770: 6c65 6374 6564 5f72 6f77 2c20 3029 2e74  lected_row, 0).t
-00004780: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
-00004790: 6c66 2e70 7265 665b 2263 6f6e 7465 7374  lf.pref["contest
-000047a0: 225d 203d 2063 6f6e 7465 7374 0a20 2020  "] = contest.   
-000047b0: 2020 2020 2073 656c 662e 7772 6974 655f       self.write_
-000047c0: 7072 6566 6572 656e 6365 2829 0a20 2020  preference().   
-000047d0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-000047e0: 6728 2253 656c 6563 7465 6420 636f 6e74  g("Selected cont
-000047f0: 6573 743a 2025 7322 2c20 6622 7b63 6f6e  est: %s", f"{con
-00004800: 7465 7374 7d22 290a 2020 2020 2020 2020  test}").        
-00004810: 7365 6c66 2e6c 6f61 645f 636f 6e74 6573  self.load_contes
-00004820: 7428 290a 0a20 2020 2064 6566 2072 6566  t()..    def ref
-00004830: 696c 6c5f 6472 6f70 646f 776e 2873 656c  ill_dropdown(sel
-00004840: 662c 2074 6172 6765 742c 2073 6f75 7263  f, target, sourc
-00004850: 6529 3a0a 2020 2020 2020 2020 2222 2252  e):.        """R
-00004860: 6566 696c 6c20 5143 6f6d 626f 626f 7820  efill QCombobox 
-00004870: 7769 6467 6574 2077 6974 6820 7661 6c75  widget with valu
-00004880: 652e 2222 220a 2020 2020 2020 2020 696e  e.""".        in
-00004890: 6465 7820 3d20 7461 7267 6574 2e66 696e  dex = target.fin
-000048a0: 6454 6578 7428 736f 7572 6365 290a 2020  dText(source).  
-000048b0: 2020 2020 2020 7461 7267 6574 2e73 6574        target.set
-000048c0: 4375 7272 656e 7449 6e64 6578 2869 6e64  CurrentIndex(ind
-000048d0: 6578 290a 0a20 2020 2064 6566 2065 6469  ex)..    def edi
-000048e0: 745f 636f 6e74 6573 7428 7365 6c66 293a  t_contest(self):
-000048f0: 0a20 2020 2020 2020 2022 2222 4564 6974  .        """Edit
-00004900: 2074 6865 2063 7572 7265 6e74 2063 6f6e   the current con
-00004910: 7465 7374 2222 220a 2020 2020 2020 2020  test""".        
-00004920: 6c6f 6767 6572 2e64 6562 7567 2822 4564  logger.debug("Ed
-00004930: 6974 2063 6f6e 7465 7374 2044 6961 6c6f  it contest Dialo
-00004940: 6722 290a 2020 2020 2020 2020 6966 2073  g").        if s
-00004950: 656c 662e 636f 6e74 6573 7420 6973 204e  elf.contest is N
-00004960: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00004970: 2073 656c 662e 7368 6f77 5f6d 6573 7361   self.show_messa
-00004980: 6765 5f62 6f78 2822 596f 7520 6861 7665  ge_box("You have
-00004990: 206e 6f20 636f 6e74 6573 7420 6465 6669   no contest defi
-000049a0: 6e65 642e 2229 0a20 2020 2020 2020 2020  ned.").         
-000049b0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-000049c0: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
-000049d0: 745f 7365 7474 696e 6773 2069 7320 4e6f  t_settings is No
-000049e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000049f0: 7265 7475 726e 0a20 2020 2020 2020 2073  return.        s
-00004a00: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004a10: 6f67 203d 204e 6577 436f 6e74 6573 7428  og = NewContest(
-00004a20: 574f 524b 494e 475f 5041 5448 290a 2020  WORKING_PATH).  
-00004a30: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00004a40: 7374 5f64 6961 6c6f 672e 7365 7457 696e  st_dialog.setWin
-00004a50: 646f 7754 6974 6c65 2822 4564 6974 2043  dowTitle("Edit C
-00004a60: 6f6e 7465 7374 2229 0a20 2020 2020 2020  ontest").       
-00004a70: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00004a80: 616c 6f67 2e74 6974 6c65 2e73 6574 5465  alog.title.setTe
-00004a90: 7874 2822 2229 0a20 2020 2020 2020 2073  xt("").        s
-00004aa0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004ab0: 6f67 2e61 6363 6570 7465 642e 636f 6e6e  og.accepted.conn
-00004ac0: 6563 7428 7365 6c66 2e73 6176 655f 6564  ect(self.save_ed
-00004ad0: 6974 6564 5f63 6f6e 7465 7374 290a 2020  ited_contest).  
-00004ae0: 2020 2020 2020 7661 6c75 6520 3d20 7365        value = se
-00004af0: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
-00004b00: 6e67 732e 6765 7428 2243 6f6e 7465 7374  ngs.get("Contest
-00004b10: 4e61 6d65 2229 2e75 7070 6572 2829 2e72  Name").upper().r
-00004b20: 6570 6c61 6365 2822 5f22 2c20 2220 2229  eplace("_", " ")
-00004b30: 0a20 2020 2020 2020 2069 6620 7661 6c75  .        if valu
-00004b40: 6520 3d3d 2022 4745 4e45 5241 4c20 4c4f  e == "GENERAL LO
-00004b50: 4747 494e 4722 3a0a 2020 2020 2020 2020  GGING":.        
-00004b60: 2020 2020 7661 6c75 6520 3d20 2247 656e      value = "Gen
-00004b70: 6572 616c 204c 6f67 6769 6e67 220a 2020  eral Logging".  
-00004b80: 2020 2020 2020 7365 6c66 2e72 6566 696c        self.refil
-00004b90: 6c5f 6472 6f70 646f 776e 2873 656c 662e  l_dropdown(self.
-00004ba0: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
-00004bb0: 6f6e 7465 7374 2c20 7661 6c75 6529 0a20  ontest, value). 
-00004bc0: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
-00004bd0: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
-00004be0: 696e 6773 2e67 6574 2822 4f70 6572 6174  ings.get("Operat
-00004bf0: 6f72 4361 7465 676f 7279 2229 0a20 2020  orCategory").   
-00004c00: 2020 2020 2073 656c 662e 7265 6669 6c6c       self.refill
-00004c10: 5f64 726f 7064 6f77 6e28 7365 6c66 2e63  _dropdown(self.c
-00004c20: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
-00004c30: 6572 6174 6f72 5f63 6c61 7373 2c20 7661  erator_class, va
-00004c40: 6c75 6529 0a20 2020 2020 2020 2076 616c  lue).        val
-00004c50: 7565 203d 2073 656c 662e 636f 6e74 6573  ue = self.contes
-00004c60: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
-00004c70: 4261 6e64 4361 7465 676f 7279 2229 0a20  BandCategory"). 
-00004c80: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
-00004c90: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
-00004ca0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00004cb0: 6261 6e64 2c20 7661 6c75 6529 0a20 2020  band, value).   
-00004cc0: 2020 2020 2076 616c 7565 203d 2073 656c       value = sel
-00004cd0: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
-00004ce0: 6773 2e67 6574 2822 506f 7765 7243 6174  gs.get("PowerCat
-00004cf0: 6567 6f72 7922 290a 2020 2020 2020 2020  egory").        
-00004d00: 7365 6c66 2e72 6566 696c 6c5f 6472 6f70  self.refill_drop
-00004d10: 646f 776e 2873 656c 662e 636f 6e74 6573  down(self.contes
-00004d20: 745f 6469 616c 6f67 2e70 6f77 6572 2c20  t_dialog.power, 
-00004d30: 7661 6c75 6529 0a20 2020 2020 2020 2076  value).        v
-00004d40: 616c 7565 203d 2073 656c 662e 636f 6e74  alue = self.cont
-00004d50: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
-00004d60: 2822 4d6f 6465 4361 7465 676f 7279 2229  ("ModeCategory")
-00004d70: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00004d80: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
-00004d90: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00004da0: 672e 6d6f 6465 2c20 7661 6c75 6529 0a20  g.mode, value). 
-00004db0: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
-00004dc0: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
-00004dd0: 696e 6773 2e67 6574 2822 4f76 6572 6c61  ings.get("Overla
-00004de0: 7943 6174 6567 6f72 7922 290a 2020 2020  yCategory").    
-00004df0: 2020 2020 7365 6c66 2e72 6566 696c 6c5f      self.refill_
-00004e00: 6472 6f70 646f 776e 2873 656c 662e 636f  dropdown(self.co
-00004e10: 6e74 6573 745f 6469 616c 6f67 2e6f 7665  ntest_dialog.ove
-00004e20: 726c 6179 2c20 7661 6c75 6529 0a20 2020  rlay, value).   
-00004e30: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00004e40: 745f 6469 616c 6f67 2e6f 7065 7261 746f  t_dialog.operato
-00004e50: 7273 2e73 6574 5465 7874 2873 656c 662e  rs.setText(self.
-00004e60: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
-00004e70: 2e67 6574 2822 4f70 6572 6174 6f72 7322  .get("Operators"
-00004e80: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00004e90: 636f 6e74 6573 745f 6469 616c 6f67 2e73  contest_dialog.s
-00004ea0: 6f61 7062 6f78 2e73 6574 506c 6169 6e54  oapbox.setPlainT
-00004eb0: 6578 7428 7365 6c66 2e63 6f6e 7465 7374  ext(self.contest
-00004ec0: 5f73 6574 7469 6e67 732e 6765 7428 2253  _settings.get("S
-00004ed0: 6f61 7062 6f78 2229 290a 2020 2020 2020  oapbox")).      
-00004ee0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00004ef0: 6961 6c6f 672e 6578 6368 616e 6765 2e73  ialog.exchange.s
-00004f00: 6574 5465 7874 2873 656c 662e 636f 6e74  etText(self.cont
-00004f10: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
-00004f20: 2822 5365 6e74 4578 6368 616e 6765 2229  ("SentExchange")
-00004f30: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
-00004f40: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
-00004f50: 6574 7469 6e67 732e 6765 7428 2253 7461  ettings.get("Sta
-00004f60: 7469 6f6e 4361 7465 676f 7279 2229 0a20  tionCategory"). 
-00004f70: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
-00004f80: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
-00004f90: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00004fa0: 7374 6174 696f 6e2c 2076 616c 7565 290a  station, value).
-00004fb0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-00004fc0: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-00004fd0: 7469 6e67 732e 6765 7428 2241 7373 6973  tings.get("Assis
-00004fe0: 7465 6443 6174 6567 6f72 7922 290a 2020  tedCategory").  
-00004ff0: 2020 2020 2020 7365 6c66 2e72 6566 696c        self.refil
-00005000: 6c5f 6472 6f70 646f 776e 2873 656c 662e  l_dropdown(self.
-00005010: 636f 6e74 6573 745f 6469 616c 6f67 2e61  contest_dialog.a
-00005020: 7373 6973 7465 642c 2076 616c 7565 290a  ssisted, value).
-00005030: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-00005040: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-00005050: 7469 6e67 732e 6765 7428 2254 7261 6e73  tings.get("Trans
-00005060: 6d69 7474 6572 4361 7465 676f 7279 2229  mitterCategory")
-00005070: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00005080: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
-00005090: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-000050a0: 672e 7472 616e 736d 6974 7465 722c 2076  g.transmitter, v
-000050b0: 616c 7565 290a 2020 2020 2020 2020 7661  alue).        va
-000050c0: 6c75 6520 3d20 7365 6c66 2e63 6f6e 7465  lue = self.conte
-000050d0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
-000050e0: 2253 7461 7274 4461 7465 2229 0a20 2020  "StartDate").   
-000050f0: 2020 2020 2074 6865 5f64 6174 652c 2074       the_date, t
-00005100: 6865 5f74 696d 6520 3d20 7661 6c75 652e  he_time = value.
-00005110: 7370 6c69 7428 290a 2020 2020 2020 2020  split().        
-00005120: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00005130: 6c6f 672e 6461 7465 5469 6d65 4564 6974  log.dateTimeEdit
-00005140: 2e73 6574 4461 7465 280a 2020 2020 2020  .setDate(.      
-00005150: 2020 2020 2020 5174 436f 7265 2e51 4461        QtCore.QDa
-00005160: 7465 2e66 726f 6d53 7472 696e 6728 7468  te.fromString(th
-00005170: 655f 6461 7465 2c20 2279 7979 792d 4d4d  e_date, "yyyy-MM
-00005180: 2d64 6422 290a 2020 2020 2020 2020 290a  -dd").        ).
-00005190: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000051a0: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
-000051b0: 5469 6d65 4564 6974 2e73 6574 4361 6c65  TimeEdit.setCale
-000051c0: 6e64 6172 506f 7075 7028 5472 7565 290a  ndarPopup(True).
-000051d0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000051e0: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
-000051f0: 5469 6d65 4564 6974 2e73 6574 5469 6d65  TimeEdit.setTime
-00005200: 280a 2020 2020 2020 2020 2020 2020 5174  (.            Qt
-00005210: 436f 7265 2e51 5469 6d65 2e66 726f 6d53  Core.QTime.fromS
-00005220: 7472 696e 6728 7468 655f 7469 6d65 2c20  tring(the_time, 
-00005230: 2268 683a 6d6d 3a73 7322 290a 2020 2020  "hh:mm:ss").    
-00005240: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-00005250: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00005260: 672e 6f70 656e 2829 0a0a 2020 2020 6465  g.open()..    de
-00005270: 6620 7361 7665 5f65 6469 7465 645f 636f  f save_edited_co
-00005280: 6e74 6573 7428 7365 6c66 293a 0a20 2020  ntest(self):.   
-00005290: 2020 2020 2022 2222 5361 7665 2074 6865       """Save the
-000052a0: 2065 6469 7465 6420 636f 6e74 6573 7422   edited contest"
-000052b0: 2222 0a20 2020 2020 2020 2063 6f6e 7465  "".        conte
-000052c0: 7374 203d 207b 7d0a 2020 2020 2020 2020  st = {}.        
-000052d0: 636f 6e74 6573 745b 2243 6f6e 7465 7374  contest["Contest
-000052e0: 4e61 6d65 225d 203d 2028 0a20 2020 2020  Name"] = (.     
-000052f0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00005300: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
-00005310: 7374 2e63 7572 7265 6e74 5465 7874 2829  st.currentText()
-00005320: 2e6c 6f77 6572 2829 2e72 6570 6c61 6365  .lower().replace
-00005330: 2822 2022 2c20 225f 2229 0a20 2020 2020  (" ", "_").     
-00005340: 2020 2029 0a20 2020 2020 2020 2063 6f6e     ).        con
-00005350: 7465 7374 5b22 5374 6172 7444 6174 6522  test["StartDate"
-00005360: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-00005370: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
-00005380: 4564 6974 2e64 6174 6554 696d 6528 292e  Edit.dateTime().
-00005390: 746f 5374 7269 6e67 280a 2020 2020 2020  toString(.      
-000053a0: 2020 2020 2020 2279 7979 792d 4d4d 2d64        "yyyy-MM-d
-000053b0: 6420 6868 3a6d 6d3a 7373 220a 2020 2020  d hh:mm:ss".    
-000053c0: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
-000053d0: 6e74 6573 745b 224f 7065 7261 746f 7243  ntest["OperatorC
-000053e0: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
-000053f0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00005400: 6f70 6572 6174 6f72 5f63 6c61 7373 2e63  operator_class.c
-00005410: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
-00005420: 2020 2020 2063 6f6e 7465 7374 5b22 4261       contest["Ba
-00005430: 6e64 4361 7465 676f 7279 225d 203d 2073  ndCategory"] = s
-00005440: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00005450: 6f67 2e62 616e 642e 6375 7272 656e 7454  og.band.currentT
-00005460: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
-00005470: 6e74 6573 745b 2250 6f77 6572 4361 7465  ntest["PowerCate
-00005480: 676f 7279 225d 203d 2073 656c 662e 636f  gory"] = self.co
-00005490: 6e74 6573 745f 6469 616c 6f67 2e70 6f77  ntest_dialog.pow
-000054a0: 6572 2e63 7572 7265 6e74 5465 7874 2829  er.currentText()
-000054b0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-000054c0: 5b22 4d6f 6465 4361 7465 676f 7279 225d  ["ModeCategory"]
-000054d0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-000054e0: 6469 616c 6f67 2e6d 6f64 652e 6375 7272  dialog.mode.curr
-000054f0: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
-00005500: 2020 636f 6e74 6573 745b 224f 7665 726c    contest["Overl
-00005510: 6179 4361 7465 676f 7279 225d 203d 2073  ayCategory"] = s
-00005520: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00005530: 6f67 2e6f 7665 726c 6179 2e63 7572 7265  og.overlay.curre
-00005540: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
-00005550: 2063 6f6e 7465 7374 5b22 4f70 6572 6174   contest["Operat
-00005560: 6f72 7322 5d20 3d20 7365 6c66 2e63 6f6e  ors"] = self.con
-00005570: 7465 7374 5f64 6961 6c6f 672e 6f70 6572  test_dialog.oper
-00005580: 6174 6f72 732e 7465 7874 2829 0a20 2020  ators.text().   
-00005590: 2020 2020 2063 6f6e 7465 7374 5b22 536f       contest["So
-000055a0: 6170 626f 7822 5d20 3d20 7365 6c66 2e63  apbox"] = self.c
-000055b0: 6f6e 7465 7374 5f64 6961 6c6f 672e 736f  ontest_dialog.so
-000055c0: 6170 626f 782e 746f 506c 6169 6e54 6578  apbox.toPlainTex
-000055d0: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
-000055e0: 6573 745b 2253 656e 7445 7863 6861 6e67  est["SentExchang
-000055f0: 6522 5d20 3d20 7365 6c66 2e63 6f6e 7465  e"] = self.conte
-00005600: 7374 5f64 6961 6c6f 672e 6578 6368 616e  st_dialog.exchan
-00005610: 6765 2e74 6578 7428 290a 2020 2020 2020  ge.text().      
-00005620: 2020 636f 6e74 6573 745b 2243 6f6e 7465    contest["Conte
-00005630: 7374 4e52 225d 203d 2073 656c 662e 7072  stNR"] = self.pr
-00005640: 6566 2e67 6574 2822 636f 6e74 6573 7422  ef.get("contest"
-00005650: 2c20 3129 0a20 2020 2020 2020 2063 6f6e  , 1).        con
-00005660: 7465 7374 5b22 5374 6174 696f 6e43 6174  test["StationCat
-00005670: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
-00005680: 6f6e 7465 7374 5f64 6961 6c6f 672e 7374  ontest_dialog.st
-00005690: 6174 696f 6e2e 6375 7272 656e 7454 6578  ation.currentTex
-000056a0: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
-000056b0: 6573 745b 2241 7373 6973 7465 6443 6174  est["AssistedCat
-000056c0: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
-000056d0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6173  ontest_dialog.as
-000056e0: 7369 7374 6564 2e63 7572 7265 6e74 5465  sisted.currentTe
-000056f0: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
-00005700: 7465 7374 5b22 5472 616e 736d 6974 7465  test["Transmitte
-00005710: 7243 6174 6567 6f72 7922 5d20 3d20 7365  rCategory"] = se
-00005720: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00005730: 672e 7472 616e 736d 6974 7465 722e 6375  g.transmitter.cu
-00005740: 7272 656e 7454 6578 7428 290a 0a20 2020  rrentText()..   
-00005750: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00005760: 6728 2225 7322 2c20 6622 7b63 6f6e 7465  g("%s", f"{conte
-00005770: 7374 7d22 290a 2020 2020 2020 2020 7365  st}").        se
-00005780: 6c66 2e64 6174 6162 6173 652e 7570 6461  lf.database.upda
-00005790: 7465 5f63 6f6e 7465 7374 2863 6f6e 7465  te_contest(conte
-000057a0: 7374 290a 2020 2020 2020 2020 7365 6c66  st).        self
-000057b0: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
-000057c0: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-000057d0: 2e6c 6f61 645f 636f 6e74 6573 7428 290a  .load_contest().
-000057e0: 0a20 2020 2064 6566 206c 6f61 645f 636f  .    def load_co
-000057f0: 6e74 6573 7428 7365 6c66 293a 0a20 2020  ntest(self):.   
-00005800: 2020 2020 2022 2222 6c6f 6164 2061 2063       """load a c
-00005810: 6f6e 7465 7374 2222 220a 2020 2020 2020  ontest""".      
-00005820: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-00005830: 6574 2822 636f 6e74 6573 7422 293a 0a20  et("contest"):. 
-00005840: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005850: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
-00005860: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
-00005870: 2e66 6574 6368 5f63 6f6e 7465 7374 5f62  .fetch_contest_b
-00005880: 795f 6964 280a 2020 2020 2020 2020 2020  y_id(.          
-00005890: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-000058a0: 6765 7428 2263 6f6e 7465 7374 2229 0a20  get("contest"). 
-000058b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000058c0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000058d0: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
-000058e0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000058f0: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
-00005900: 2e63 7572 7265 6e74 5f63 6f6e 7465 7374  .current_contest
-00005910: 203d 2073 656c 662e 7072 6566 2e67 6574   = self.pref.get
-00005920: 2822 636f 6e74 6573 7422 290a 2020 2020  ("contest").    
-00005930: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00005940: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
-00005950: 696e 6773 2e67 6574 2822 436f 6e74 6573  ings.get("Contes
-00005960: 744e 616d 6522 293a 0a20 2020 2020 2020  tName"):.       
-00005970: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005980: 662e 636f 6e74 6573 7420 3d20 646f 696d  f.contest = doim
-00005990: 7028 7365 6c66 2e63 6f6e 7465 7374 5f73  p(self.contest_s
-000059a0: 6574 7469 6e67 732e 6765 7428 2243 6f6e  ettings.get("Con
-000059b0: 7465 7374 4e61 6d65 2229 290a 2020 2020  testName")).    
-000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059d0: 6c6f 6767 6572 2e64 6562 7567 2822 4c6f  logger.debug("Lo
-000059e0: 6164 6564 2043 6f6e 7465 7374 204e 616d  aded Contest Nam
-000059f0: 6520 3d20 2573 222c 2073 656c 662e 636f  e = %s", self.co
-00005a00: 6e74 6573 742e 6e61 6d65 290a 2020 2020  ntest.name).    
-00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a20: 7365 6c66 2e73 6574 5f77 696e 646f 775f  self.set_window_
-00005a30: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
-00005a40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005a50: 2e63 6f6e 7465 7374 2e69 6e69 745f 636f  .contest.init_co
-00005a60: 6e74 6573 7428 7365 6c66 290a 2020 2020  ntest(self).    
-00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a80: 7365 6c66 2e68 6964 655f 6261 6e64 5f6d  self.hide_band_m
-00005a90: 6f64 6528 7365 6c66 2e63 6f6e 7465 7374  ode(self.contest
-00005aa0: 5f73 6574 7469 6e67 732e 6765 7428 224d  _settings.get("M
-00005ab0: 6f64 6543 6174 6567 6f72 7922 2c20 2222  odeCategory", ""
-00005ac0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00005ad0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00005ae0: 6275 6728 2225 7322 2c20 6622 7b73 656c  bug("%s", f"{sel
-00005af0: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
-00005b00: 6773 7d22 290a 2020 2020 2020 2020 2020  gs}").          
-00005b10: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00005b20: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
-00005b30: 6773 2e67 6574 2822 4d6f 6465 4361 7465  gs.get("ModeCate
-00005b40: 676f 7279 222c 2022 2229 203d 3d20 2243  gory", "") == "C
-00005b50: 5722 3a0a 2020 2020 2020 2020 2020 2020  W":.            
-00005b60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005b70: 2e73 6574 6d6f 6465 2822 4357 2229 0a20  .setmode("CW"). 
-00005b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b90: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-00005ba0: 6f5f 7374 6174 655b 226d 6f64 6522 5d20  o_state["mode"] 
-00005bb0: 3d20 2243 5722 0a20 2020 2020 2020 2020  = "CW".         
-00005bc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005bd0: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
-00005be0: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-00005c10: 726f 6c2e 6f6e 6c69 6e65 3a0a 2020 2020  rol.online:.    
-00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005c40: 2e72 6967 5f63 6f6e 7472 6f6c 2e73 6574  .rig_control.set
-00005c50: 5f6d 6f64 6528 2243 5722 290a 2020 2020  _mode("CW").    
-00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c70: 2020 2020 6261 6e64 203d 2067 6574 6261      band = getba
-00005c80: 6e64 2873 7472 2873 656c 662e 7261 6469  nd(str(self.radi
-00005c90: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
-00005ca0: 6122 2c20 2230 2e30 2229 2929 0a20 2020  a", "0.0"))).   
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2020 2020 2073 656c 662e 7365 745f 6261       self.set_ba
-00005cd0: 6e64 5f69 6e64 6963 6174 6f72 2862 616e  nd_indicator(ban
-00005ce0: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-00005cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005d00: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
-00005d10: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00005d20: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00005d30: 6f6e 7465 7374 5f73 6574 7469 6e67 732e  ontest_settings.
-00005d40: 6765 7428 224d 6f64 6543 6174 6567 6f72  get("ModeCategor
-00005d50: 7922 2c20 2222 2920 3d3d 2022 5353 4222  y", "") == "SSB"
-00005d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005d70: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00005d80: 6574 6d6f 6465 2822 5353 4222 290a 2020  etmode("SSB").  
-00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005da0: 2020 2020 2020 6966 2069 6e74 2873 656c        if int(sel
-00005db0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-00005dc0: 7428 2276 666f 6122 2c20 3029 2920 3e20  t("vfoa", 0)) > 
-00005dd0: 3130 3030 3030 3030 3a0a 2020 2020 2020  10000000:.      
-00005de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005df0: 2020 2020 2020 7365 6c66 2e72 6164 696f        self.radio
-00005e00: 5f73 7461 7465 5b22 6d6f 6465 225d 203d  _state["mode"] =
-00005e10: 2022 5553 4222 0a20 2020 2020 2020 2020   "USB".         
-00005e20: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00005e30: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00001b80: 2073 656c 662e 7261 6469 6f42 7574 746f   self.radioButto
+00001b90: 6e5f 7275 6e2e 636c 6963 6b65 642e 636f  n_run.clicked.co
+00001ba0: 6e6e 6563 7428 7365 6c66 2e72 756e 5f73  nnect(self.run_s
+00001bb0: 705f 6275 7474 6f6e 735f 636c 6963 6b65  p_buttons_clicke
+00001bc0: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+00001bd0: 7261 6469 6f42 7574 746f 6e5f 7370 2e63  radioButton_sp.c
+00001be0: 6c69 636b 6564 2e63 6f6e 6e65 6374 2873  licked.connect(s
+00001bf0: 656c 662e 7275 6e5f 7370 5f62 7574 746f  elf.run_sp_butto
+00001c00: 6e73 5f63 6c69 636b 6564 290a 2020 2020  ns_clicked).    
+00001c10: 2020 2020 7365 6c66 2e73 636f 7265 2e73      self.score.s
+00001c20: 6574 5465 7874 2822 3022 290a 2020 2020  etText("0").    
+00001c30: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+00001c40: 6e2e 7465 7874 4564 6974 6564 2e63 6f6e  n.textEdited.con
+00001c50: 6e65 6374 2873 656c 662e 6361 6c6c 7369  nect(self.callsi
+00001c60: 676e 5f63 6861 6e67 6564 290a 2020 2020  gn_changed).    
+00001c70: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+00001c80: 6e2e 7265 7475 726e 5072 6573 7365 642e  n.returnPressed.
+00001c90: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
+00001ca0: 655f 636f 6e74 6163 7429 0a20 2020 2020  e_contact).     
+00001cb0: 2020 2073 656c 662e 7365 6e74 2e72 6574     self.sent.ret
+00001cc0: 7572 6e50 7265 7373 6564 2e63 6f6e 6e65  urnPressed.conne
+00001cd0: 6374 2873 656c 662e 7361 7665 5f63 6f6e  ct(self.save_con
+00001ce0: 7461 6374 290a 2020 2020 2020 2020 7365  tact).        se
+00001cf0: 6c66 2e72 6563 6569 7665 2e72 6574 7572  lf.receive.retur
+00001d00: 6e50 7265 7373 6564 2e63 6f6e 6e65 6374  nPressed.connect
+00001d10: 2873 656c 662e 7361 7665 5f63 6f6e 7461  (self.save_conta
+00001d20: 6374 290a 2020 2020 2020 2020 7365 6c66  ct).        self
+00001d30: 2e6f 7468 6572 5f31 2e72 6574 7572 6e50  .other_1.returnP
+00001d40: 7265 7373 6564 2e63 6f6e 6e65 6374 2873  ressed.connect(s
+00001d50: 656c 662e 7361 7665 5f63 6f6e 7461 6374  elf.save_contact
+00001d60: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
+00001d70: 7468 6572 5f32 2e72 6574 7572 6e50 7265  ther_2.returnPre
+00001d80: 7373 6564 2e63 6f6e 6e65 6374 2873 656c  ssed.connect(sel
+00001d90: 662e 7361 7665 5f63 6f6e 7461 6374 290a  f.save_contact).
+00001da0: 2020 2020 2020 2020 7365 6c66 2e6f 7468          self.oth
+00001db0: 6572 5f32 2e74 6578 7445 6469 7465 642e  er_2.textEdited.
+00001dc0: 636f 6e6e 6563 7428 7365 6c66 2e6f 7468  connect(self.oth
+00001dd0: 6572 5f32 5f63 6861 6e67 6564 290a 0a20  er_2_changed).. 
+00001de0: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
+00001df0: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
+00001e00: 2020 2020 2020 2073 656c 662e 7265 6365         self.rece
+00001e10: 6976 652e 7365 7454 6578 7428 2235 3922  ive.setText("59"
+00001e20: 290a 2020 2020 2020 2020 6963 6f6e 5f70  ).        icon_p
+00001e30: 6174 6820 3d20 574f 524b 494e 475f 5041  ath = WORKING_PA
+00001e40: 5448 202b 2022 2f64 6174 612f 220a 2020  TH + "/data/".  
+00001e50: 2020 2020 2020 7365 6c66 2e67 7265 656e        self.green
+00001e60: 646f 7420 3d20 5174 4775 692e 5150 6978  dot = QtGui.QPix
+00001e70: 6d61 7028 6963 6f6e 5f70 6174 6820 2b20  map(icon_path + 
+00001e80: 2267 7265 656e 646f 742e 706e 6722 290a  "greendot.png").
+00001e90: 2020 2020 2020 2020 7365 6c66 2e72 6564          self.red
+00001ea0: 646f 7420 3d20 5174 4775 692e 5150 6978  dot = QtGui.QPix
+00001eb0: 6d61 7028 6963 6f6e 5f70 6174 6820 2b20  map(icon_path + 
+00001ec0: 2272 6564 646f 742e 706e 6722 290a 2020  "reddot.png").  
+00001ed0: 2020 2020 2020 7365 6c66 2e6c 6566 7464        self.leftd
+00001ee0: 6f74 2e73 6574 5069 786d 6170 2873 656c  ot.setPixmap(sel
+00001ef0: 662e 6772 6565 6e64 6f74 290a 2020 2020  f.greendot).    
+00001f00: 2020 2020 7365 6c66 2e72 6967 6874 646f      self.rightdo
+00001f10: 742e 7365 7450 6978 6d61 7028 7365 6c66  t.setPixmap(self
+00001f20: 2e72 6564 646f 7429 0a0a 2020 2020 2020  .reddot)..      
+00001f30: 2020 7365 6c66 2e46 312e 7365 7443 6f6e    self.F1.setCon
+00001f40: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00001f50: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00001f60: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00001f70: 2020 2020 7365 6c66 2e46 312e 6375 7374      self.F1.cust
+00001f80: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00001f90: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00001fa0: 656c 662e 6564 6974 5f46 3129 0a20 2020  elf.edit_F1).   
+00001fb0: 2020 2020 2073 656c 662e 4631 2e63 6c69       self.F1.cli
+00001fc0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00001fd0: 662e 7365 6e64 6631 290a 2020 2020 2020  f.sendf1).      
+00001fe0: 2020 7365 6c66 2e46 322e 7365 7443 6f6e    self.F2.setCon
+00001ff0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002000: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002010: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002020: 2020 2020 7365 6c66 2e46 322e 6375 7374      self.F2.cust
+00002030: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002040: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002050: 656c 662e 6564 6974 5f46 3229 0a20 2020  elf.edit_F2).   
+00002060: 2020 2020 2073 656c 662e 4632 2e63 6c69       self.F2.cli
+00002070: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002080: 662e 7365 6e64 6632 290a 2020 2020 2020  f.sendf2).      
+00002090: 2020 7365 6c66 2e46 332e 7365 7443 6f6e    self.F3.setCon
+000020a0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+000020b0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+000020c0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+000020d0: 2020 2020 7365 6c66 2e46 332e 6375 7374      self.F3.cust
+000020e0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+000020f0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002100: 656c 662e 6564 6974 5f46 3329 0a20 2020  elf.edit_F3).   
+00002110: 2020 2020 2073 656c 662e 4633 2e63 6c69       self.F3.cli
+00002120: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002130: 662e 7365 6e64 6633 290a 2020 2020 2020  f.sendf3).      
+00002140: 2020 7365 6c66 2e46 342e 7365 7443 6f6e    self.F4.setCon
+00002150: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002160: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002170: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002180: 2020 2020 7365 6c66 2e46 342e 6375 7374      self.F4.cust
+00002190: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+000021a0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+000021b0: 656c 662e 6564 6974 5f46 3429 0a20 2020  elf.edit_F4).   
+000021c0: 2020 2020 2073 656c 662e 4634 2e63 6c69       self.F4.cli
+000021d0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+000021e0: 662e 7365 6e64 6634 290a 2020 2020 2020  f.sendf4).      
+000021f0: 2020 7365 6c66 2e46 352e 7365 7443 6f6e    self.F5.setCon
+00002200: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002210: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002220: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002230: 2020 2020 7365 6c66 2e46 352e 6375 7374      self.F5.cust
+00002240: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002250: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002260: 656c 662e 6564 6974 5f46 3529 0a20 2020  elf.edit_F5).   
+00002270: 2020 2020 2073 656c 662e 4635 2e63 6c69       self.F5.cli
+00002280: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002290: 662e 7365 6e64 6635 290a 2020 2020 2020  f.sendf5).      
+000022a0: 2020 7365 6c66 2e46 362e 7365 7443 6f6e    self.F6.setCon
+000022b0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+000022c0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+000022d0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+000022e0: 2020 2020 7365 6c66 2e46 362e 6375 7374      self.F6.cust
+000022f0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002300: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002310: 656c 662e 6564 6974 5f46 3629 0a20 2020  elf.edit_F6).   
+00002320: 2020 2020 2073 656c 662e 4636 2e63 6c69       self.F6.cli
+00002330: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002340: 662e 7365 6e64 6636 290a 2020 2020 2020  f.sendf6).      
+00002350: 2020 7365 6c66 2e46 372e 7365 7443 6f6e    self.F7.setCon
+00002360: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002370: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002380: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002390: 2020 2020 7365 6c66 2e46 372e 6375 7374      self.F7.cust
+000023a0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+000023b0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+000023c0: 656c 662e 6564 6974 5f46 3729 0a20 2020  elf.edit_F7).   
+000023d0: 2020 2020 2073 656c 662e 4637 2e63 6c69       self.F7.cli
+000023e0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+000023f0: 662e 7365 6e64 6637 290a 2020 2020 2020  f.sendf7).      
+00002400: 2020 7365 6c66 2e46 382e 7365 7443 6f6e    self.F8.setCon
+00002410: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002420: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002430: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002440: 2020 2020 7365 6c66 2e46 382e 6375 7374      self.F8.cust
+00002450: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002460: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002470: 656c 662e 6564 6974 5f46 3829 0a20 2020  elf.edit_F8).   
+00002480: 2020 2020 2073 656c 662e 4638 2e63 6c69       self.F8.cli
+00002490: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+000024a0: 662e 7365 6e64 6638 290a 2020 2020 2020  f.sendf8).      
+000024b0: 2020 7365 6c66 2e46 392e 7365 7443 6f6e    self.F9.setCon
+000024c0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+000024d0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+000024e0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+000024f0: 2020 2020 7365 6c66 2e46 392e 6375 7374      self.F9.cust
+00002500: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
+00002510: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
+00002520: 656c 662e 6564 6974 5f46 3929 0a20 2020  elf.edit_F9).   
+00002530: 2020 2020 2073 656c 662e 4639 2e63 6c69       self.F9.cli
+00002540: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002550: 662e 7365 6e64 6639 290a 2020 2020 2020  f.sendf9).      
+00002560: 2020 7365 6c66 2e46 3130 2e73 6574 436f    self.F10.setCo
+00002570: 6e74 6578 744d 656e 7550 6f6c 6963 7928  ntextMenuPolicy(
+00002580: 5174 436f 7265 2e51 742e 4375 7374 6f6d  QtCore.Qt.Custom
+00002590: 436f 6e74 6578 744d 656e 7529 0a20 2020  ContextMenu).   
+000025a0: 2020 2020 2073 656c 662e 4631 302e 6375       self.F10.cu
+000025b0: 7374 6f6d 436f 6e74 6578 744d 656e 7552  stomContextMenuR
+000025c0: 6571 7565 7374 6564 2e63 6f6e 6e65 6374  equested.connect
+000025d0: 2873 656c 662e 6564 6974 5f46 3130 290a  (self.edit_F10).
+000025e0: 2020 2020 2020 2020 7365 6c66 2e46 3130          self.F10
+000025f0: 2e63 6c69 636b 6564 2e63 6f6e 6e65 6374  .clicked.connect
+00002600: 2873 656c 662e 7365 6e64 6631 3029 0a20  (self.sendf10). 
+00002610: 2020 2020 2020 2073 656c 662e 4631 312e         self.F11.
+00002620: 7365 7443 6f6e 7465 7874 4d65 6e75 506f  setContextMenuPo
+00002630: 6c69 6379 2851 7443 6f72 652e 5174 2e43  licy(QtCore.Qt.C
+00002640: 7573 746f 6d43 6f6e 7465 7874 4d65 6e75  ustomContextMenu
+00002650: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
+00002660: 3131 2e63 7573 746f 6d43 6f6e 7465 7874  11.customContext
+00002670: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+00002680: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+00002690: 4631 3129 0a20 2020 2020 2020 2073 656c  F11).        sel
+000026a0: 662e 4631 312e 636c 6963 6b65 642e 636f  f.F11.clicked.co
+000026b0: 6e6e 6563 7428 7365 6c66 2e73 656e 6466  nnect(self.sendf
+000026c0: 3131 290a 2020 2020 2020 2020 7365 6c66  11).        self
+000026d0: 2e46 3132 2e73 6574 436f 6e74 6578 744d  .F12.setContextM
+000026e0: 656e 7550 6f6c 6963 7928 5174 436f 7265  enuPolicy(QtCore
+000026f0: 2e51 742e 4375 7374 6f6d 436f 6e74 6578  .Qt.CustomContex
+00002700: 744d 656e 7529 0a20 2020 2020 2020 2073  tMenu).        s
+00002710: 656c 662e 4631 322e 6375 7374 6f6d 436f  elf.F12.customCo
+00002720: 6e74 6578 744d 656e 7552 6571 7565 7374  ntextMenuRequest
+00002730: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+00002740: 6564 6974 5f46 3132 290a 2020 2020 2020  edit_F12).      
+00002750: 2020 7365 6c66 2e46 3132 2e63 6c69 636b    self.F12.click
+00002760: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+00002770: 7365 6e64 6631 3229 0a0a 2020 2020 2020  sendf12)..      
+00002780: 2020 7365 6c66 2e72 6561 6470 7265 6665    self.readprefe
+00002790: 7265 6e63 6573 2829 0a20 2020 2020 2020  rences().       
+000027a0: 2073 656c 662e 6462 6e61 6d65 203d 2044   self.dbname = D
+000027b0: 4154 415f 5041 5448 202b 2022 2f22 202b  ATA_PATH + "/" +
+000027c0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+000027d0: 6375 7272 656e 745f 6461 7461 6261 7365  current_database
+000027e0: 222c 2022 6861 6d2e 6462 2229 0a20 2020  ", "ham.db").   
+000027f0: 2020 2020 2073 656c 662e 6461 7461 6261       self.databa
+00002800: 7365 203d 2044 6174 6142 6173 6528 7365  se = DataBase(se
+00002810: 6c66 2e64 626e 616d 652c 2057 4f52 4b49  lf.dbname, WORKI
+00002820: 4e47 5f50 4154 4829 0a20 2020 2020 2020  NG_PATH).       
+00002830: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
+00002840: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
+00002850: 7463 685f 7374 6174 696f 6e28 290a 2020  tch_station().  
+00002860: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+00002870: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
+00002880: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002890: 7374 6174 696f 6e20 3d20 7b7d 0a20 2020  station = {}.   
+000028a0: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
+000028b0: 6974 5f73 7461 7469 6f6e 5f73 6574 7469  it_station_setti
+000028c0: 6e67 7328 290a 2020 2020 2020 2020 2020  ngs().          
+000028d0: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
+000028e0: 2073 656c 662e 6461 7461 6261 7365 2e66   self.database.f
+000028f0: 6574 6368 5f73 7461 7469 6f6e 2829 0a20  etch_station(). 
+00002900: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00002910: 6c66 2e73 7461 7469 6f6e 2069 7320 4e6f  lf.station is No
+00002920: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00002930: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+00002940: 203d 207b 7d0a 2020 2020 2020 2020 7365   = {}.        se
+00002950: 6c66 2e63 6f6e 7461 6374 203d 2073 656c  lf.contact = sel
+00002960: 662e 6461 7461 6261 7365 2e65 6d70 7479  f.database.empty
+00002970: 5f63 6f6e 7461 6374 0a20 2020 2020 2020  _contact.       
+00002980: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
+00002990: 203d 2073 656c 662e 7374 6174 696f 6e2e   = self.station.
+000029a0: 6765 7428 2243 616c 6c22 2c20 2222 290a  get("Call", "").
+000029b0: 2020 2020 2020 2020 7365 6c66 2e6d 616b          self.mak
+000029c0: 655f 6f70 5f64 6972 2829 0a20 2020 2020  e_op_dir().     
+000029d0: 2020 2073 656c 662e 7265 6164 5f63 775f     self.read_cw_
+000029e0: 6d61 6372 6f73 2829 0a20 2020 2020 2020  macros().       
+000029f0: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
+00002a00: 7328 290a 0a20 2020 2020 2020 2073 656c  s()..        sel
+00002a10: 662e 6261 6e64 5f69 6e64 6963 6174 6f72  f.band_indicator
+00002a20: 735f 6377 203d 207b 0a20 2020 2020 2020  s_cw = {.       
+00002a30: 2020 2020 2022 3136 3022 3a20 7365 6c66       "160": self
+00002a40: 2e63 775f 6261 6e64 5f31 3630 2c0a 2020  .cw_band_160,.  
+00002a50: 2020 2020 2020 2020 2020 2238 3022 3a20            "80": 
+00002a60: 7365 6c66 2e63 775f 6261 6e64 5f38 302c  self.cw_band_80,
+00002a70: 0a20 2020 2020 2020 2020 2020 2022 3430  .            "40
+00002a80: 223a 2073 656c 662e 6377 5f62 616e 645f  ": self.cw_band_
+00002a90: 3430 2c0a 2020 2020 2020 2020 2020 2020  40,.            
+00002aa0: 2232 3022 3a20 7365 6c66 2e63 775f 6261  "20": self.cw_ba
+00002ab0: 6e64 5f32 302c 0a20 2020 2020 2020 2020  nd_20,.         
+00002ac0: 2020 2022 3135 223a 2073 656c 662e 6377     "15": self.cw
+00002ad0: 5f62 616e 645f 3135 2c0a 2020 2020 2020  _band_15,.      
+00002ae0: 2020 2020 2020 2231 3022 3a20 7365 6c66        "10": self
+00002af0: 2e63 775f 6261 6e64 5f31 302c 0a20 2020  .cw_band_10,.   
+00002b00: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00002b10: 7365 6c66 2e62 616e 645f 696e 6469 6361  self.band_indica
+00002b20: 746f 7273 5f73 7362 203d 207b 0a20 2020  tors_ssb = {.   
+00002b30: 2020 2020 2020 2020 2022 3136 3022 3a20           "160": 
+00002b40: 7365 6c66 2e73 7362 5f62 616e 645f 3136  self.ssb_band_16
+00002b50: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+00002b60: 3830 223a 2073 656c 662e 7373 625f 6261  80": self.ssb_ba
+00002b70: 6e64 5f38 302c 0a20 2020 2020 2020 2020  nd_80,.         
+00002b80: 2020 2022 3430 223a 2073 656c 662e 7373     "40": self.ss
+00002b90: 625f 6261 6e64 5f34 302c 0a20 2020 2020  b_band_40,.     
+00002ba0: 2020 2020 2020 2022 3230 223a 2073 656c         "20": sel
+00002bb0: 662e 7373 625f 6261 6e64 5f32 302c 0a20  f.ssb_band_20,. 
+00002bc0: 2020 2020 2020 2020 2020 2022 3135 223a             "15":
+00002bd0: 2073 656c 662e 7373 625f 6261 6e64 5f31   self.ssb_band_1
+00002be0: 352c 0a20 2020 2020 2020 2020 2020 2022  5,.            "
+00002bf0: 3130 223a 2073 656c 662e 7373 625f 6261  10": self.ssb_ba
+00002c00: 6e64 5f31 302c 0a20 2020 2020 2020 207d  nd_10,.        }
+00002c10: 0a0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
+00002c20: 616e 645f 696e 6469 6361 746f 7273 5f72  and_indicators_r
+00002c30: 7474 7920 3d20 7b0a 2020 2020 2020 2020  tty = {.        
+00002c40: 2020 2020 2231 3630 223a 2073 656c 662e      "160": self.
+00002c50: 7274 7479 5f62 616e 645f 3136 302c 0a20  rtty_band_160,. 
+00002c60: 2020 2020 2020 2020 2020 2022 3830 223a             "80":
+00002c70: 2073 656c 662e 7274 7479 5f62 616e 645f   self.rtty_band_
+00002c80: 3830 2c0a 2020 2020 2020 2020 2020 2020  80,.            
+00002c90: 2234 3022 3a20 7365 6c66 2e72 7474 795f  "40": self.rtty_
+00002ca0: 6261 6e64 5f34 302c 0a20 2020 2020 2020  band_40,.       
+00002cb0: 2020 2020 2022 3230 223a 2073 656c 662e       "20": self.
+00002cc0: 7274 7479 5f62 616e 645f 3230 2c0a 2020  rtty_band_20,.  
+00002cd0: 2020 2020 2020 2020 2020 2231 3522 3a20            "15": 
+00002ce0: 7365 6c66 2e72 7474 795f 6261 6e64 5f31  self.rtty_band_1
+00002cf0: 352c 0a20 2020 2020 2020 2020 2020 2022  5,.            "
+00002d00: 3130 223a 2073 656c 662e 7274 7479 5f62  10": self.rtty_b
+00002d10: 616e 645f 3130 2c0a 2020 2020 2020 2020  and_10,.        
+00002d20: 7d0a 0a20 2020 2020 2020 2073 656c 662e  }..        self.
+00002d30: 616c 6c5f 6d6f 6465 5f69 6e64 6963 6174  all_mode_indicat
+00002d40: 6f72 7320 3d20 7b0a 2020 2020 2020 2020  ors = {.        
+00002d50: 2020 2020 2243 5722 3a20 7365 6c66 2e62      "CW": self.b
+00002d60: 616e 645f 696e 6469 6361 746f 7273 5f63  and_indicators_c
+00002d70: 772c 0a20 2020 2020 2020 2020 2020 2022  w,.            "
+00002d80: 5353 4222 3a20 7365 6c66 2e62 616e 645f  SSB": self.band_
+00002d90: 696e 6469 6361 746f 7273 5f73 7362 2c0a  indicators_ssb,.
+00002da0: 2020 2020 2020 2020 2020 2020 2252 5454              "RTT
+00002db0: 5922 3a20 7365 6c66 2e62 616e 645f 696e  Y": self.band_in
+00002dc0: 6469 6361 746f 7273 5f72 7474 792c 0a20  dicators_rtty,. 
+00002dd0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+00002de0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+00002df0: 6574 2822 636f 6e74 6573 7422 293a 0a20  et("contest"):. 
+00002e00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002e10: 6c6f 6164 5f63 6f6e 7465 7374 2829 0a0a  load_contest()..
+00002e20: 2020 2020 2020 2020 6966 2056 6572 7369          if Versi
+00002e30: 6f6e 5465 7374 285f 5f76 6572 7369 6f6e  onTest(__version
+00002e40: 5f5f 292e 7465 7374 2829 3a0a 2020 2020  __).test():.    
+00002e50: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
+00002e60: 775f 6d65 7373 6167 655f 626f 7828 0a20  w_message_box(. 
+00002e70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002e80: 5468 6572 6520 6973 2061 206e 6577 6572  There is a newer
+00002e90: 2076 6572 7369 6f6e 206f 6620 6e6f 7431   version of not1
+00002ea0: 6d6d 2061 7661 696c 6162 6c65 2e5c 6e22  mm available.\n"
+00002eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ec0: 2022 596f 7520 6361 6e20 7564 6174 6520   "You can udate 
+00002ed0: 746f 2074 6865 2063 7572 7265 6e74 2076  to the current v
+00002ee0: 6572 7369 6f6e 2062 7920 7573 696e 673a  ersion by using:
+00002ef0: 5c6e 7069 7020 696e 7374 616c 6c20 2d55  \npip install -U
+00002f00: 206e 6f74 316d 6d22 0a20 2020 2020 2020   not1mm".       
+00002f10: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00002f20: 7365 6c66 2e63 6865 636b 5f66 6f72 5f6e  self.check_for_n
+00002f30: 6577 5f63 7479 2829 0a0a 2020 2020 4073  ew_cty()..    @s
+00002f40: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00002f50: 6465 6620 6368 6563 6b5f 7072 6f63 6573  def check_proces
+00002f60: 7328 6e61 6d65 3a20 7374 7229 202d 3e20  s(name: str) -> 
+00002f70: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+00002f80: 2263 6865 636b 7320 746f 2073 6565 2069  "checks to see i
+00002f90: 6620 7072 6f67 7261 6d20 6f66 206e 616d  f program of nam
+00002fa0: 6520 6973 2069 6e20 7468 6520 6163 7469  e is in the acti
+00002fb0: 7665 2070 726f 6365 7373 206c 6973 7422  ve process list"
+00002fc0: 2222 0a20 2020 2020 2020 2066 6f72 2070  "".        for p
+00002fd0: 726f 6320 696e 2070 7375 7469 6c2e 7072  roc in psutil.pr
+00002fe0: 6f63 6573 735f 6974 6572 2829 3a0a 2020  ocess_iter():.  
+00002ff0: 2020 2020 2020 2020 2020 6966 2062 6f6f            if boo
+00003000: 6c28 7265 2e6d 6174 6368 286e 616d 652c  l(re.match(name,
+00003010: 2070 726f 632e 6e61 6d65 2829 2e6c 6f77   proc.name().low
+00003020: 6572 2829 2929 3a0a 2020 2020 2020 2020  er())):.        
+00003030: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00003040: 7275 650a 2020 2020 2020 2020 7265 7475  rue.        retu
+00003050: 726e 2046 616c 7365 0a0a 2020 2020 6465  rn False..    de
+00003060: 6620 7368 6f77 5f6d 6573 7361 6765 5f62  f show_message_b
+00003070: 6f78 2873 656c 662c 206d 6573 7361 6765  ox(self, message
+00003080: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
+00003090: 2020 2020 2020 2020 2222 2264 6f63 2222          """doc""
+000030a0: 220a 2020 2020 2020 2020 6d65 7373 6167  ".        messag
+000030b0: 655f 626f 7820 3d20 5174 5769 6467 6574  e_box = QtWidget
+000030c0: 732e 514d 6573 7361 6765 426f 7828 290a  s.QMessageBox().
+000030d0: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
+000030e0: 626f 782e 7365 7449 636f 6e28 5174 5769  box.setIcon(QtWi
+000030f0: 6467 6574 732e 514d 6573 7361 6765 426f  dgets.QMessageBo
+00003100: 782e 496e 666f 726d 6174 696f 6e29 0a20  x.Information). 
+00003110: 2020 2020 2020 206d 6573 7361 6765 5f62         message_b
+00003120: 6f78 2e73 6574 5465 7874 286d 6573 7361  ox.setText(messa
+00003130: 6765 290a 2020 2020 2020 2020 6d65 7373  ge).        mess
+00003140: 6167 655f 626f 782e 7365 7457 696e 646f  age_box.setWindo
+00003150: 7754 6974 6c65 2822 496e 666f 726d 6174  wTitle("Informat
+00003160: 696f 6e22 290a 2020 2020 2020 2020 6d65  ion").        me
+00003170: 7373 6167 655f 626f 782e 7365 7453 7461  ssage_box.setSta
+00003180: 6e64 6172 6442 7574 746f 6e73 2851 7457  ndardButtons(QtW
+00003190: 6964 6765 7473 2e51 4d65 7373 6167 6542  idgets.QMessageB
+000031a0: 6f78 2e4f 6b29 0a20 2020 2020 2020 205f  ox.Ok).        _
+000031b0: 203d 206d 6573 7361 6765 5f62 6f78 2e65   = message_box.e
+000031c0: 7865 635f 2829 0a0a 2020 2020 6465 6620  xec_()..    def 
+000031d0: 7368 6f77 5f61 626f 7574 5f64 6961 6c6f  show_about_dialo
+000031e0: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+000031f0: 2022 2222 5368 6f77 2061 626f 7574 2064   """Show about d
+00003200: 6961 6c6f 6722 2222 0a20 2020 2020 2020  ialog""".       
+00003210: 2073 656c 662e 6162 6f75 745f 6469 616c   self.about_dial
+00003220: 6f67 203d 2041 626f 7574 2857 4f52 4b49  og = About(WORKI
+00003230: 4e47 5f50 4154 4829 0a20 2020 2020 2020  NG_PATH).       
+00003240: 2073 656c 662e 6162 6f75 745f 6469 616c   self.about_dial
+00003250: 6f67 2e64 6f6e 6f72 732e 7365 7453 6f75  og.donors.setSou
+00003260: 7263 6528 0a20 2020 2020 2020 2020 2020  rce(.           
+00003270: 2051 7443 6f72 652e 5155 726c 2e66 726f   QtCore.QUrl.fro
+00003280: 6d4c 6f63 616c 4669 6c65 2857 4f52 4b49  mLocalFile(WORKI
+00003290: 4e47 5f50 4154 4820 2b20 222f 6461 7461  NG_PATH + "/data
+000032a0: 2f64 6f6e 6f72 732e 6874 6d6c 2229 0a20  /donors.html"). 
+000032b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000032c0: 2073 656c 662e 6162 6f75 745f 6469 616c   self.about_dial
+000032d0: 6f67 2e6f 7065 6e28 290a 0a20 2020 2064  og.open()..    d
+000032e0: 6566 2065 6469 745f 636f 6e66 6967 7572  ef edit_configur
+000032f0: 6174 696f 6e5f 7365 7474 696e 6773 2873  ation_settings(s
+00003300: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00003310: 2243 6f6e 6669 6775 7261 7469 6f6e 2053  "Configuration S
+00003320: 6574 7469 6e67 7320 7761 7320 636c 6963  ettings was clic
+00003330: 6b65 6422 2222 0a20 2020 2020 2020 2073  ked""".        s
+00003340: 656c 662e 636f 6e66 6967 7572 6174 696f  elf.configuratio
+00003350: 6e5f 6469 616c 6f67 203d 2053 6574 7469  n_dialog = Setti
+00003360: 6e67 7328 574f 524b 494e 475f 5041 5448  ngs(WORKING_PATH
+00003370: 2c20 434f 4e46 4947 5f50 4154 482c 2073  , CONFIG_PATH, s
+00003380: 656c 662e 7072 6566 290a 2020 2020 2020  elf.pref).      
+00003390: 2020 7365 6c66 2e63 6f6e 6669 6775 7261    self.configura
+000033a0: 7469 6f6e 5f64 6961 6c6f 672e 7573 6568  tion_dialog.useh
+000033b0: 616d 6462 5f72 6164 696f 4275 7474 6f6e  amdb_radioButton
+000033c0: 2e68 6964 6528 290a 2020 2020 2020 2020  .hide().        
+000033d0: 7365 6c66 2e63 6f6e 6669 6775 7261 7469  self.configurati
+000033e0: 6f6e 5f64 6961 6c6f 672e 7368 6f77 2829  on_dialog.show()
+000033f0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00003400: 6e66 6967 7572 6174 696f 6e5f 6469 616c  nfiguration_dial
+00003410: 6f67 2e61 6363 6570 7465 642e 636f 6e6e  og.accepted.conn
+00003420: 6563 7428 7365 6c66 2e65 6469 745f 636f  ect(self.edit_co
+00003430: 6e66 6967 7572 6174 696f 6e5f 7265 7475  nfiguration_retu
+00003440: 726e 290a 0a20 2020 2064 6566 2065 6469  rn)..    def edi
+00003450: 745f 636f 6e66 6967 7572 6174 696f 6e5f  t_configuration_
+00003460: 7265 7475 726e 2873 656c 6629 3a0a 2020  return(self):.  
+00003470: 2020 2020 2020 2222 2252 6574 7572 6e73        """Returns
+00003480: 2068 6572 6520 7768 656e 2063 6f6e 6669   here when confi
+00003490: 6775 7261 7469 6f6e 2064 6961 6c6f 6720  guration dialog 
+000034a0: 636c 6f73 6564 2077 6974 6820 6f6b 6179  closed with okay
+000034b0: 2e22 2222 0a20 2020 2020 2020 2073 656c  .""".        sel
+000034c0: 662e 636f 6e66 6967 7572 6174 696f 6e5f  f.configuration_
+000034d0: 6469 616c 6f67 2e73 6176 655f 6368 616e  dialog.save_chan
+000034e0: 6765 7328 290a 2020 2020 2020 2020 7365  ges().        se
+000034f0: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
+00003500: 6e63 6528 290a 2020 2020 2020 2020 6c6f  nce().        lo
+00003510: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
+00003520: 2066 227b 7365 6c66 2e70 7265 667d 2229   f"{self.pref}")
+00003530: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00003540: 6164 7072 6566 6572 656e 6365 7328 290a  adpreferences().
+00003550: 0a20 2020 2064 6566 206e 6577 5f64 6174  .    def new_dat
+00003560: 6162 6173 6528 7365 6c66 293a 0a20 2020  abase(self):.   
+00003570: 2020 2020 2022 2222 4372 6561 7465 206e       """Create n
+00003580: 6577 2064 6174 6162 6173 652e 2222 220a  ew database.""".
+00003590: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+000035a0: 203d 2073 656c 662e 6669 6c65 7069 636b   = self.filepick
+000035b0: 6572 2822 6e65 7722 290a 2020 2020 2020  er("new").      
+000035c0: 2020 6966 2066 696c 656e 616d 653a 0a20    if filename:. 
+000035d0: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
+000035e0: 6c65 6e61 6d65 5b2d 333a 5d20 213d 2022  lename[-3:] != "
+000035f0: 2e64 6222 3a0a 2020 2020 2020 2020 2020  .db":.          
+00003600: 2020 2020 2020 6669 6c65 6e61 6d65 202b        filename +
+00003610: 3d20 222e 6462 220a 2020 2020 2020 2020  = ".db".        
+00003620: 2020 2020 7365 6c66 2e70 7265 665b 2263      self.pref["c
+00003630: 7572 7265 6e74 5f64 6174 6162 6173 6522  urrent_database"
+00003640: 5d20 3d20 6669 6c65 6e61 6d65 2e73 706c  ] = filename.spl
+00003650: 6974 2822 2f22 295b 2d31 3a5d 5b30 5d0a  it("/")[-1:][0].
+00003660: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003670: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
+00003680: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00003690: 7365 6c66 2e64 626e 616d 6520 3d20 4441  self.dbname = DA
+000036a0: 5441 5f50 4154 4820 2b20 222f 2220 2b20  TA_PATH + "/" + 
+000036b0: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
+000036c0: 7572 7265 6e74 5f64 6174 6162 6173 6522  urrent_database"
+000036d0: 2c20 2268 616d 2e64 6222 290a 2020 2020  , "ham.db").    
+000036e0: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+000036f0: 6162 6173 6520 3d20 4461 7461 4261 7365  abase = DataBase
+00003700: 2873 656c 662e 6462 6e61 6d65 2c20 574f  (self.dbname, WO
+00003710: 524b 494e 475f 5041 5448 290a 2020 2020  RKING_PATH).    
+00003720: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00003730: 7461 6374 203d 2073 656c 662e 6461 7461  tact = self.data
+00003740: 6261 7365 2e65 6d70 7479 5f63 6f6e 7461  base.empty_conta
+00003750: 6374 0a20 2020 2020 2020 2020 2020 2073  ct.            s
+00003760: 656c 662e 7374 6174 696f 6e20 3d20 7365  elf.station = se
+00003770: 6c66 2e64 6174 6162 6173 652e 6665 7463  lf.database.fetc
+00003780: 685f 7374 6174 696f 6e28 290a 2020 2020  h_station().    
+00003790: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000037a0: 7374 6174 696f 6e20 6973 204e 6f6e 653a  station is None:
+000037b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000037c0: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
+000037d0: 7b7d 0a20 2020 2020 2020 2020 2020 2073  {}.            s
+000037e0: 656c 662e 6375 7272 656e 745f 6f70 203d  elf.current_op =
+000037f0: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
+00003800: 7428 2243 616c 6c22 2c20 2222 290a 2020  t("Call", "").  
+00003810: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00003820: 616b 655f 6f70 5f64 6972 2829 0a20 2020  ake_op_dir().   
+00003830: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+00003840: 7d0a 2020 2020 2020 2020 2020 2020 636d  }.            cm
+00003850: 645b 2263 6d64 225d 203d 2022 4e45 5744  d["cmd"] = "NEWD
+00003860: 4222 0a20 2020 2020 2020 2020 2020 2063  B".            c
+00003870: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
+00003880: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+00003890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000038a0: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
+000038b0: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
+000038c0: 6e28 636d 6429 0a20 2020 2020 2020 2020  n(cmd).         
+000038d0: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
+000038e0: 7574 7328 290a 2020 2020 2020 2020 2020  uts().          
+000038f0: 2020 7365 6c66 2e65 6469 745f 7374 6174    self.edit_stat
+00003900: 696f 6e5f 7365 7474 696e 6773 2829 0a0a  ion_settings()..
+00003910: 2020 2020 6465 6620 6f70 656e 5f64 6174      def open_dat
+00003920: 6162 6173 6528 7365 6c66 293a 0a20 2020  abase(self):.   
+00003930: 2020 2020 2022 2222 4f70 656e 2065 7869       """Open exi
+00003940: 7374 696e 6720 6461 7461 6261 7365 2e22  sting database."
+00003950: 2222 0a20 2020 2020 2020 2066 696c 656e  "".        filen
+00003960: 616d 6520 3d20 7365 6c66 2e66 696c 6570  ame = self.filep
+00003970: 6963 6b65 7228 226f 7065 6e22 290a 2020  icker("open").  
+00003980: 2020 2020 2020 6966 2066 696c 656e 616d        if filenam
+00003990: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000039a0: 656c 662e 7072 6566 5b22 6375 7272 656e  elf.pref["curren
+000039b0: 745f 6461 7461 6261 7365 225d 203d 2066  t_database"] = f
+000039c0: 696c 656e 616d 652e 7370 6c69 7428 222f  ilename.split("/
+000039d0: 2229 5b2d 313a 5d5b 305d 0a20 2020 2020  ")[-1:][0].     
+000039e0: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
+000039f0: 655f 7072 6566 6572 656e 6365 2829 0a20  e_preference(). 
+00003a00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003a10: 6462 6e61 6d65 203d 2044 4154 415f 5041  dbname = DATA_PA
+00003a20: 5448 202b 2022 2f22 202b 2073 656c 662e  TH + "/" + self.
+00003a30: 7072 6566 2e67 6574 2822 6375 7272 656e  pref.get("curren
+00003a40: 745f 6461 7461 6261 7365 222c 2022 6861  t_database", "ha
+00003a50: 6d2e 6462 2229 0a20 2020 2020 2020 2020  m.db").         
+00003a60: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
+00003a70: 203d 2044 6174 6142 6173 6528 7365 6c66   = DataBase(self
+00003a80: 2e64 626e 616d 652c 2057 4f52 4b49 4e47  .dbname, WORKING
+00003a90: 5f50 4154 4829 0a20 2020 2020 2020 2020  _PATH).         
+00003aa0: 2020 2073 656c 662e 636f 6e74 6163 7420     self.contact 
+00003ab0: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
+00003ac0: 656d 7074 795f 636f 6e74 6163 740a 2020  empty_contact.  
+00003ad0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00003ae0: 7461 7469 6f6e 203d 2073 656c 662e 6461  tation = self.da
+00003af0: 7461 6261 7365 2e66 6574 6368 5f73 7461  tabase.fetch_sta
+00003b00: 7469 6f6e 2829 0a20 2020 2020 2020 2020  tion().         
+00003b10: 2020 2069 6620 7365 6c66 2e73 7461 7469     if self.stati
+00003b20: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00003b30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003b40: 2e73 7461 7469 6f6e 203d 207b 7d0a 2020  .station = {}.  
+00003b50: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00003b60: 662e 7374 6174 696f 6e2e 6765 7428 2243  f.station.get("C
+00003b70: 616c 6c22 2c20 2222 2920 3d3d 2022 223a  all", "") == "":
+00003b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b90: 2073 656c 662e 6564 6974 5f73 7461 7469   self.edit_stati
+00003ba0: 6f6e 5f73 6574 7469 6e67 7328 290a 2020  on_settings().  
+00003bb0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00003bc0: 7572 7265 6e74 5f6f 7020 3d20 7365 6c66  urrent_op = self
+00003bd0: 2e73 7461 7469 6f6e 2e67 6574 2822 4361  .station.get("Ca
+00003be0: 6c6c 222c 2022 2229 0a20 2020 2020 2020  ll", "").       
+00003bf0: 2020 2020 2073 656c 662e 6d61 6b65 5f6f       self.make_o
+00003c00: 705f 6469 7228 290a 2020 2020 2020 2020  p_dir().        
+00003c10: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
+00003c20: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
+00003c30: 6422 5d20 3d20 224e 4557 4442 220a 2020  d"] = "NEWDB".  
+00003c40: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
+00003c50: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+00003c60: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+00003c70: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
+00003c80: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+00003c90: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
+00003ca0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00003cb0: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
+00003cc0: 0a0a 2020 2020 6465 6620 6e65 775f 636f  ..    def new_co
+00003cd0: 6e74 6573 7428 7365 6c66 293a 0a20 2020  ntest(self):.   
+00003ce0: 2020 2020 2022 2222 4372 6561 7465 206e       """Create n
+00003cf0: 6577 2063 6f6e 7465 7374 2069 6e20 6578  ew contest in ex
+00003d00: 6973 7469 6e67 2064 6174 6162 6173 652e  isting database.
+00003d10: 2222 220a 0a20 2020 2064 6566 206f 7065  """..    def ope
+00003d20: 6e5f 636f 6e74 6573 7428 7365 6c66 293a  n_contest(self):
+00003d30: 0a20 2020 2020 2020 2022 2222 5377 6974  .        """Swit
+00003d40: 6368 2074 6f20 6120 6469 6666 6572 656e  ch to a differen
+00003d50: 7420 6578 6973 7469 6e67 2063 6f6e 7465  t existing conte
+00003d60: 7374 2069 6e20 6578 6973 7469 6e67 2064  st in existing d
+00003d70: 6174 6162 6173 652e 2222 220a 2020 2020  atabase.""".    
+00003d80: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00003d90: 2822 4f70 656e 2043 6f6e 7465 7374 2073  ("Open Contest s
+00003da0: 656c 6563 7465 6422 290a 2020 2020 2020  elected").      
+00003db0: 2020 636f 6e74 6573 7473 203d 2073 656c    contests = sel
+00003dc0: 662e 6461 7461 6261 7365 2e66 6574 6368  f.database.fetch
+00003dd0: 5f61 6c6c 5f63 6f6e 7465 7374 7328 290a  _all_contests().
+00003de0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00003df0: 6562 7567 2822 2573 222c 2066 227b 636f  ebug("%s", f"{co
+00003e00: 6e74 6573 7473 7d22 290a 0a20 2020 2020  ntests}")..     
+00003e10: 2020 2069 6620 636f 6e74 6573 7473 3a0a     if contests:.
+00003e20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003e30: 2e63 6f6e 7465 7374 5f64 6961 6c6f 6720  .contest_dialog 
+00003e40: 3d20 5365 6c65 6374 436f 6e74 6573 7428  = SelectContest(
+00003e50: 574f 524b 494e 475f 5041 5448 290a 2020  WORKING_PATH).  
+00003e60: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00003e70: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
+00003e80: 6e74 6573 745f 6c69 7374 2e73 6574 526f  ntest_list.setRo
+00003e90: 7743 6f75 6e74 2830 290a 2020 2020 2020  wCount(0).      
+00003ea0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+00003eb0: 7374 5f64 6961 6c6f 672e 636f 6e74 6573  st_dialog.contes
+00003ec0: 745f 6c69 7374 2e73 6574 436f 6c75 6d6e  t_list.setColumn
+00003ed0: 436f 756e 7428 3429 0a20 2020 2020 2020  Count(4).       
+00003ee0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00003ef0: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
+00003f00: 5f6c 6973 742e 7665 7274 6963 616c 4865  _list.verticalHe
+00003f10: 6164 6572 2829 2e73 6574 5669 7369 626c  ader().setVisibl
+00003f20: 6528 4661 6c73 6529 0a20 2020 2020 2020  e(False).       
+00003f30: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00003f40: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
+00003f50: 5f6c 6973 742e 7365 7443 6f6c 756d 6e57  _list.setColumnW
+00003f60: 6964 7468 2831 2c20 3230 3029 0a20 2020  idth(1, 200).   
+00003f70: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00003f80: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+00003f90: 7465 7374 5f6c 6973 742e 7365 7443 6f6c  test_list.setCol
+00003fa0: 756d 6e57 6964 7468 2832 2c20 3230 3029  umnWidth(2, 200)
+00003fb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003fc0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00003fd0: 2e63 6f6e 7465 7374 5f6c 6973 742e 7365  .contest_list.se
+00003fe0: 7448 6f72 697a 6f6e 7461 6c48 6561 6465  tHorizontalHeade
+00003ff0: 7249 7465 6d28 0a20 2020 2020 2020 2020  rItem(.         
+00004000: 2020 2020 2020 2030 2c20 5174 5769 6467         0, QtWidg
+00004010: 6574 732e 5154 6162 6c65 5769 6467 6574  ets.QTableWidget
+00004020: 4974 656d 2822 436f 6e74 6573 7420 4e72  Item("Contest Nr
+00004030: 2229 0a20 2020 2020 2020 2020 2020 2029  ").            )
+00004040: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00004050: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004060: 2e63 6f6e 7465 7374 5f6c 6973 742e 7365  .contest_list.se
+00004070: 7448 6f72 697a 6f6e 7461 6c48 6561 6465  tHorizontalHeade
+00004080: 7249 7465 6d28 0a20 2020 2020 2020 2020  rItem(.         
+00004090: 2020 2020 2020 2031 2c20 5174 5769 6467         1, QtWidg
+000040a0: 6574 732e 5154 6162 6c65 5769 6467 6574  ets.QTableWidget
+000040b0: 4974 656d 2822 436f 6e74 6573 7420 4e61  Item("Contest Na
+000040c0: 6d65 2229 0a20 2020 2020 2020 2020 2020  me").           
+000040d0: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
+000040e0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+000040f0: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
+00004100: 7365 7448 6f72 697a 6f6e 7461 6c48 6561  setHorizontalHea
+00004110: 6465 7249 7465 6d28 0a20 2020 2020 2020  derItem(.       
+00004120: 2020 2020 2020 2020 2032 2c20 5174 5769           2, QtWi
+00004130: 6467 6574 732e 5154 6162 6c65 5769 6467  dgets.QTableWidg
+00004140: 6574 4974 656d 2822 436f 6e74 6573 7420  etItem("Contest 
+00004150: 5374 6172 7422 290a 2020 2020 2020 2020  Start").        
+00004160: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00004170: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+00004180: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
+00004190: 7374 2e73 6574 486f 7269 7a6f 6e74 616c  st.setHorizontal
+000041a0: 4865 6164 6572 4974 656d 280a 2020 2020  HeaderItem(.    
+000041b0: 2020 2020 2020 2020 2020 2020 332c 2051              3, Q
+000041c0: 7457 6964 6765 7473 2e51 5461 626c 6557  tWidgets.QTableW
+000041d0: 6964 6765 7449 7465 6d28 224e 6f74 2055  idgetItem("Not U
+000041e0: 4973 6564 2229 0a20 2020 2020 2020 2020  Ised").         
+000041f0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00004200: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00004210: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
+00004220: 742e 7365 7443 6f6c 756d 6e48 6964 6465  t.setColumnHidde
+00004230: 6e28 302c 2054 7275 6529 0a20 2020 2020  n(0, True).     
+00004240: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00004250: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+00004260: 7374 5f6c 6973 742e 7365 7443 6f6c 756d  st_list.setColum
+00004270: 6e48 6964 6465 6e28 332c 2054 7275 6529  nHidden(3, True)
+00004280: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00004290: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+000042a0: 2e61 6363 6570 7465 642e 636f 6e6e 6563  .accepted.connec
+000042b0: 7428 7365 6c66 2e6f 7065 6e5f 636f 6e74  t(self.open_cont
+000042c0: 6573 745f 7265 7475 726e 290a 2020 2020  est_return).    
+000042d0: 2020 2020 2020 2020 666f 7220 636f 6e74          for cont
+000042e0: 6573 7420 696e 2063 6f6e 7465 7374 733a  est in contests:
+000042f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004300: 206e 756d 6265 725f 6f66 5f72 6f77 7320   number_of_rows 
+00004310: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+00004320: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
+00004330: 7374 2e72 6f77 436f 756e 7428 290a 2020  st.rowCount().  
+00004340: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004350: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00004360: 672e 636f 6e74 6573 745f 6c69 7374 2e69  g.contest_list.i
+00004370: 6e73 6572 7452 6f77 286e 756d 6265 725f  nsertRow(number_
+00004380: 6f66 5f72 6f77 7329 0a20 2020 2020 2020  of_rows).       
+00004390: 2020 2020 2020 2020 2063 6f6e 7465 7374           contest
+000043a0: 5f69 6420 3d20 7374 7228 636f 6e74 6573  _id = str(contes
+000043b0: 742e 6765 7428 2243 6f6e 7465 7374 4944  t.get("ContestID
+000043c0: 222c 2031 2929 0a20 2020 2020 2020 2020  ", 1)).         
+000043d0: 2020 2020 2020 2063 6f6e 7465 7374 5f6e         contest_n
+000043e0: 616d 6520 3d20 636f 6e74 6573 742e 6765  ame = contest.ge
+000043f0: 7428 2243 6f6e 7465 7374 4e61 6d65 222c  t("ContestName",
+00004400: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
+00004410: 2020 2020 7374 6172 745f 6461 7465 203d      start_date =
+00004420: 2063 6f6e 7465 7374 2e67 6574 2822 5374   contest.get("St
+00004430: 6172 7444 6174 6522 2c20 3129 0a20 2020  artDate", 1).   
+00004440: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00004450: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004460: 2e63 6f6e 7465 7374 5f6c 6973 742e 7365  .contest_list.se
+00004470: 7449 7465 6d28 0a20 2020 2020 2020 2020  tItem(.         
+00004480: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
+00004490: 725f 6f66 5f72 6f77 732c 2030 2c20 5174  r_of_rows, 0, Qt
+000044a0: 5769 6467 6574 732e 5154 6162 6c65 5769  Widgets.QTableWi
+000044b0: 6467 6574 4974 656d 2863 6f6e 7465 7374  dgetItem(contest
+000044c0: 5f69 6429 0a20 2020 2020 2020 2020 2020  _id).           
+000044d0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000044e0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+000044f0: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+00004500: 7374 5f6c 6973 742e 7365 7449 7465 6d28  st_list.setItem(
+00004510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004520: 2020 2020 206e 756d 6265 725f 6f66 5f72       number_of_r
+00004530: 6f77 732c 2031 2c20 5174 5769 6467 6574  ows, 1, QtWidget
+00004540: 732e 5154 6162 6c65 5769 6467 6574 4974  s.QTableWidgetIt
+00004550: 656d 2863 6f6e 7465 7374 5f6e 616d 6529  em(contest_name)
+00004560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004570: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00004580: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00004590: 6469 616c 6f67 2e63 6f6e 7465 7374 5f6c  dialog.contest_l
+000045a0: 6973 742e 7365 7449 7465 6d28 0a20 2020  ist.setItem(.   
+000045b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045c0: 206e 756d 6265 725f 6f66 5f72 6f77 732c   number_of_rows,
+000045d0: 2032 2c20 5174 5769 6467 6574 732e 5154   2, QtWidgets.QT
+000045e0: 6162 6c65 5769 6467 6574 4974 656d 2873  ableWidgetItem(s
+000045f0: 7461 7274 5f64 6174 6529 0a20 2020 2020  tart_date).     
+00004600: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00004610: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00004620: 745f 6469 616c 6f67 2e73 686f 7728 290a  t_dialog.show().
+00004630: 0a20 2020 2064 6566 206f 7065 6e5f 636f  .    def open_co
+00004640: 6e74 6573 745f 7265 7475 726e 2873 656c  ntest_return(sel
+00004650: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
+00004660: 616c 6c65 6420 6279 206f 7065 6e5f 636f  alled by open_co
+00004670: 6e74 6573 7422 2222 0a20 2020 2020 2020  ntest""".       
+00004680: 2073 656c 6563 7465 645f 726f 7720 3d20   selected_row = 
+00004690: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+000046a0: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
+000046b0: 2e63 7572 7265 6e74 526f 7728 290a 2020  .currentRow().  
+000046c0: 2020 2020 2020 636f 6e74 6573 7420 3d20        contest = 
+000046d0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+000046e0: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
+000046f0: 2e69 7465 6d28 7365 6c65 6374 6564 5f72  .item(selected_r
+00004700: 6f77 2c20 3029 2e74 6578 7428 290a 2020  ow, 0).text().  
+00004710: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
+00004720: 2263 6f6e 7465 7374 225d 203d 2063 6f6e  "contest"] = con
+00004730: 7465 7374 0a20 2020 2020 2020 2073 656c  test.        sel
+00004740: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
+00004750: 6365 2829 0a20 2020 2020 2020 206c 6f67  ce().        log
+00004760: 6765 722e 6465 6275 6728 2253 656c 6563  ger.debug("Selec
+00004770: 7465 6420 636f 6e74 6573 743a 2025 7322  ted contest: %s"
+00004780: 2c20 6622 7b63 6f6e 7465 7374 7d22 290a  , f"{contest}").
+00004790: 2020 2020 2020 2020 7365 6c66 2e6c 6f61          self.loa
+000047a0: 645f 636f 6e74 6573 7428 290a 0a20 2020  d_contest()..   
+000047b0: 2064 6566 2072 6566 696c 6c5f 6472 6f70   def refill_drop
+000047c0: 646f 776e 2873 656c 662c 2074 6172 6765  down(self, targe
+000047d0: 742c 2073 6f75 7263 6529 3a0a 2020 2020  t, source):.    
+000047e0: 2020 2020 2222 2252 6566 696c 6c20 5143      """Refill QC
+000047f0: 6f6d 626f 626f 7820 7769 6467 6574 2077  ombobox widget w
+00004800: 6974 6820 7661 6c75 652e 2222 220a 2020  ith value.""".  
+00004810: 2020 2020 2020 696e 6465 7820 3d20 7461        index = ta
+00004820: 7267 6574 2e66 696e 6454 6578 7428 736f  rget.findText(so
+00004830: 7572 6365 290a 2020 2020 2020 2020 7461  urce).        ta
+00004840: 7267 6574 2e73 6574 4375 7272 656e 7449  rget.setCurrentI
+00004850: 6e64 6578 2869 6e64 6578 290a 0a20 2020  ndex(index)..   
+00004860: 2064 6566 2065 6469 745f 636f 6e74 6573   def edit_contes
+00004870: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00004880: 2022 2222 4564 6974 2074 6865 2063 7572   """Edit the cur
+00004890: 7265 6e74 2063 6f6e 7465 7374 2222 220a  rent contest""".
+000048a0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+000048b0: 6562 7567 2822 4564 6974 2063 6f6e 7465  ebug("Edit conte
+000048c0: 7374 2044 6961 6c6f 6722 290a 2020 2020  st Dialog").    
+000048d0: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
+000048e0: 6573 745f 7365 7474 696e 6773 2069 7320  est_settings is 
+000048f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00004900: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00004910: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00004920: 616c 6f67 203d 204e 6577 436f 6e74 6573  alog = NewContes
+00004930: 7428 574f 524b 494e 475f 5041 5448 290a  t(WORKING_PATH).
+00004940: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00004950: 7465 7374 5f64 6961 6c6f 672e 7365 7457  test_dialog.setW
+00004960: 696e 646f 7754 6974 6c65 2822 4564 6974  indowTitle("Edit
+00004970: 2043 6f6e 7465 7374 2229 0a20 2020 2020   Contest").     
+00004980: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00004990: 6469 616c 6f67 2e74 6974 6c65 2e73 6574  dialog.title.set
+000049a0: 5465 7874 2822 2229 0a20 2020 2020 2020  Text("").       
+000049b0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+000049c0: 616c 6f67 2e61 6363 6570 7465 642e 636f  alog.accepted.co
+000049d0: 6e6e 6563 7428 7365 6c66 2e73 6176 655f  nnect(self.save_
+000049e0: 6564 6974 6564 5f63 6f6e 7465 7374 290a  edited_contest).
+000049f0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00004a00: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00004a10: 7469 6e67 732e 6765 7428 2243 6f6e 7465  tings.get("Conte
+00004a20: 7374 4e61 6d65 2229 2e75 7070 6572 2829  stName").upper()
+00004a30: 2e72 6570 6c61 6365 2822 5f22 2c20 2220  .replace("_", " 
+00004a40: 2229 0a20 2020 2020 2020 2069 6620 7661  ").        if va
+00004a50: 6c75 6520 3d3d 2022 4745 4e45 5241 4c20  lue == "GENERAL 
+00004a60: 4c4f 4747 494e 4722 3a0a 2020 2020 2020  LOGGING":.      
+00004a70: 2020 2020 2020 7661 6c75 6520 3d20 2247        value = "G
+00004a80: 656e 6572 616c 204c 6f67 6769 6e67 220a  eneral Logging".
+00004a90: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+00004aa0: 696c 6c5f 6472 6f70 646f 776e 2873 656c  ill_dropdown(sel
+00004ab0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004ac0: 2e63 6f6e 7465 7374 2c20 7661 6c75 6529  .contest, value)
+00004ad0: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
+00004ae0: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
+00004af0: 7474 696e 6773 2e67 6574 2822 4f70 6572  ttings.get("Oper
+00004b00: 6174 6f72 4361 7465 676f 7279 2229 0a20  atorCategory"). 
+00004b10: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
+00004b20: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
+00004b30: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00004b40: 6f70 6572 6174 6f72 5f63 6c61 7373 2c20  operator_class, 
+00004b50: 7661 6c75 6529 0a20 2020 2020 2020 2076  value).        v
+00004b60: 616c 7565 203d 2073 656c 662e 636f 6e74  alue = self.cont
+00004b70: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
+00004b80: 2822 4261 6e64 4361 7465 676f 7279 2229  ("BandCategory")
+00004b90: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00004ba0: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
+00004bb0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00004bc0: 672e 6261 6e64 2c20 7661 6c75 6529 0a20  g.band, value). 
+00004bd0: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
+00004be0: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
+00004bf0: 696e 6773 2e67 6574 2822 506f 7765 7243  ings.get("PowerC
+00004c00: 6174 6567 6f72 7922 290a 2020 2020 2020  ategory").      
+00004c10: 2020 7365 6c66 2e72 6566 696c 6c5f 6472    self.refill_dr
+00004c20: 6f70 646f 776e 2873 656c 662e 636f 6e74  opdown(self.cont
+00004c30: 6573 745f 6469 616c 6f67 2e70 6f77 6572  est_dialog.power
+00004c40: 2c20 7661 6c75 6529 0a20 2020 2020 2020  , value).       
+00004c50: 2076 616c 7565 203d 2073 656c 662e 636f   value = self.co
+00004c60: 6e74 6573 745f 7365 7474 696e 6773 2e67  ntest_settings.g
+00004c70: 6574 2822 4d6f 6465 4361 7465 676f 7279  et("ModeCategory
+00004c80: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00004c90: 7265 6669 6c6c 5f64 726f 7064 6f77 6e28  refill_dropdown(
+00004ca0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00004cb0: 6c6f 672e 6d6f 6465 2c20 7661 6c75 6529  log.mode, value)
+00004cc0: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
+00004cd0: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
+00004ce0: 7474 696e 6773 2e67 6574 2822 4f76 6572  ttings.get("Over
+00004cf0: 6c61 7943 6174 6567 6f72 7922 290a 2020  layCategory").  
+00004d00: 2020 2020 2020 7365 6c66 2e72 6566 696c        self.refil
+00004d10: 6c5f 6472 6f70 646f 776e 2873 656c 662e  l_dropdown(self.
+00004d20: 636f 6e74 6573 745f 6469 616c 6f67 2e6f  contest_dialog.o
+00004d30: 7665 726c 6179 2c20 7661 6c75 6529 0a20  verlay, value). 
+00004d40: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00004d50: 6573 745f 6469 616c 6f67 2e6f 7065 7261  est_dialog.opera
+00004d60: 746f 7273 2e73 6574 5465 7874 2873 656c  tors.setText(sel
+00004d70: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
+00004d80: 6773 2e67 6574 2822 4f70 6572 6174 6f72  gs.get("Operator
+00004d90: 7322 2929 0a20 2020 2020 2020 2073 656c  s")).        sel
+00004da0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004db0: 2e73 6f61 7062 6f78 2e73 6574 506c 6169  .soapbox.setPlai
+00004dc0: 6e54 6578 7428 7365 6c66 2e63 6f6e 7465  nText(self.conte
+00004dd0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
+00004de0: 2253 6f61 7062 6f78 2229 290a 2020 2020  "Soapbox")).    
+00004df0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00004e00: 5f64 6961 6c6f 672e 6578 6368 616e 6765  _dialog.exchange
+00004e10: 2e73 6574 5465 7874 2873 656c 662e 636f  .setText(self.co
+00004e20: 6e74 6573 745f 7365 7474 696e 6773 2e67  ntest_settings.g
+00004e30: 6574 2822 5365 6e74 4578 6368 616e 6765  et("SentExchange
+00004e40: 2229 290a 2020 2020 2020 2020 7661 6c75  ")).        valu
+00004e50: 6520 3d20 7365 6c66 2e63 6f6e 7465 7374  e = self.contest
+00004e60: 5f73 6574 7469 6e67 732e 6765 7428 2253  _settings.get("S
+00004e70: 7461 7469 6f6e 4361 7465 676f 7279 2229  tationCategory")
+00004e80: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00004e90: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
+00004ea0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00004eb0: 672e 7374 6174 696f 6e2c 2076 616c 7565  g.station, value
+00004ec0: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
+00004ed0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
+00004ee0: 6574 7469 6e67 732e 6765 7428 2241 7373  ettings.get("Ass
+00004ef0: 6973 7465 6443 6174 6567 6f72 7922 290a  istedCategory").
+00004f00: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+00004f10: 696c 6c5f 6472 6f70 646f 776e 2873 656c  ill_dropdown(sel
+00004f20: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004f30: 2e61 7373 6973 7465 642c 2076 616c 7565  .assisted, value
+00004f40: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
+00004f50: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
+00004f60: 6574 7469 6e67 732e 6765 7428 2254 7261  ettings.get("Tra
+00004f70: 6e73 6d69 7474 6572 4361 7465 676f 7279  nsmitterCategory
+00004f80: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00004f90: 7265 6669 6c6c 5f64 726f 7064 6f77 6e28  refill_dropdown(
+00004fa0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00004fb0: 6c6f 672e 7472 616e 736d 6974 7465 722c  log.transmitter,
+00004fc0: 2076 616c 7565 290a 2020 2020 2020 2020   value).        
+00004fd0: 7661 6c75 6520 3d20 7365 6c66 2e63 6f6e  value = self.con
+00004fe0: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
+00004ff0: 7428 2253 7461 7274 4461 7465 2229 0a20  t("StartDate"). 
+00005000: 2020 2020 2020 2074 6865 5f64 6174 652c         the_date,
+00005010: 2074 6865 5f74 696d 6520 3d20 7661 6c75   the_time = valu
+00005020: 652e 7370 6c69 7428 290a 2020 2020 2020  e.split().      
+00005030: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+00005040: 6961 6c6f 672e 6461 7465 5469 6d65 4564  ialog.dateTimeEd
+00005050: 6974 2e73 6574 4461 7465 280a 2020 2020  it.setDate(.    
+00005060: 2020 2020 2020 2020 5174 436f 7265 2e51          QtCore.Q
+00005070: 4461 7465 2e66 726f 6d53 7472 696e 6728  Date.fromString(
+00005080: 7468 655f 6461 7465 2c20 2279 7979 792d  the_date, "yyyy-
+00005090: 4d4d 2d64 6422 290a 2020 2020 2020 2020  MM-dd").        
+000050a0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+000050b0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6461  ontest_dialog.da
+000050c0: 7465 5469 6d65 4564 6974 2e73 6574 4361  teTimeEdit.setCa
+000050d0: 6c65 6e64 6172 506f 7075 7028 5472 7565  lendarPopup(True
+000050e0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+000050f0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6461  ontest_dialog.da
+00005100: 7465 5469 6d65 4564 6974 2e73 6574 5469  teTimeEdit.setTi
+00005110: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
+00005120: 5174 436f 7265 2e51 5469 6d65 2e66 726f  QtCore.QTime.fro
+00005130: 6d53 7472 696e 6728 7468 655f 7469 6d65  mString(the_time
+00005140: 2c20 2268 683a 6d6d 3a73 7322 290a 2020  , "hh:mm:ss").  
+00005150: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00005160: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00005170: 6c6f 672e 6f70 656e 2829 0a0a 2020 2020  log.open()..    
+00005180: 6465 6620 7361 7665 5f65 6469 7465 645f  def save_edited_
+00005190: 636f 6e74 6573 7428 7365 6c66 293a 0a20  contest(self):. 
+000051a0: 2020 2020 2020 2022 2222 5361 7665 2074         """Save t
+000051b0: 6865 2065 6469 7465 6420 636f 6e74 6573  he edited contes
+000051c0: 7422 2222 0a20 2020 2020 2020 2063 6f6e  t""".        con
+000051d0: 7465 7374 203d 207b 7d0a 2020 2020 2020  test = {}.      
+000051e0: 2020 636f 6e74 6573 745b 2243 6f6e 7465    contest["Conte
+000051f0: 7374 4e61 6d65 225d 203d 2028 0a20 2020  stName"] = (.   
+00005200: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00005210: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+00005220: 7465 7374 2e63 7572 7265 6e74 5465 7874  test.currentText
+00005230: 2829 2e6c 6f77 6572 2829 2e72 6570 6c61  ().lower().repla
+00005240: 6365 2822 2022 2c20 225f 2229 0a20 2020  ce(" ", "_").   
+00005250: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
+00005260: 6f6e 7465 7374 5b22 5374 6172 7444 6174  ontest["StartDat
+00005270: 6522 5d20 3d20 7365 6c66 2e63 6f6e 7465  e"] = self.conte
+00005280: 7374 5f64 6961 6c6f 672e 6461 7465 5469  st_dialog.dateTi
+00005290: 6d65 4564 6974 2e64 6174 6554 696d 6528  meEdit.dateTime(
+000052a0: 292e 746f 5374 7269 6e67 280a 2020 2020  ).toString(.    
+000052b0: 2020 2020 2020 2020 2279 7979 792d 4d4d          "yyyy-MM
+000052c0: 2d64 6420 6868 3a6d 6d3a 7373 220a 2020  -dd hh:mm:ss".  
+000052d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000052e0: 636f 6e74 6573 745b 224f 7065 7261 746f  contest["Operato
+000052f0: 7243 6174 6567 6f72 7922 5d20 3d20 7365  rCategory"] = se
+00005300: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00005310: 672e 6f70 6572 6174 6f72 5f63 6c61 7373  g.operator_class
+00005320: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
+00005330: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
+00005340: 4261 6e64 4361 7465 676f 7279 225d 203d  BandCategory"] =
+00005350: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00005360: 616c 6f67 2e62 616e 642e 6375 7272 656e  alog.band.curren
+00005370: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
+00005380: 636f 6e74 6573 745b 2250 6f77 6572 4361  contest["PowerCa
+00005390: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
+000053a0: 636f 6e74 6573 745f 6469 616c 6f67 2e70  contest_dialog.p
+000053b0: 6f77 6572 2e63 7572 7265 6e74 5465 7874  ower.currentText
+000053c0: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
+000053d0: 7374 5b22 4d6f 6465 4361 7465 676f 7279  st["ModeCategory
+000053e0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+000053f0: 745f 6469 616c 6f67 2e6d 6f64 652e 6375  t_dialog.mode.cu
+00005400: 7272 656e 7454 6578 7428 290a 2020 2020  rrentText().    
+00005410: 2020 2020 636f 6e74 6573 745b 224f 7665      contest["Ove
+00005420: 726c 6179 4361 7465 676f 7279 225d 203d  rlayCategory"] =
+00005430: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00005440: 616c 6f67 2e6f 7665 726c 6179 2e63 7572  alog.overlay.cur
+00005450: 7265 6e74 5465 7874 2829 0a20 2020 2020  rentText().     
+00005460: 2020 2063 6f6e 7465 7374 5b22 4f70 6572     contest["Oper
+00005470: 6174 6f72 7322 5d20 3d20 7365 6c66 2e63  ators"] = self.c
+00005480: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
+00005490: 6572 6174 6f72 732e 7465 7874 2829 0a20  erators.text(). 
+000054a0: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
+000054b0: 536f 6170 626f 7822 5d20 3d20 7365 6c66  Soapbox"] = self
+000054c0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+000054d0: 736f 6170 626f 782e 746f 506c 6169 6e54  soapbox.toPlainT
+000054e0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+000054f0: 6e74 6573 745b 2253 656e 7445 7863 6861  ntest["SentExcha
+00005500: 6e67 6522 5d20 3d20 7365 6c66 2e63 6f6e  nge"] = self.con
+00005510: 7465 7374 5f64 6961 6c6f 672e 6578 6368  test_dialog.exch
+00005520: 616e 6765 2e74 6578 7428 290a 2020 2020  ange.text().    
+00005530: 2020 2020 636f 6e74 6573 745b 2243 6f6e      contest["Con
+00005540: 7465 7374 4e52 225d 203d 2073 656c 662e  testNR"] = self.
+00005550: 7072 6566 2e67 6574 2822 636f 6e74 6573  pref.get("contes
+00005560: 7422 2c20 3129 0a20 2020 2020 2020 2063  t", 1).        c
+00005570: 6f6e 7465 7374 5b22 5374 6174 696f 6e43  ontest["StationC
+00005580: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
+00005590: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+000055a0: 7374 6174 696f 6e2e 6375 7272 656e 7454  station.currentT
+000055b0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+000055c0: 6e74 6573 745b 2241 7373 6973 7465 6443  ntest["AssistedC
+000055d0: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
+000055e0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+000055f0: 6173 7369 7374 6564 2e63 7572 7265 6e74  assisted.current
+00005600: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
+00005610: 6f6e 7465 7374 5b22 5472 616e 736d 6974  ontest["Transmit
+00005620: 7465 7243 6174 6567 6f72 7922 5d20 3d20  terCategory"] = 
+00005630: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00005640: 6c6f 672e 7472 616e 736d 6974 7465 722e  log.transmitter.
+00005650: 6375 7272 656e 7454 6578 7428 290a 0a20  currentText().. 
+00005660: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00005670: 6275 6728 2225 7322 2c20 6622 7b63 6f6e  bug("%s", f"{con
+00005680: 7465 7374 7d22 290a 2020 2020 2020 2020  test}").        
+00005690: 7365 6c66 2e64 6174 6162 6173 652e 7570  self.database.up
+000056a0: 6461 7465 5f63 6f6e 7465 7374 2863 6f6e  date_contest(con
+000056b0: 7465 7374 290a 2020 2020 2020 2020 7365  test).        se
+000056c0: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
+000056d0: 6e63 6528 290a 2020 2020 2020 2020 7365  nce().        se
+000056e0: 6c66 2e6c 6f61 645f 636f 6e74 6573 7428  lf.load_contest(
+000056f0: 290a 0a20 2020 2064 6566 206c 6f61 645f  )..    def load_
+00005700: 636f 6e74 6573 7428 7365 6c66 293a 0a20  contest(self):. 
+00005710: 2020 2020 2020 2022 2222 6c6f 6164 2061         """load a
+00005720: 2063 6f6e 7465 7374 2222 220a 2020 2020   contest""".    
+00005730: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
+00005740: 2e67 6574 2822 636f 6e74 6573 7422 293a  .get("contest"):
+00005750: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005760: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
+00005770: 6773 203d 2073 656c 662e 6461 7461 6261  gs = self.databa
+00005780: 7365 2e66 6574 6368 5f63 6f6e 7465 7374  se.fetch_contest
+00005790: 5f62 795f 6964 280a 2020 2020 2020 2020  _by_id(.        
+000057a0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+000057b0: 662e 6765 7428 2263 6f6e 7465 7374 2229  f.get("contest")
+000057c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000057d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000057e0: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
+000057f0: 6e67 733a 0a20 2020 2020 2020 2020 2020  ngs:.           
+00005800: 2020 2020 2073 656c 662e 6461 7461 6261       self.databa
+00005810: 7365 2e63 7572 7265 6e74 5f63 6f6e 7465  se.current_conte
+00005820: 7374 203d 2073 656c 662e 7072 6566 2e67  st = self.pref.g
+00005830: 6574 2822 636f 6e74 6573 7422 290a 2020  et("contest").  
+00005840: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005850: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
+00005860: 7474 696e 6773 2e67 6574 2822 436f 6e74  ttings.get("Cont
+00005870: 6573 744e 616d 6522 293a 0a20 2020 2020  estName"):.     
+00005880: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005890: 656c 662e 636f 6e74 6573 7420 3d20 646f  elf.contest = do
+000058a0: 696d 7028 7365 6c66 2e63 6f6e 7465 7374  imp(self.contest
+000058b0: 5f73 6574 7469 6e67 732e 6765 7428 2243  _settings.get("C
+000058c0: 6f6e 7465 7374 4e61 6d65 2229 290a 2020  ontestName")).  
+000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058e0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+000058f0: 4c6f 6164 6564 2043 6f6e 7465 7374 204e  Loaded Contest N
+00005900: 616d 6520 3d20 2573 222c 2073 656c 662e  ame = %s", self.
+00005910: 636f 6e74 6573 742e 6e61 6d65 290a 2020  contest.name).  
+00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005930: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
+00005940: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
+00005950: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005960: 6c66 2e63 6f6e 7465 7374 2e69 6e69 745f  lf.contest.init_
+00005970: 636f 6e74 6573 7428 7365 6c66 290a 2020  contest(self).  
+00005980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005990: 2020 7365 6c66 2e68 6964 655f 6261 6e64    self.hide_band
+000059a0: 5f6d 6f64 6528 7365 6c66 2e63 6f6e 7465  _mode(self.conte
+000059b0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
+000059c0: 224d 6f64 6543 6174 6567 6f72 7922 2c20  "ModeCategory", 
+000059d0: 2222 2929 0a20 2020 2020 2020 2020 2020  "")).           
+000059e0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+000059f0: 6465 6275 6728 2225 7322 2c20 6622 7b73  debug("%s", f"{s
+00005a00: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
+00005a10: 696e 6773 7d22 290a 2020 2020 2020 2020  ings}").        
+00005a20: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00005a30: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
+00005a40: 696e 6773 2e67 6574 2822 4d6f 6465 4361  ings.get("ModeCa
+00005a50: 7465 676f 7279 222c 2022 2229 203d 3d20  tegory", "") == 
+00005a60: 2243 5722 3a0a 2020 2020 2020 2020 2020  "CW":.          
+00005a70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005a80: 6c66 2e73 6574 6d6f 6465 2822 4357 2229  lf.setmode("CW")
+00005a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005aa0: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+00005ab0: 6469 6f5f 7374 6174 655b 226d 6f64 6522  dio_state["mode"
+00005ac0: 5d20 3d20 2243 5722 0a20 2020 2020 2020  ] = "CW".       
+00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ae0: 2069 6620 7365 6c66 2e72 6967 5f63 6f6e   if self.rig_con
+00005af0: 7472 6f6c 3a0a 2020 2020 2020 2020 2020  trol:.          
+00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b10: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
+00005b20: 6e74 726f 6c2e 6f6e 6c69 6e65 3a0a 2020  ntrol.online:.  
+00005b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005b50: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e73  lf.rig_control.s
+00005b60: 6574 5f6d 6f64 6528 2243 5722 290a 2020  et_mode("CW").  
+00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b80: 2020 2020 2020 6261 6e64 203d 2067 6574        band = get
+00005b90: 6261 6e64 2873 7472 2873 656c 662e 7261  band(str(self.ra
+00005ba0: 6469 6f5f 7374 6174 652e 6765 7428 2276  dio_state.get("v
+00005bb0: 666f 6122 2c20 2230 2e30 2229 2929 0a20  foa", "0.0"))). 
+00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bd0: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00005be0: 6261 6e64 5f69 6e64 6963 6174 6f72 2862  band_indicator(b
+00005bf0: 616e 6429 0a20 2020 2020 2020 2020 2020  and).           
+00005c00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005c10: 662e 7365 745f 7769 6e64 6f77 5f74 6974  f.set_window_tit
+00005c20: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
+00005c30: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00005c40: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
+00005c50: 732e 6765 7428 224d 6f64 6543 6174 6567  s.get("ModeCateg
+00005c60: 6f72 7922 2c20 2222 2920 3d3d 2022 5353  ory", "") == "SS
+00005c70: 4222 3a0a 2020 2020 2020 2020 2020 2020  B":.            
+00005c80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005c90: 2e73 6574 6d6f 6465 2822 5353 4222 290a  .setmode("SSB").
+00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cb0: 2020 2020 2020 2020 6966 2069 6e74 2873          if int(s
+00005cc0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+00005cd0: 6765 7428 2276 666f 6122 2c20 3029 2920  get("vfoa", 0)) 
+00005ce0: 3e20 3130 3030 3030 3030 3a0a 2020 2020  > 10000000:.    
+00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d00: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+00005d10: 696f 5f73 7461 7465 5b22 6d6f 6465 225d  io_state["mode"]
+00005d20: 203d 2022 5553 4222 0a20 2020 2020 2020   = "USB".       
+00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 2020 2073 656c 662e 7261 6469 6f5f 7374     self.radio_st
+00005d70: 6174 655b 226d 6f64 6522 5d20 3d20 224c  ate["mode"] = "L
+00005d80: 5342 220a 2020 2020 2020 2020 2020 2020  SB".            
+00005d90: 2020 2020 2020 2020 2020 2020 6261 6e64              band
+00005da0: 203d 2067 6574 6261 6e64 2873 7472 2873   = getband(str(s
+00005db0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+00005dc0: 6765 7428 2276 666f 6122 2c20 2230 2e30  get("vfoa", "0.0
+00005dd0: 2229 2929 0a20 2020 2020 2020 2020 2020  "))).           
+00005de0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005df0: 662e 7365 745f 6261 6e64 5f69 6e64 6963  f.set_band_indic
+00005e00: 6174 6f72 2862 616e 6429 0a20 2020 2020  ator(band).     
+00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e20: 2020 2073 656c 662e 7365 745f 7769 6e64     self.set_wind
+00005e30: 6f77 5f74 6974 6c65 2829 0a20 2020 2020  ow_title().     
 00005e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e50: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-00005e60: 655b 226d 6f64 6522 5d20 3d20 224c 5342  e["mode"] = "LSB
-00005e70: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00005e80: 2020 2020 2020 2020 2020 6261 6e64 203d            band =
-00005e90: 2067 6574 6261 6e64 2873 7472 2873 656c   getband(str(sel
-00005ea0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-00005eb0: 7428 2276 666f 6122 2c20 2230 2e30 2229  t("vfoa", "0.0")
-00005ec0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00005ed0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005ee0: 7365 745f 6261 6e64 5f69 6e64 6963 6174  set_band_indicat
-00005ef0: 6f72 2862 616e 6429 0a20 2020 2020 2020  or(band).       
-00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f10: 2073 656c 662e 7365 745f 7769 6e64 6f77   self.set_window
-00005f20: 5f74 6974 6c65 2829 0a20 2020 2020 2020  _title().       
-00005f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f40: 2069 6620 7365 6c66 2e72 6967 5f63 6f6e   if self.rig_con
-00005f50: 7472 6f6c 3a0a 2020 2020 2020 2020 2020  trol:.          
-00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f70: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
-00005f80: 6f6c 2e73 6574 5f6d 6f64 6528 7365 6c66  ol.set_mode(self
-00005f90: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-00005fa0: 2822 6d6f 6465 2229 290a 0a20 2020 2020  ("mode"))..     
-00005fb0: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
-00005fc0: 7361 7474 7228 7365 6c66 2e63 6f6e 7465  sattr(self.conte
-00005fd0: 7374 2c20 226d 6f64 6522 293a 0a20 2020  st, "mode"):.   
-00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ff0: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
-00006000: 7322 2c20 6622 2020 2a2a 2a2a 2020 7b73  s", f"  ****  {s
-00006010: 656c 662e 636f 6e74 6573 747d 2229 0a20  elf.contest}"). 
+00005e50: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
+00005e60: 6f6e 7472 6f6c 3a0a 2020 2020 2020 2020  ontrol:.        
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e80: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
+00005e90: 7472 6f6c 2e73 6574 5f6d 6f64 6528 7365  trol.set_mode(se
+00005ea0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+00005eb0: 6574 2822 6d6f 6465 2229 290a 0a20 2020  et("mode"))..   
+00005ec0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00005ed0: 6861 7361 7474 7228 7365 6c66 2e63 6f6e  hasattr(self.con
+00005ee0: 7465 7374 2c20 226d 6f64 6522 293a 0a20  test, "mode"):. 
+00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f00: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00005f10: 2225 7322 2c20 6622 2020 2a2a 2a2a 2020  "%s", f"  ****  
+00005f20: 7b73 656c 662e 636f 6e74 6573 747d 2229  {self.contest}")
+00005f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005f40: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+00005f50: 7465 7374 2e6d 6f64 6520 696e 205b 2243  test.mode in ["C
+00005f60: 5722 2c20 2242 4f54 4822 5d3a 0a20 2020  W", "BOTH"]:.   
+00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f80: 2020 2020 2073 656c 662e 6377 5f73 7065       self.cw_spe
+00005f90: 6564 2e73 686f 7728 290a 2020 2020 2020  ed.show().      
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00005fb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00005fc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005fd0: 2e63 775f 7370 6565 642e 6869 6465 2829  .cw_speed.hide()
+00005fe0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005ff0: 2020 636d 6420 3d20 7b7d 0a20 2020 2020    cmd = {}.     
+00006000: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+00006010: 636d 6422 5d20 3d20 224e 4557 4442 220a  cmd"] = "NEWDB".
 00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006030: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
-00006040: 7374 2e6d 6f64 6520 696e 205b 2243 5722  st.mode in ["CW"
-00006050: 2c20 2242 4f54 4822 5d3a 0a20 2020 2020  , "BOTH"]:.     
-00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006070: 2020 2073 656c 662e 6377 5f73 7065 6564     self.cw_speed
-00006080: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
-00006090: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000060a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000060b0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000060c0: 775f 7370 6565 642e 6869 6465 2829 0a0a  w_speed.hide()..
-000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060e0: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
-000060f0: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
-00006100: 6422 5d20 3d20 224e 4557 4442 220a 2020  d"] = "NEWDB".  
-00006110: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-00006120: 645b 2273 7461 7469 6f6e 225d 203d 2070  d["station"] = p
-00006130: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
-00006140: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006150: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
-00006160: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
-00006170: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
-00006180: 2020 2020 2020 2020 2020 6966 2068 6173            if has
-00006190: 6174 7472 2873 656c 662e 636f 6e74 6573  attr(self.contes
-000061a0: 742c 2022 636f 6c75 6d6e 7322 293a 0a20  t, "columns"):. 
-000061b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061c0: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061e0: 636d 645b 2263 6d64 225d 203d 2022 5348  cmd["cmd"] = "SH
-000061f0: 4f57 434f 4c55 4d4e 5322 0a20 2020 2020  OWCOLUMNS".     
-00006200: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00006210: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
-00006220: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
-00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006240: 2020 2020 636d 645b 2243 4f4c 554d 4e53      cmd["COLUMNS
-00006250: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-00006260: 742e 636f 6c75 6d6e 730a 2020 2020 2020  t.columns.      
-00006270: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006280: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-00006290: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
-000062a0: 736f 6e28 636d 6429 0a0a 2020 2020 6465  son(cmd)..    de
-000062b0: 6620 6368 6563 6b5f 666f 725f 6e65 775f  f check_for_new_
-000062c0: 6374 7928 7365 6c66 293a 0a20 2020 2020  cty(self):.     
-000062d0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-000062e0: 6865 636b 7320 666f 7220 6120 6e65 7720  hecks for a new 
-000062f0: 6374 792e 6461 7420 6669 6c65 2e0a 2020  cty.dat file..  
-00006300: 2020 2020 2020 4c6f 6164 7320 6974 2069        Loads it i
-00006310: 6620 6176 6169 6c61 626c 652e 0a20 2020  f available..   
-00006320: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00006330: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00006340: 2020 6374 7920 3d20 6e6f 7463 7479 7061    cty = notctypa
-00006350: 7273 6572 2e42 6967 4374 7928 574f 524b  rser.BigCty(WORK
-00006360: 494e 475f 5041 5448 202b 2022 2f64 6174  ING_PATH + "/dat
-00006370: 612f 6374 792e 6a73 6f6e 2229 0a20 2020  a/cty.json").   
-00006380: 2020 2020 2020 2020 2075 7064 6174 655f           update_
-00006390: 6176 6169 6c61 626c 6520 3d20 6374 792e  available = cty.
-000063a0: 6368 6563 6b5f 7570 6461 7465 2829 0a20  check_update(). 
-000063b0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-000063c0: 6365 7074 696f 6e20 6173 2074 6865 5f65  ception as the_e
-000063d0: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
-000063e0: 2020 6374 7920 3d20 4e6f 6e65 2020 2320    cty = None  # 
-000063f0: 6672 6565 2075 7020 7468 6520 6d65 6d6f  free up the memo
-00006400: 7279 0a20 2020 2020 2020 2020 2020 206c  ry.            l
-00006410: 6f67 6765 722e 6465 6275 6728 2263 7479  ogger.debug("cty
-00006420: 2070 6172 7365 7220 7265 7475 726e 6564   parser returned
-00006430: 2061 6e20 6572 726f 723a 2025 7322 2c20   an error: %s", 
-00006440: 7468 655f 6572 726f 7229 0a20 2020 2020  the_error).     
-00006450: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00006460: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00006470: 7567 2822 4e65 7765 7220 6374 7920 6669  ug("Newer cty fi
-00006480: 6c65 2061 7661 696c 6162 6c65 2025 7322  le available %s"
-00006490: 2c20 7374 7228 7570 6461 7465 5f61 7661  , str(update_ava
-000064a0: 696c 6162 6c65 2929 0a0a 2020 2020 2020  ilable))..      
-000064b0: 2020 6966 2075 7064 6174 655f 6176 6169    if update_avai
-000064c0: 6c61 626c 653a 0a20 2020 2020 2020 2020  lable:.         
-000064d0: 2020 2073 656c 662e 7368 6f77 5f6d 6573     self.show_mes
-000064e0: 7361 6765 5f62 6f78 2822 5570 6461 7469  sage_box("Updati
-000064f0: 6e67 2063 7479 2066 696c 652e 2e22 290a  ng cty file..").
-00006500: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00006510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006520: 2075 7064 6174 6564 203d 2063 7479 2e75   updated = cty.u
-00006530: 7064 6174 6528 290a 2020 2020 2020 2020  pdate().        
-00006540: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00006550: 7469 6f6e 2061 7320 7468 655f 6572 726f  tion as the_erro
-00006560: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00006570: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00006580: 2263 7479 2070 6172 7365 7220 7265 7475  "cty parser retu
-00006590: 726e 6564 2061 6e20 6572 726f 723a 2025  rned an error: %
-000065a0: 7322 2c20 7468 655f 6572 726f 7229 0a20  s", the_error). 
-000065b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000065c0: 7479 203d 204e 6f6e 6520 2023 2066 7265  ty = None  # fre
-000065d0: 6520 7570 2074 6865 206d 656d 6f72 790a  e up the memory.
-000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065f0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-00006600: 2020 2069 6620 7570 6461 7465 643a 0a20     if updated:. 
-00006610: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00006620: 7479 2e64 756d 7028 574f 524b 494e 475f  ty.dump(WORKING_
-00006630: 5041 5448 202b 2022 2f64 6174 612f 6374  PATH + "/data/ct
-00006640: 792e 6a73 6f6e 2229 0a20 2020 2020 2020  y.json").       
-00006650: 2020 2020 2020 2020 2073 656c 662e 7368           self.sh
-00006660: 6f77 5f6d 6573 7361 6765 5f62 6f78 2822  ow_message_box("
-00006670: 6374 7920 6669 6c65 2075 7064 6174 6564  cty file updated
-00006680: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-00006690: 2020 2020 7769 7468 206f 7065 6e28 0a20      with open(. 
-000066a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066b0: 2020 2057 4f52 4b49 4e47 5f50 4154 4820     WORKING_PATH 
-000066c0: 2b20 222f 6461 7461 2f63 7479 2e6a 736f  + "/data/cty.jso
-000066d0: 6e22 2c20 2272 7422 2c20 656e 636f 6469  n", "rt", encodi
-000066e0: 6e67 3d22 7574 662d 3822 0a20 2020 2020  ng="utf-8".     
-000066f0: 2020 2020 2020 2020 2020 2029 2061 7320             ) as 
-00006700: 635f 6669 6c65 3a0a 2020 2020 2020 2020  c_file:.        
-00006710: 2020 2020 2020 2020 2020 2020 676c 6f62              glob
-00006720: 616c 7328 295b 2243 5459 4649 4c45 225d  als()["CTYFILE"]
-00006730: 203d 206c 6f61 6473 2863 5f66 696c 652e   = loads(c_file.
-00006740: 7265 6164 2829 290a 2020 2020 2020 2020  read()).        
-00006750: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00006760: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00006770: 686f 775f 6d65 7373 6167 655f 626f 7828  how_message_box(
-00006780: 2241 6e20 4572 726f 7220 6f63 6375 7265  "An Error occure
-00006790: 6420 7570 6461 7469 6e67 2066 696c 652e  d updating file.
-000067a0: 2229 0a20 2020 2020 2020 2063 7479 203d  ").        cty =
-000067b0: 204e 6f6e 6520 2023 2066 7265 6520 7570   None  # free up
-000067c0: 2074 6865 206d 656d 6f72 790a 0a20 2020   the memory..   
-000067d0: 2064 6566 2068 6964 655f 6261 6e64 5f6d   def hide_band_m
-000067e0: 6f64 6528 7365 6c66 2c20 7468 655f 6d6f  ode(self, the_mo
-000067f0: 6465 3a20 7374 7229 202d 3e20 4e6f 6e65  de: str) -> None
-00006800: 3a0a 2020 2020 2020 2020 2222 2268 6964  :.        """hid
-00006810: 6522 2222 0a20 2020 2020 2020 206c 6f67  e""".        log
-00006820: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
-00006830: 6622 7b74 6865 5f6d 6f64 657d 2229 0a20  f"{the_mode}"). 
-00006840: 2020 2020 2020 2073 656c 662e 4261 6e64         self.Band
-00006850: 5f4d 6f64 655f 4672 616d 655f 4357 2e68  _Mode_Frame_CW.h
-00006860: 6964 6528 290a 2020 2020 2020 2020 7365  ide().        se
-00006870: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
-00006880: 6d65 5f53 5342 2e68 6964 6528 290a 2020  me_SSB.hide().  
-00006890: 2020 2020 2020 7365 6c66 2e42 616e 645f        self.Band_
-000068a0: 4d6f 6465 5f46 7261 6d65 5f52 5454 592e  Mode_Frame_RTTY.
-000068b0: 6869 6465 2829 0a20 2020 2020 2020 206d  hide().        m
-000068c0: 6f64 6573 203d 207b 0a20 2020 2020 2020  odes = {.       
-000068d0: 2020 2020 2022 4357 223a 2028 7365 6c66       "CW": (self
-000068e0: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
-000068f0: 5f43 572c 292c 0a20 2020 2020 2020 2020  _CW,),.         
-00006900: 2020 2022 5353 4222 3a20 2873 656c 662e     "SSB": (self.
-00006910: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
-00006920: 5353 422c 292c 0a20 2020 2020 2020 2020  SSB,),.         
-00006930: 2020 2022 5254 5459 223a 2028 7365 6c66     "RTTY": (self
-00006940: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
-00006950: 5f52 5454 592c 292c 0a20 2020 2020 2020  _RTTY,),.       
-00006960: 2020 2020 2022 5053 4b22 3a20 2873 656c       "PSK": (sel
-00006970: 662e 4261 6e64 5f4d 6f64 655f 4672 616d  f.Band_Mode_Fram
-00006980: 655f 5254 5459 2c29 2c0a 2020 2020 2020  e_RTTY,),.      
-00006990: 2020 2020 2020 2253 5342 2b43 5722 3a20        "SSB+CW": 
-000069a0: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
-000069b0: 4672 616d 655f 4357 2c20 7365 6c66 2e42  Frame_CW, self.B
-000069c0: 616e 645f 4d6f 6465 5f46 7261 6d65 5f53  and_Mode_Frame_S
-000069d0: 5342 292c 0a20 2020 2020 2020 2020 2020  SB),.           
-000069e0: 2022 424f 5448 223a 2028 7365 6c66 2e42   "BOTH": (self.B
-000069f0: 616e 645f 4d6f 6465 5f46 7261 6d65 5f43  and_Mode_Frame_C
-00006a00: 572c 2073 656c 662e 4261 6e64 5f4d 6f64  W, self.Band_Mod
-00006a10: 655f 4672 616d 655f 5353 4229 2c0a 2020  e_Frame_SSB),.  
-00006a20: 2020 2020 2020 2020 2020 2244 4947 4954            "DIGIT
-00006a30: 414c 223a 2028 7365 6c66 2e42 616e 645f  AL": (self.Band_
-00006a40: 4d6f 6465 5f46 7261 6d65 5f52 5454 592c  Mode_Frame_RTTY,
-00006a50: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
-00006a60: 5353 422b 4357 2b44 4947 4954 414c 223a  SSB+CW+DIGITAL":
-00006a70: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00006a80: 2020 2073 656c 662e 4261 6e64 5f4d 6f64     self.Band_Mod
-00006a90: 655f 4672 616d 655f 5254 5459 2c0a 2020  e_Frame_RTTY,.  
-00006aa0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006ab0: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
-00006ac0: 6d65 5f43 572c 0a20 2020 2020 2020 2020  me_CW,.         
-00006ad0: 2020 2020 2020 2073 656c 662e 4261 6e64         self.Band
-00006ae0: 5f4d 6f64 655f 4672 616d 655f 5353 422c  _Mode_Frame_SSB,
-00006af0: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-00006b00: 2020 2020 2020 2020 2020 2020 2246 4d22              "FM"
-00006b10: 3a20 2873 656c 662e 4261 6e64 5f4d 6f64  : (self.Band_Mod
-00006b20: 655f 4672 616d 655f 5353 422c 292c 0a20  e_Frame_SSB,),. 
-00006b30: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00006b40: 2066 7261 6d65 7320 3d20 6d6f 6465 732e   frames = modes.
-00006b50: 6765 7428 7468 655f 6d6f 6465 290a 2020  get(the_mode).  
-00006b60: 2020 2020 2020 6966 2066 7261 6d65 733a        if frames:
-00006b70: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00006b80: 2066 7261 6d65 2069 6e20 6672 616d 6573   frame in frames
-00006b90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006ba0: 2020 6672 616d 652e 7368 6f77 2829 0a0a    frame.show()..
-00006bb0: 2020 2020 6465 6620 6669 6c65 7069 636b      def filepick
-00006bc0: 6572 2873 656c 662c 2061 6374 696f 6e3a  er(self, action:
-00006bd0: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
-00006be0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00006bf0: 2020 4765 7420 6120 6669 6c65 6e61 6d65    Get a filename
-00006c00: 0a20 2020 2020 2020 2061 6374 696f 6e3a  .        action:
-00006c10: 2022 6e65 7722 206f 7220 226f 7065 6e22   "new" or "open"
-00006c20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00006c30: 2020 2020 206f 7074 696f 6e73 203d 2051       options = Q
-00006c40: 4669 6c65 4469 616c 6f67 2e4f 7074 696f  FileDialog.Optio
-00006c50: 6e73 2829 0a20 2020 2020 2020 206f 7074  ns().        opt
-00006c60: 696f 6e73 207c 3d20 5146 696c 6544 6961  ions |= QFileDia
-00006c70: 6c6f 672e 446f 6e74 5573 654e 6174 6976  log.DontUseNativ
-00006c80: 6544 6961 6c6f 670a 2020 2020 2020 2020  eDialog.        
-00006c90: 6f70 7469 6f6e 7320 7c3d 2051 4669 6c65  options |= QFile
-00006ca0: 4469 616c 6f67 2e44 6f6e 7443 6f6e 6669  Dialog.DontConfi
-00006cb0: 726d 4f76 6572 7772 6974 650a 2020 2020  rmOverwrite.    
-00006cc0: 2020 2020 6966 2061 6374 696f 6e20 3d3d      if action ==
-00006cd0: 2022 6e65 7722 3a0a 2020 2020 2020 2020   "new":.        
-00006ce0: 2020 2020 6669 6c65 2c20 5f20 3d20 5146      file, _ = QF
-00006cf0: 696c 6544 6961 6c6f 672e 6765 7453 6176  ileDialog.getSav
-00006d00: 6546 696c 654e 616d 6528 0a20 2020 2020  eFileName(.     
-00006d10: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-00006d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d30: 2022 4368 6f6f 7365 2061 2044 6174 6162   "Choose a Datab
-00006d40: 6173 6522 2c0a 2020 2020 2020 2020 2020  ase",.          
-00006d50: 2020 2020 2020 4441 5441 5f50 4154 482c        DATA_PATH,
-00006d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d70: 2022 4461 7461 6261 7365 2028 2a2e 6462   "Database (*.db
-00006d80: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
-00006d90: 2020 2020 6f70 7469 6f6e 733d 6f70 7469      options=opti
-00006da0: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
-00006db0: 2029 0a20 2020 2020 2020 2069 6620 6163   ).        if ac
-00006dc0: 7469 6f6e 203d 3d20 226f 7065 6e22 3a0a  tion == "open":.
-00006dd0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00006de0: 2c20 5f20 3d20 5146 696c 6544 6961 6c6f  , _ = QFileDialo
-00006df0: 672e 6765 744f 7065 6e46 696c 654e 616d  g.getOpenFileNam
-00006e00: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00006e10: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00006e20: 2020 2020 2020 2020 2022 4368 6f6f 7365           "Choose
-00006e30: 2061 2044 6174 6162 6173 6522 2c0a 2020   a Database",.  
-00006e40: 2020 2020 2020 2020 2020 2020 2020 4441                DA
-00006e50: 5441 5f50 4154 482c 0a20 2020 2020 2020  TA_PATH,.       
-00006e60: 2020 2020 2020 2020 2022 4461 7461 6261           "Databa
-00006e70: 7365 2028 2a2e 6462 2922 2c0a 2020 2020  se (*.db)",.    
-00006e80: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-00006e90: 6f6e 733d 6f70 7469 6f6e 732c 0a20 2020  ons=options,.   
-00006ea0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00006eb0: 2020 2072 6574 7572 6e20 6669 6c65 0a0a     return file..
-00006ec0: 2020 2020 6465 6620 7265 6361 6c63 756c      def recalcul
-00006ed0: 6174 655f 6d75 6c74 7328 7365 6c66 293a  ate_mults(self):
-00006ee0: 0a20 2020 2020 2020 2022 2222 5265 6361  .        """Reca
-00006ef0: 6c63 756c 6174 6520 4d75 6c74 6970 6c69  lculate Multipli
-00006f00: 6572 7322 2222 0a20 2020 2020 2020 2073  ers""".        s
-00006f10: 656c 662e 636f 6e74 6573 742e 7265 6361  elf.contest.reca
-00006f20: 6c63 756c 6174 655f 6d75 6c74 7328 7365  lculate_mults(se
-00006f30: 6c66 290a 0a20 2020 2064 6566 206c 6175  lf)..    def lau
-00006f40: 6e63 685f 6c6f 675f 7769 6e64 6f77 2873  nch_log_window(s
-00006f50: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00006f60: 226c 6175 6e63 6820 7468 6520 4c6f 6720  "launch the Log 
-00006f70: 5769 6e64 6f77 2222 220a 2020 2020 2020  Window""".      
-00006f80: 2020 6966 206e 6f74 2063 6865 636b 5f70    if not check_p
-00006f90: 726f 6365 7373 2822 6c6f 6777 696e 646f  rocess("logwindo
-00006fa0: 772e 7079 2229 3a0a 2020 2020 2020 2020  w.py"):.        
-00006fb0: 2020 2020 5f20 3d20 7375 6270 726f 6365      _ = subproce
-00006fc0: 7373 2e50 6f70 656e 285b 7379 732e 6578  ss.Popen([sys.ex
-00006fd0: 6563 7574 6162 6c65 2c20 574f 524b 494e  ecutable, WORKIN
-00006fe0: 475f 5041 5448 202b 2022 2f6c 6f67 7769  G_PATH + "/logwi
-00006ff0: 6e64 6f77 2e70 7922 5d29 0a0a 2020 2020  ndow.py"])..    
-00007000: 6465 6620 6c61 756e 6368 5f62 616e 646d  def launch_bandm
-00007010: 6170 5f77 696e 646f 7728 7365 6c66 293a  ap_window(self):
-00007020: 0a20 2020 2020 2020 2022 2222 6c61 756e  .        """laun
-00007030: 6368 2074 6865 204c 6f67 2057 696e 646f  ch the Log Windo
-00007040: 7722 2222 0a20 2020 2020 2020 2069 6620  w""".        if 
-00007050: 6e6f 7420 6368 6563 6b5f 7072 6f63 6573  not check_proces
-00007060: 7328 2262 616e 646d 6170 2e70 7922 293a  s("bandmap.py"):
-00007070: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
-00007080: 2073 7562 7072 6f63 6573 732e 506f 7065   subprocess.Pope
-00007090: 6e28 5b73 7973 2e65 7865 6375 7461 626c  n([sys.executabl
-000070a0: 652c 2057 4f52 4b49 4e47 5f50 4154 4820  e, WORKING_PATH 
-000070b0: 2b20 222f 6261 6e64 6d61 702e 7079 225d  + "/bandmap.py"]
-000070c0: 290a 0a20 2020 2064 6566 2063 6c65 6172  )..    def clear
-000070d0: 5f62 616e 645f 696e 6469 6361 746f 7273  _band_indicators
-000070e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000070f0: 2222 2243 6c65 6172 2074 6865 2069 6e64  """Clear the ind
-00007100: 6963 6174 6f72 7322 2222 0a20 2020 2020  icators""".     
-00007110: 2020 2066 6f72 205f 2c20 696e 6469 6361     for _, indica
-00007120: 746f 7273 2069 6e20 7365 6c66 2e61 6c6c  tors in self.all
-00007130: 5f6d 6f64 655f 696e 6469 6361 746f 7273  _mode_indicators
-00007140: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00007150: 2020 2020 2020 666f 7220 5f2c 2069 6e64        for _, ind
-00007160: 6963 6174 6f72 2069 6e20 696e 6469 6361  icator in indica
-00007170: 746f 7273 2e69 7465 6d73 2829 3a0a 2020  tors.items():.  
-00007180: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00007190: 6469 6361 746f 722e 7365 7446 7261 6d65  dicator.setFrame
-000071a0: 5368 6170 6528 5174 5769 6467 6574 732e  Shape(QtWidgets.
-000071b0: 5146 7261 6d65 2e4e 6f46 7261 6d65 290a  QFrame.NoFrame).
-000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071d0: 696e 6469 6361 746f 722e 7365 7453 7479  indicator.setSty
-000071e0: 6c65 5368 6565 7428 2266 6f6e 742d 6661  leSheet("font-fa
-000071f0: 6d69 6c79 3a20 4a65 7442 7261 696e 7320  mily: JetBrains 
-00007200: 4d6f 6e6f 3b22 290a 0a20 2020 2064 6566  Mono;")..    def
-00007210: 2073 6574 5f62 616e 645f 696e 6469 6361   set_band_indica
-00007220: 746f 7228 7365 6c66 2c20 6261 6e64 3a20  tor(self, band: 
-00007230: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
-00007240: 2020 2020 2020 2222 2253 6574 2074 6865        """Set the
-00007250: 2062 616e 6420 696e 6469 6361 746f 7222   band indicator"
-00007260: 2222 0a20 2020 2020 2020 2023 206c 6f67  "".        # log
-00007270: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
-00007280: 6622 6261 6e64 3a7b 6261 6e64 7d20 6d6f  f"band:{band} mo
-00007290: 6465 3a20 7b73 656c 662e 6375 7272 656e  de: {self.curren
-000072a0: 745f 6d6f 6465 7d22 290a 2020 2020 2020  t_mode}").      
-000072b0: 2020 6966 2062 616e 6420 616e 6420 7365    if band and se
-000072c0: 6c66 2e63 7572 7265 6e74 5f6d 6f64 653a  lf.current_mode:
-000072d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000072e0: 662e 636c 6561 725f 6261 6e64 5f69 6e64  f.clear_band_ind
-000072f0: 6963 6174 6f72 7328 290a 2020 2020 2020  icators().      
-00007300: 2020 2020 2020 696e 6469 6361 746f 7220        indicator 
-00007310: 3d20 7365 6c66 2e61 6c6c 5f6d 6f64 655f  = self.all_mode_
-00007320: 696e 6469 6361 746f 7273 5b73 656c 662e  indicators[self.
-00007330: 6375 7272 656e 745f 6d6f 6465 5d2e 6765  current_mode].ge
-00007340: 7428 6261 6e64 2c20 4e6f 6e65 290a 2020  t(band, None).  
-00007350: 2020 2020 2020 2020 2020 6966 2069 6e64            if ind
-00007360: 6963 6174 6f72 3a0a 2020 2020 2020 2020  icator:.        
-00007370: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
-00007380: 722e 7365 7446 7261 6d65 5368 6170 6528  r.setFrameShape(
-00007390: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-000073a0: 2e42 6f78 290a 2020 2020 2020 2020 2020  .Box).          
-000073b0: 2020 2020 2020 696e 6469 6361 746f 722e        indicator.
-000073c0: 7365 7453 7479 6c65 5368 6565 7428 2266  setStyleSheet("f
-000073d0: 6f6e 742d 6661 6d69 6c79 3a20 4a65 7442  ont-family: JetB
-000073e0: 7261 696e 7320 4d6f 6e6f 3b20 636f 6c6f  rains Mono; colo
-000073f0: 723a 2067 7265 656e 3b22 290a 0a20 2020  r: green;")..   
-00007400: 2064 6566 2063 6c6f 7365 4576 656e 7428   def closeEvent(
-00007410: 7365 6c66 2c20 5f65 7665 6e74 293a 0a20  self, _event):. 
-00007420: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007430: 2020 2057 7269 7465 2077 696e 646f 7720     Write window 
-00007440: 7369 7a65 2061 6e64 2070 6f73 6974 696f  size and positio
-00007450: 6e20 746f 2063 6f6e 6669 6720 6669 6c65  n to config file
-00007460: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007470: 2020 2020 2073 656c 662e 7072 6566 5b22       self.pref["
-00007480: 7769 6e64 6f77 5f77 6964 7468 225d 203d  window_width"] =
-00007490: 2073 656c 662e 7369 7a65 2829 2e77 6964   self.size().wid
-000074a0: 7468 2829 0a20 2020 2020 2020 2073 656c  th().        sel
-000074b0: 662e 7072 6566 5b22 7769 6e64 6f77 5f68  f.pref["window_h
-000074c0: 6569 6768 7422 5d20 3d20 7365 6c66 2e73  eight"] = self.s
-000074d0: 697a 6528 292e 6865 6967 6874 2829 0a20  ize().height(). 
-000074e0: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-000074f0: 5b22 7769 6e64 6f77 5f78 225d 203d 2073  ["window_x"] = s
-00007500: 656c 662e 706f 7328 292e 7828 290a 2020  elf.pos().x().  
-00007510: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
-00007520: 2277 696e 646f 775f 7922 5d20 3d20 7365  "window_y"] = se
-00007530: 6c66 2e70 6f73 2829 2e79 2829 0a20 2020  lf.pos().y().   
-00007540: 2020 2020 2073 656c 662e 7772 6974 655f       self.write_
-00007550: 7072 6566 6572 656e 6365 2829 0a0a 2020  preference()..  
-00007560: 2020 6465 6620 6374 795f 6c6f 6f6b 7570    def cty_lookup
-00007570: 2873 656c 662c 2063 616c 6c73 6967 6e3a  (self, callsign:
-00007580: 2073 7472 293a 0a20 2020 2020 2020 2022   str):.        "
-00007590: 2222 4c6f 6f6b 7570 2063 616c 6c73 6967  ""Lookup callsig
-000075a0: 6e20 696e 2063 7479 2e64 6174 2066 696c  n in cty.dat fil
-000075b0: 6522 2222 0a20 2020 2020 2020 2063 616c  e""".        cal
-000075c0: 6c73 6967 6e20 3d20 6361 6c6c 7369 676e  lsign = callsign
-000075d0: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
-000075e0: 2066 6f72 2063 6f75 6e74 2069 6e20 7265   for count in re
-000075f0: 7665 7273 6564 2872 616e 6765 286c 656e  versed(range(len
-00007600: 2863 616c 6c73 6967 6e29 2929 3a0a 2020  (callsign))):.  
-00007610: 2020 2020 2020 2020 2020 7365 6172 6368            search
-00007620: 6974 656d 203d 2063 616c 6c73 6967 6e5b  item = callsign[
-00007630: 3a20 636f 756e 7420 2b20 315d 0a20 2020  : count + 1].   
-00007640: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-00007650: 3d20 7b6b 6579 3a20 7661 6c20 666f 7220  = {key: val for 
-00007660: 6b65 792c 2076 616c 2069 6e20 4354 5946  key, val in CTYF
-00007670: 494c 452e 6974 656d 7328 2920 6966 206b  ILE.items() if k
-00007680: 6579 203d 3d20 7365 6172 6368 6974 656d  ey == searchitem
-00007690: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
-000076a0: 206e 6f74 2072 6573 756c 743a 0a20 2020   not result:.   
-000076b0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000076c0: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-000076d0: 2020 6966 2072 6573 756c 742e 6765 7428    if result.get(
-000076e0: 7365 6172 6368 6974 656d 292e 6765 7428  searchitem).get(
-000076f0: 2265 7861 6374 5f6d 6174 6368 2229 3a0a  "exact_match"):.
-00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007710: 6966 2073 6561 7263 6869 7465 6d20 3d3d  if searchitem ==
-00007720: 2063 616c 6c73 6967 6e3a 0a20 2020 2020   callsign:.     
-00007730: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00007740: 6574 7572 6e20 7265 7375 6c74 0a20 2020  eturn result.   
-00007750: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00007760: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-00007770: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00007780: 0a20 2020 2064 6566 2063 7773 7065 6564  .    def cwspeed
-00007790: 5f73 7069 6e62 6f78 5f63 6861 6e67 6564  _spinbox_changed
-000077a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000077b0: 2222 2274 7269 6767 6572 6564 2077 6865  """triggered whe
-000077c0: 6e20 7661 6c75 6520 6f66 2043 5720 7370  n value of CW sp
-000077d0: 6565 6420 696e 2074 6865 2073 7069 6e62  eed in the spinb
-000077e0: 6f78 2063 6861 6e67 6573 2e22 2222 0a20  ox changes.""". 
-000077f0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00007800: 7720 6973 204e 6f6e 653a 0a20 2020 2020  w is None:.     
-00007810: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00007820: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
-00007830: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
-00007840: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00007850: 6c66 2e63 772e 7370 6565 6420 3d20 7365  lf.cw.speed = se
-00007860: 6c66 2e63 775f 7370 6565 642e 7661 6c75  lf.cw_speed.valu
-00007870: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00007880: 7365 6c66 2e63 772e 7365 6e64 6377 2866  self.cw.sendcw(f
-00007890: 225c 7831 6232 7b73 656c 662e 6377 2e73  "\x1b2{self.cw.s
-000078a0: 7065 6564 7d22 290a 2020 2020 2020 2020  peed}").        
-000078b0: 6966 2073 656c 662e 6377 2e73 6572 7665  if self.cw.serve
-000078c0: 7274 7970 6520 3d3d 2032 3a0a 2020 2020  rtype == 2:.    
-000078d0: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-000078e0: 7365 745f 7769 6e6b 6579 6572 5f73 7065  set_winkeyer_spe
-000078f0: 6564 2873 656c 662e 6377 5f73 7065 6564  ed(self.cw_speed
-00007900: 2e76 616c 7565 2829 290a 0a20 2020 2064  .value())..    d
-00007910: 6566 206b 6579 5072 6573 7345 7665 6e74  ef keyPressEvent
-00007920: 2873 656c 662c 2065 7665 6e74 293a 2020  (self, event):  
-00007930: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-00007940: 653d 696e 7661 6c69 642d 6e61 6d65 0a20  e=invalid-name. 
-00007950: 2020 2020 2020 2022 2222 5468 6973 206f         """This o
-00007960: 7665 7272 6964 6573 2051 7420 6b65 7920  verrides Qt key 
-00007970: 6576 656e 742e 2222 220a 2020 2020 2020  event.""".      
-00007980: 2020 6d6f 6469 6669 6572 203d 2065 7665    modifier = eve
-00007990: 6e74 2e6d 6f64 6966 6965 7273 2829 0a20  nt.modifiers(). 
-000079a0: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-000079b0: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
-000079c0: 5320 616e 6420 6d6f 6469 6669 6572 203d  S and modifier =
-000079d0: 3d20 5174 2e43 6f6e 7472 6f6c 4d6f 6469  = Qt.ControlModi
-000079e0: 6669 6572 3a0a 2020 2020 2020 2020 2020  fier:.          
-000079f0: 2020 6672 6571 203d 2073 656c 662e 7261    freq = self.ra
-00007a00: 6469 6f5f 7374 6174 652e 6765 7428 2276  dio_state.get("v
-00007a10: 666f 6122 290a 2020 2020 2020 2020 2020  foa").          
-00007a20: 2020 6478 203d 2073 656c 662e 6361 6c6c    dx = self.call
-00007a30: 7369 676e 2e74 6578 7428 290a 2020 2020  sign.text().    
-00007a40: 2020 2020 2020 2020 6966 2066 7265 7120          if freq 
-00007a50: 616e 6420 6478 3a0a 2020 2020 2020 2020  and dx:.        
-00007a60: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
-00007a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007a80: 2063 6d64 5b22 636d 6422 5d20 3d20 2253   cmd["cmd"] = "S
-00007a90: 504f 5444 5822 0a20 2020 2020 2020 2020  POTDX".         
-00007aa0: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
-00007ab0: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
-00007ac0: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-00007ad0: 2020 2020 2020 2020 636d 645b 2264 7822          cmd["dx"
-00007ae0: 5d20 3d20 6478 0a20 2020 2020 2020 2020  ] = dx.         
-00007af0: 2020 2020 2020 2063 6d64 5b22 6672 6571         cmd["freq
-00007b00: 225d 203d 2066 6c6f 6174 2869 6e74 2866  "] = float(int(f
-00007b10: 7265 7129 202f 2031 3030 3029 0a20 2020  req) / 1000).   
-00007b20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007b30: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
-00007b40: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
-00007b50: 6f6e 2863 6d64 290a 2020 2020 2020 2020  on(cmd).        
-00007b60: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00007b70: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-00007b80: 2920 3d3d 2051 742e 4b65 795f 4720 616e  ) == Qt.Key_G an
-00007b90: 6420 6d6f 6469 6669 6572 203d 3d20 5174  d modifier == Qt
-00007ba0: 2e43 6f6e 7472 6f6c 4d6f 6469 6669 6572  .ControlModifier
-00007bb0: 3a0a 2020 2020 2020 2020 2020 2020 6478  :.            dx
-00007bc0: 203d 2073 656c 662e 6361 6c6c 7369 676e   = self.callsign
-00007bd0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-00007be0: 2020 2020 6966 2064 783a 0a20 2020 2020      if dx:.     
-00007bf0: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-00007c00: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-00007c10: 2020 2020 636d 645b 2263 6d64 225d 203d      cmd["cmd"] =
-00007c20: 2022 4649 4e44 4458 220a 2020 2020 2020   "FINDDX".      
-00007c30: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
-00007c40: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
-00007c50: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
-00007c60: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00007c70: 6478 225d 203d 2064 780a 2020 2020 2020  dx"] = dx.      
-00007c80: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00007c90: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
-00007ca0: 6365 2e73 656e 645f 6173 5f6a 736f 6e28  ce.send_as_json(
-00007cb0: 636d 6429 0a20 2020 2020 2020 2020 2020  cmd).           
-00007cc0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00007cd0: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-00007ce0: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00007cf0: 5174 2e4b 6579 2e4b 6579 5f45 7363 6170  Qt.Key.Key_Escap
-00007d00: 6520 616e 6420 6d6f 6469 6669 6572 2021  e and modifier !
-00007d10: 3d20 5174 2e43 6f6e 7472 6f6c 4d6f 6469  = Qt.ControlModi
-00007d20: 6669 6572 0a20 2020 2020 2020 2029 3a20  fier.        ): 
-00007d30: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-00007d40: 6c65 3d6e 6f2d 6d65 6d62 6572 0a20 2020  le=no-member.   
-00007d50: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-00007d60: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
-00007d70: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00007d80: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-00007d90: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
-00007da0: 4b65 795f 4573 6361 7065 2061 6e64 206d  Key_Escape and m
-00007db0: 6f64 6966 6965 7220 3d3d 2051 742e 436f  odifier == Qt.Co
-00007dc0: 6e74 726f 6c4d 6f64 6966 6965 723a 0a20  ntrolModifier:. 
-00007dd0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00007de0: 6c66 2e63 7720 6973 206e 6f74 204e 6f6e  lf.cw is not Non
-00007df0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00007e00: 2020 2069 6620 7365 6c66 2e63 772e 7365     if self.cw.se
-00007e10: 7276 6572 7479 7065 203d 3d20 313a 0a20  rvertype == 1:. 
-00007e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e30: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
-00007e40: 7728 225c 7831 6234 2229 0a20 2020 2020  w("\x1b4").     
-00007e50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00007e60: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-00007e70: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00007e80: 5174 2e4b 6579 2e4b 6579 5f55 703a 0a20  Qt.Key.Key_Up:. 
-00007e90: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-00007ea0: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-00007eb0: 636d 645b 2263 6d64 225d 203d 2022 5052  cmd["cmd"] = "PR
-00007ec0: 4556 5350 4f54 220a 2020 2020 2020 2020  EVSPOT".        
-00007ed0: 2020 2020 636d 645b 2273 7461 7469 6f6e      cmd["station
-00007ee0: 225d 203d 2070 6c61 7466 6f72 6d2e 6e6f  "] = platform.no
-00007ef0: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
-00007f00: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
-00007f10: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
-00007f20: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
-00007f30: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00007f40: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-00007f50: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
-00007f60: 4b65 795f 446f 776e 3a0a 2020 2020 2020  Key_Down:.      
-00007f70: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
-00007f80: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00007f90: 636d 6422 5d20 3d20 224e 4558 5453 504f  cmd"] = "NEXTSPO
-00007fa0: 5422 0a20 2020 2020 2020 2020 2020 2063  T".            c
-00007fb0: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
-00007fc0: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
-00007fd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007fe0: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-00007ff0: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
-00008000: 6e28 636d 6429 0a20 2020 2020 2020 2020  n(cmd).         
-00008010: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00008020: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
-00008030: 203d 3d20 5174 2e4b 6579 2e4b 6579 5f50   == Qt.Key.Key_P
-00008040: 6167 6555 7020 616e 6420 6d6f 6469 6669  ageUp and modifi
-00008050: 6572 2021 3d20 5174 2e43 6f6e 7472 6f6c  er != Qt.Control
-00008060: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
-00008070: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
-00008080: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00008090: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000080a0: 6c66 2e63 772e 7370 6565 6420 2b3d 2031  lf.cw.speed += 1
-000080b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000080c0: 2073 656c 662e 6377 5f73 7065 6564 2e73   self.cw_speed.s
-000080d0: 6574 5661 6c75 6528 7365 6c66 2e63 772e  etValue(self.cw.
-000080e0: 7370 6565 6429 0a20 2020 2020 2020 2020  speed).         
-000080f0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00008100: 772e 7365 7276 6572 7479 7065 203d 3d20  w.servertype == 
-00008110: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-00008120: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-00008130: 656e 6463 7728 6622 5c78 3162 327b 7365  endcw(f"\x1b2{se
-00008140: 6c66 2e63 772e 7370 6565 647d 2229 0a20  lf.cw.speed}"). 
-00008150: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00008160: 6620 7365 6c66 2e63 772e 7365 7276 6572  f self.cw.server
-00008170: 7479 7065 203d 3d20 323a 0a20 2020 2020  type == 2:.     
-00008180: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00008190: 656c 662e 6377 2e73 6574 5f77 696e 6b65  elf.cw.set_winke
-000081a0: 7965 725f 7370 6565 6428 7365 6c66 2e63  yer_speed(self.c
-000081b0: 775f 7370 6565 642e 7661 6c75 6528 2929  w_speed.value())
-000081c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000081d0: 7572 6e0a 2020 2020 2020 2020 6966 2065  urn.        if e
-000081e0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
-000081f0: 2e4b 6579 2e4b 6579 5f50 6167 6544 6f77  .Key.Key_PageDow
-00008200: 6e20 616e 6420 6d6f 6469 6669 6572 2021  n and modifier !
-00008210: 3d20 5174 2e43 6f6e 7472 6f6c 4d6f 6469  = Qt.ControlModi
-00008220: 6669 6572 3a0a 2020 2020 2020 2020 2020  fier:.          
-00008230: 2020 6966 2073 656c 662e 6377 2069 7320    if self.cw is 
-00008240: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00008250: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00008260: 772e 7370 6565 6420 2d3d 2031 0a20 2020  w.speed -= 1.   
-00008270: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00008280: 662e 6377 5f73 7065 6564 2e73 6574 5661  f.cw_speed.setVa
-00008290: 6c75 6528 7365 6c66 2e63 772e 7370 6565  lue(self.cw.spee
-000082a0: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-000082b0: 2020 2069 6620 7365 6c66 2e63 772e 7365     if self.cw.se
-000082c0: 7276 6572 7479 7065 203d 3d20 313a 0a20  rvertype == 1:. 
-000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082e0: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
-000082f0: 7728 6622 5c78 3162 327b 7365 6c66 2e63  w(f"\x1b2{self.c
-00008300: 772e 7370 6565 647d 2229 0a20 2020 2020  w.speed}").     
-00008310: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00008320: 6c66 2e63 772e 7365 7276 6572 7479 7065  lf.cw.servertype
-00008330: 203d 3d20 323a 0a20 2020 2020 2020 2020   == 2:.         
-00008340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008350: 6377 2e73 6574 5f77 696e 6b65 7965 725f  cw.set_winkeyer_
-00008360: 7370 6565 6428 7365 6c66 2e63 775f 7370  speed(self.cw_sp
-00008370: 6565 642e 7661 6c75 6528 2929 0a20 2020  eed.value()).   
-00008380: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00008390: 2020 2020 2020 2020 2320 6966 2065 7665          # if eve
-000083a0: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
-000083b0: 6579 2e4b 6579 5f45 6e74 6572 3a0a 2020  ey.Key_Enter:.  
-000083c0: 2020 2020 2020 2320 2020 2020 7365 6c66        #     self
-000083d0: 2e73 6176 655f 636f 6e74 6163 7428 290a  .save_contact().
-000083e0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-000083f0: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-00008400: 2e4b 6579 5f54 6162 206f 7220 6576 656e  .Key_Tab or even
-00008410: 742e 6b65 7928 2920 3d3d 2051 742e 4b65  t.key() == Qt.Ke
-00008420: 792e 4b65 795f 4261 636b 7461 623a 0a20  y.Key_Backtab:. 
-00008430: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00008440: 6c66 2e73 656e 742e 6861 7346 6f63 7573  lf.sent.hasFocus
-00008450: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00008460: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00008470: 2822 4672 6f6d 2073 656e 7422 290a 2020  ("From sent").  
-00008480: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00008490: 206d 6f64 6966 6965 7220 3d3d 2051 742e   modifier == Qt.
-000084a0: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
-000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084c0: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
-000084d0: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
-000084e0: 7365 6c66 2e73 656e 7429 0a20 2020 2020  self.sent).     
-000084f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00008500: 7265 765f 7461 622e 7365 7446 6f63 7573  rev_tab.setFocus
-00008510: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00008520: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-00008530: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
-00008540: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00008550: 7265 765f 7461 622e 656e 6428 4661 6c73  rev_tab.end(Fals
-00008560: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00008570: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00008580: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00008590: 745f 7461 6220 3d20 7365 6c66 2e74 6162  t_tab = self.tab
-000085a0: 5f6e 6578 742e 6765 7428 7365 6c66 2e73  _next.get(self.s
-000085b0: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
-000085c0: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-000085d0: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
-000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085f0: 206e 6578 745f 7461 622e 6465 7365 6c65   next_tab.desele
-00008600: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-00008610: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-00008620: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
-00008630: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00008640: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-00008650: 6966 2073 656c 662e 7265 6365 6976 652e  if self.receive.
-00008660: 6861 7346 6f63 7573 2829 3a0a 2020 2020  hasFocus():.    
-00008670: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00008680: 6572 2e64 6562 7567 2822 4672 6f6d 2072  er.debug("From r
-00008690: 6563 6569 7665 2229 0a20 2020 2020 2020  eceive").       
-000086a0: 2020 2020 2020 2020 2069 6620 6d6f 6469           if modi
-000086b0: 6669 6572 203d 3d20 5174 2e53 6869 6674  fier == Qt.Shift
-000086c0: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
-000086d0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000086e0: 6576 5f74 6162 203d 2073 656c 662e 7461  ev_tab = self.ta
-000086f0: 625f 7072 6576 2e67 6574 2873 656c 662e  b_prev.get(self.
-00008700: 7265 6365 6976 6529 0a20 2020 2020 2020  receive).       
-00008710: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00008720: 765f 7461 622e 7365 7446 6f63 7573 2829  v_tab.setFocus()
+00006030: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
+00006040: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
+00006050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006060: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
+00006070: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
+00006080: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
+00006090: 2020 2020 2020 2020 2020 2020 6966 2068              if h
+000060a0: 6173 6174 7472 2873 656c 662e 636f 6e74  asattr(self.cont
+000060b0: 6573 742c 2022 636f 6c75 6d6e 7322 293a  est, "columns"):
+000060c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000060d0: 2020 2020 2063 6d64 203d 207b 7d0a 2020       cmd = {}.  
+000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060f0: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
+00006100: 5348 4f57 434f 4c55 4d4e 5322 0a20 2020  SHOWCOLUMNS".   
+00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006120: 2063 6d64 5b22 7374 6174 696f 6e22 5d20   cmd["station"] 
+00006130: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
+00006140: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006150: 2020 2020 2020 636d 645b 2243 4f4c 554d        cmd["COLUM
+00006160: 4e53 225d 203d 2073 656c 662e 636f 6e74  NS"] = self.cont
+00006170: 6573 742e 636f 6c75 6d6e 730a 2020 2020  est.columns.    
+00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006190: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+000061a0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+000061b0: 5f6a 736f 6e28 636d 6429 0a0a 2020 2020  _json(cmd)..    
+000061c0: 6465 6620 6368 6563 6b5f 666f 725f 6e65  def check_for_ne
+000061d0: 775f 6374 7928 7365 6c66 293a 0a20 2020  w_cty(self):.   
+000061e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000061f0: 2043 6865 636b 7320 666f 7220 6120 6e65   Checks for a ne
+00006200: 7720 6374 792e 6461 7420 6669 6c65 2e0a  w cty.dat file..
+00006210: 2020 2020 2020 2020 4c6f 6164 7320 6974          Loads it
+00006220: 2069 6620 6176 6169 6c61 626c 652e 0a20   if available.. 
+00006230: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006240: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00006250: 2020 2020 6374 7920 3d20 6e6f 7463 7479      cty = notcty
+00006260: 7061 7273 6572 2e42 6967 4374 7928 574f  parser.BigCty(WO
+00006270: 524b 494e 475f 5041 5448 202b 2022 2f64  RKING_PATH + "/d
+00006280: 6174 612f 6374 792e 6a73 6f6e 2229 0a20  ata/cty.json"). 
+00006290: 2020 2020 2020 2020 2020 2075 7064 6174             updat
+000062a0: 655f 6176 6169 6c61 626c 6520 3d20 6374  e_available = ct
+000062b0: 792e 6368 6563 6b5f 7570 6461 7465 2829  y.check_update()
+000062c0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000062d0: 4578 6365 7074 696f 6e20 6173 2074 6865  Exception as the
+000062e0: 5f65 7272 6f72 3a0a 2020 2020 2020 2020  _error:.        
+000062f0: 2020 2020 6374 7920 3d20 4e6f 6e65 2020      cty = None  
+00006300: 2320 6672 6565 2075 7020 7468 6520 6d65  # free up the me
+00006310: 6d6f 7279 0a20 2020 2020 2020 2020 2020  mory.           
+00006320: 206c 6f67 6765 722e 6465 6275 6728 2263   logger.debug("c
+00006330: 7479 2070 6172 7365 7220 7265 7475 726e  ty parser return
+00006340: 6564 2061 6e20 6572 726f 723a 2025 7322  ed an error: %s"
+00006350: 2c20 7468 655f 6572 726f 7229 0a20 2020  , the_error).   
+00006360: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00006370: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00006380: 6562 7567 2822 4e65 7765 7220 6374 7920  ebug("Newer cty 
+00006390: 6669 6c65 2061 7661 696c 6162 6c65 2025  file available %
+000063a0: 7322 2c20 7374 7228 7570 6461 7465 5f61  s", str(update_a
+000063b0: 7661 696c 6162 6c65 2929 0a0a 2020 2020  vailable))..    
+000063c0: 2020 2020 6966 2075 7064 6174 655f 6176      if update_av
+000063d0: 6169 6c61 626c 653a 0a20 2020 2020 2020  ailable:.       
+000063e0: 2020 2020 2073 656c 662e 7368 6f77 5f6d       self.show_m
+000063f0: 6573 7361 6765 5f62 6f78 2822 5570 6461  essage_box("Upda
+00006400: 7469 6e67 2063 7479 2066 696c 652e 2e22  ting cty file.."
+00006410: 290a 2020 2020 2020 2020 2020 2020 7472  ).            tr
+00006420: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00006430: 2020 2075 7064 6174 6564 203d 2063 7479     updated = cty
+00006440: 2e75 7064 6174 6528 290a 2020 2020 2020  .update().      
+00006450: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00006460: 6570 7469 6f6e 2061 7320 7468 655f 6572  eption as the_er
+00006470: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+00006480: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00006490: 6728 2263 7479 2070 6172 7365 7220 7265  g("cty parser re
+000064a0: 7475 726e 6564 2061 6e20 6572 726f 723a  turned an error:
+000064b0: 2025 7322 2c20 7468 655f 6572 726f 7229   %s", the_error)
+000064c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000064d0: 2063 7479 203d 204e 6f6e 6520 2023 2066   cty = None  # f
+000064e0: 7265 6520 7570 2074 6865 206d 656d 6f72  ree up the memor
+000064f0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+00006500: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00006510: 2020 2020 2069 6620 7570 6461 7465 643a       if updated:
+00006520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006530: 2063 7479 2e64 756d 7028 574f 524b 494e   cty.dump(WORKIN
+00006540: 475f 5041 5448 202b 2022 2f64 6174 612f  G_PATH + "/data/
+00006550: 6374 792e 6a73 6f6e 2229 0a20 2020 2020  cty.json").     
+00006560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006570: 7368 6f77 5f6d 6573 7361 6765 5f62 6f78  show_message_box
+00006580: 2822 6374 7920 6669 6c65 2075 7064 6174  ("cty file updat
+00006590: 6564 2e22 290a 2020 2020 2020 2020 2020  ed.").          
+000065a0: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+000065b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000065c0: 2020 2020 2057 4f52 4b49 4e47 5f50 4154       WORKING_PAT
+000065d0: 4820 2b20 222f 6461 7461 2f63 7479 2e6a  H + "/data/cty.j
+000065e0: 736f 6e22 2c20 2272 7422 2c20 656e 636f  son", "rt", enco
+000065f0: 6469 6e67 3d22 7574 662d 3822 0a20 2020  ding="utf-8".   
+00006600: 2020 2020 2020 2020 2020 2020 2029 2061               ) a
+00006610: 7320 635f 6669 6c65 3a0a 2020 2020 2020  s c_file:.      
+00006620: 2020 2020 2020 2020 2020 2020 2020 676c                gl
+00006630: 6f62 616c 7328 295b 2243 5459 4649 4c45  obals()["CTYFILE
+00006640: 225d 203d 206c 6f61 6473 2863 5f66 696c  "] = loads(c_fil
+00006650: 652e 7265 6164 2829 290a 2020 2020 2020  e.read()).      
+00006660: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00006670: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006680: 2e73 686f 775f 6d65 7373 6167 655f 626f  .show_message_bo
+00006690: 7828 2241 6e20 4572 726f 7220 6f63 6375  x("An Error occu
+000066a0: 7265 6420 7570 6461 7469 6e67 2066 696c  red updating fil
+000066b0: 652e 2229 0a20 2020 2020 2020 2063 7479  e.").        cty
+000066c0: 203d 204e 6f6e 6520 2023 2066 7265 6520   = None  # free 
+000066d0: 7570 2074 6865 206d 656d 6f72 790a 0a20  up the memory.. 
+000066e0: 2020 2064 6566 2068 6964 655f 6261 6e64     def hide_band
+000066f0: 5f6d 6f64 6528 7365 6c66 2c20 7468 655f  _mode(self, the_
+00006700: 6d6f 6465 3a20 7374 7229 202d 3e20 4e6f  mode: str) -> No
+00006710: 6e65 3a0a 2020 2020 2020 2020 2222 2268  ne:.        """h
+00006720: 6964 6522 2222 0a20 2020 2020 2020 206c  ide""".        l
+00006730: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
+00006740: 2c20 6622 7b74 6865 5f6d 6f64 657d 2229  , f"{the_mode}")
+00006750: 0a20 2020 2020 2020 2073 656c 662e 4261  .        self.Ba
+00006760: 6e64 5f4d 6f64 655f 4672 616d 655f 4357  nd_Mode_Frame_CW
+00006770: 2e68 6964 6528 290a 2020 2020 2020 2020  .hide().        
+00006780: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
+00006790: 7261 6d65 5f53 5342 2e68 6964 6528 290a  rame_SSB.hide().
+000067a0: 2020 2020 2020 2020 7365 6c66 2e42 616e          self.Ban
+000067b0: 645f 4d6f 6465 5f46 7261 6d65 5f52 5454  d_Mode_Frame_RTT
+000067c0: 592e 6869 6465 2829 0a20 2020 2020 2020  Y.hide().       
+000067d0: 206d 6f64 6573 203d 207b 0a20 2020 2020   modes = {.     
+000067e0: 2020 2020 2020 2022 4357 223a 2028 7365         "CW": (se
+000067f0: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
+00006800: 6d65 5f43 572c 292c 0a20 2020 2020 2020  me_CW,),.       
+00006810: 2020 2020 2022 5353 4222 3a20 2873 656c       "SSB": (sel
+00006820: 662e 4261 6e64 5f4d 6f64 655f 4672 616d  f.Band_Mode_Fram
+00006830: 655f 5353 422c 292c 0a20 2020 2020 2020  e_SSB,),.       
+00006840: 2020 2020 2022 5254 5459 223a 2028 7365       "RTTY": (se
+00006850: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
+00006860: 6d65 5f52 5454 592c 292c 0a20 2020 2020  me_RTTY,),.     
+00006870: 2020 2020 2020 2022 5053 4b22 3a20 2873         "PSK": (s
+00006880: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
+00006890: 616d 655f 5254 5459 2c29 2c0a 2020 2020  ame_RTTY,),.    
+000068a0: 2020 2020 2020 2020 2253 5342 2b43 5722          "SSB+CW"
+000068b0: 3a20 2873 656c 662e 4261 6e64 5f4d 6f64  : (self.Band_Mod
+000068c0: 655f 4672 616d 655f 4357 2c20 7365 6c66  e_Frame_CW, self
+000068d0: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
+000068e0: 5f53 5342 292c 0a20 2020 2020 2020 2020  _SSB),.         
+000068f0: 2020 2022 424f 5448 223a 2028 7365 6c66     "BOTH": (self
+00006900: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
+00006910: 5f43 572c 2073 656c 662e 4261 6e64 5f4d  _CW, self.Band_M
+00006920: 6f64 655f 4672 616d 655f 5353 4229 2c0a  ode_Frame_SSB),.
+00006930: 2020 2020 2020 2020 2020 2020 2244 4947              "DIG
+00006940: 4954 414c 223a 2028 7365 6c66 2e42 616e  ITAL": (self.Ban
+00006950: 645f 4d6f 6465 5f46 7261 6d65 5f52 5454  d_Mode_Frame_RTT
+00006960: 592c 292c 0a20 2020 2020 2020 2020 2020  Y,),.           
+00006970: 2022 5353 422b 4357 2b44 4947 4954 414c   "SSB+CW+DIGITAL
+00006980: 223a 2028 0a20 2020 2020 2020 2020 2020  ": (.           
+00006990: 2020 2020 2073 656c 662e 4261 6e64 5f4d       self.Band_M
+000069a0: 6f64 655f 4672 616d 655f 5254 5459 2c0a  ode_Frame_RTTY,.
+000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069c0: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
+000069d0: 7261 6d65 5f43 572c 0a20 2020 2020 2020  rame_CW,.       
+000069e0: 2020 2020 2020 2020 2073 656c 662e 4261           self.Ba
+000069f0: 6e64 5f4d 6f64 655f 4672 616d 655f 5353  nd_Mode_Frame_SS
+00006a00: 422c 0a20 2020 2020 2020 2020 2020 2029  B,.            )
+00006a10: 2c0a 2020 2020 2020 2020 2020 2020 2246  ,.            "F
+00006a20: 4d22 3a20 2873 656c 662e 4261 6e64 5f4d  M": (self.Band_M
+00006a30: 6f64 655f 4672 616d 655f 5353 422c 292c  ode_Frame_SSB,),
+00006a40: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00006a50: 2020 2066 7261 6d65 7320 3d20 6d6f 6465     frames = mode
+00006a60: 732e 6765 7428 7468 655f 6d6f 6465 290a  s.get(the_mode).
+00006a70: 2020 2020 2020 2020 6966 2066 7261 6d65          if frame
+00006a80: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
+00006a90: 6f72 2066 7261 6d65 2069 6e20 6672 616d  or frame in fram
+00006aa0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00006ab0: 2020 2020 6672 616d 652e 7368 6f77 2829      frame.show()
+00006ac0: 0a0a 2020 2020 6465 6620 6669 6c65 7069  ..    def filepi
+00006ad0: 636b 6572 2873 656c 662c 2061 6374 696f  cker(self, actio
+00006ae0: 6e3a 2073 7472 2920 2d3e 2073 7472 3a0a  n: str) -> str:.
+00006af0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006b00: 2020 2020 4765 7420 6120 6669 6c65 6e61      Get a filena
+00006b10: 6d65 0a20 2020 2020 2020 2061 6374 696f  me.        actio
+00006b20: 6e3a 2022 6e65 7722 206f 7220 226f 7065  n: "new" or "ope
+00006b30: 6e22 0a20 2020 2020 2020 2022 2222 0a20  n".        """. 
+00006b40: 2020 2020 2020 206f 7074 696f 6e73 203d         options =
+00006b50: 2051 4669 6c65 4469 616c 6f67 2e4f 7074   QFileDialog.Opt
+00006b60: 696f 6e73 2829 0a20 2020 2020 2020 206f  ions().        o
+00006b70: 7074 696f 6e73 207c 3d20 5146 696c 6544  ptions |= QFileD
+00006b80: 6961 6c6f 672e 446f 6e74 5573 654e 6174  ialog.DontUseNat
+00006b90: 6976 6544 6961 6c6f 670a 2020 2020 2020  iveDialog.      
+00006ba0: 2020 6f70 7469 6f6e 7320 7c3d 2051 4669    options |= QFi
+00006bb0: 6c65 4469 616c 6f67 2e44 6f6e 7443 6f6e  leDialog.DontCon
+00006bc0: 6669 726d 4f76 6572 7772 6974 650a 2020  firmOverwrite.  
+00006bd0: 2020 2020 2020 6966 2061 6374 696f 6e20        if action 
+00006be0: 3d3d 2022 6e65 7722 3a0a 2020 2020 2020  == "new":.      
+00006bf0: 2020 2020 2020 6669 6c65 2c20 5f20 3d20        file, _ = 
+00006c00: 5146 696c 6544 6961 6c6f 672e 6765 7453  QFileDialog.getS
+00006c10: 6176 6546 696c 654e 616d 6528 0a20 2020  aveFileName(.   
+00006c20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006c30: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+00006c40: 2020 2022 4368 6f6f 7365 2061 2044 6174     "Choose a Dat
+00006c50: 6162 6173 6522 2c0a 2020 2020 2020 2020  abase",.        
+00006c60: 2020 2020 2020 2020 4441 5441 5f50 4154          DATA_PAT
+00006c70: 482c 0a20 2020 2020 2020 2020 2020 2020  H,.             
+00006c80: 2020 2022 4461 7461 6261 7365 2028 2a2e     "Database (*.
+00006c90: 6462 2922 2c0a 2020 2020 2020 2020 2020  db)",.          
+00006ca0: 2020 2020 2020 6f70 7469 6f6e 733d 6f70        options=op
+00006cb0: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
+00006cc0: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00006cd0: 6163 7469 6f6e 203d 3d20 226f 7065 6e22  action == "open"
+00006ce0: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
+00006cf0: 6c65 2c20 5f20 3d20 5146 696c 6544 6961  le, _ = QFileDia
+00006d00: 6c6f 672e 6765 744f 7065 6e46 696c 654e  log.getOpenFileN
+00006d10: 616d 6528 0a20 2020 2020 2020 2020 2020  ame(.           
+00006d20: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00006d30: 2020 2020 2020 2020 2020 2022 4368 6f6f             "Choo
+00006d40: 7365 2061 2044 6174 6162 6173 6522 2c0a  se a Database",.
+00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d60: 4441 5441 5f50 4154 482c 0a20 2020 2020  DATA_PATH,.     
+00006d70: 2020 2020 2020 2020 2020 2022 4461 7461             "Data
+00006d80: 6261 7365 2028 2a2e 6462 2922 2c0a 2020  base (*.db)",.  
+00006d90: 2020 2020 2020 2020 2020 2020 2020 6f70                op
+00006da0: 7469 6f6e 733d 6f70 7469 6f6e 732c 0a20  tions=options,. 
+00006db0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00006dc0: 2020 2020 2072 6574 7572 6e20 6669 6c65       return file
+00006dd0: 0a0a 2020 2020 6465 6620 7265 6361 6c63  ..    def recalc
+00006de0: 756c 6174 655f 6d75 6c74 7328 7365 6c66  ulate_mults(self
+00006df0: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+00006e00: 6361 6c63 756c 6174 6520 4d75 6c74 6970  calculate Multip
+00006e10: 6c69 6572 7322 2222 0a20 2020 2020 2020  liers""".       
+00006e20: 2073 656c 662e 636f 6e74 6573 742e 7265   self.contest.re
+00006e30: 6361 6c63 756c 6174 655f 6d75 6c74 7328  calculate_mults(
+00006e40: 7365 6c66 290a 0a20 2020 2064 6566 206c  self)..    def l
+00006e50: 6175 6e63 685f 6c6f 675f 7769 6e64 6f77  aunch_log_window
+00006e60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00006e70: 2222 226c 6175 6e63 6820 7468 6520 4c6f  """launch the Lo
+00006e80: 6720 5769 6e64 6f77 2222 220a 2020 2020  g Window""".    
+00006e90: 2020 2020 6966 206e 6f74 2063 6865 636b      if not check
+00006ea0: 5f70 726f 6365 7373 2822 6c6f 6777 696e  _process("logwin
+00006eb0: 646f 772e 7079 2229 3a0a 2020 2020 2020  dow.py"):.      
+00006ec0: 2020 2020 2020 5f20 3d20 7375 6270 726f        _ = subpro
+00006ed0: 6365 7373 2e50 6f70 656e 285b 7379 732e  cess.Popen([sys.
+00006ee0: 6578 6563 7574 6162 6c65 2c20 574f 524b  executable, WORK
+00006ef0: 494e 475f 5041 5448 202b 2022 2f6c 6f67  ING_PATH + "/log
+00006f00: 7769 6e64 6f77 2e70 7922 5d29 0a0a 2020  window.py"])..  
+00006f10: 2020 6465 6620 6c61 756e 6368 5f62 616e    def launch_ban
+00006f20: 646d 6170 5f77 696e 646f 7728 7365 6c66  dmap_window(self
+00006f30: 293a 0a20 2020 2020 2020 2022 2222 6c61  ):.        """la
+00006f40: 756e 6368 2074 6865 204c 6f67 2057 696e  unch the Log Win
+00006f50: 646f 7722 2222 0a20 2020 2020 2020 2069  dow""".        i
+00006f60: 6620 6e6f 7420 6368 6563 6b5f 7072 6f63  f not check_proc
+00006f70: 6573 7328 2262 616e 646d 6170 2e70 7922  ess("bandmap.py"
+00006f80: 293a 0a20 2020 2020 2020 2020 2020 205f  ):.            _
+00006f90: 203d 2073 7562 7072 6f63 6573 732e 506f   = subprocess.Po
+00006fa0: 7065 6e28 5b73 7973 2e65 7865 6375 7461  pen([sys.executa
+00006fb0: 626c 652c 2057 4f52 4b49 4e47 5f50 4154  ble, WORKING_PAT
+00006fc0: 4820 2b20 222f 6261 6e64 6d61 702e 7079  H + "/bandmap.py
+00006fd0: 225d 290a 0a20 2020 2064 6566 2063 6c65  "])..    def cle
+00006fe0: 6172 5f62 616e 645f 696e 6469 6361 746f  ar_band_indicato
+00006ff0: 7273 2873 656c 6629 3a0a 2020 2020 2020  rs(self):.      
+00007000: 2020 2222 2243 6c65 6172 2074 6865 2069    """Clear the i
+00007010: 6e64 6963 6174 6f72 7322 2222 0a20 2020  ndicators""".   
+00007020: 2020 2020 2066 6f72 205f 2c20 696e 6469       for _, indi
+00007030: 6361 746f 7273 2069 6e20 7365 6c66 2e61  cators in self.a
+00007040: 6c6c 5f6d 6f64 655f 696e 6469 6361 746f  ll_mode_indicato
+00007050: 7273 2e69 7465 6d73 2829 3a0a 2020 2020  rs.items():.    
+00007060: 2020 2020 2020 2020 666f 7220 5f2c 2069          for _, i
+00007070: 6e64 6963 6174 6f72 2069 6e20 696e 6469  ndicator in indi
+00007080: 6361 746f 7273 2e69 7465 6d73 2829 3a0a  cators.items():.
+00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070a0: 696e 6469 6361 746f 722e 7365 7446 7261  indicator.setFra
+000070b0: 6d65 5368 6170 6528 5174 5769 6467 6574  meShape(QtWidget
+000070c0: 732e 5146 7261 6d65 2e4e 6f46 7261 6d65  s.QFrame.NoFrame
+000070d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000070e0: 2020 696e 6469 6361 746f 722e 7365 7453    indicator.setS
+000070f0: 7479 6c65 5368 6565 7428 2266 6f6e 742d  tyleSheet("font-
+00007100: 6661 6d69 6c79 3a20 4a65 7442 7261 696e  family: JetBrain
+00007110: 7320 4d6f 6e6f 3b22 290a 0a20 2020 2064  s Mono;")..    d
+00007120: 6566 2073 6574 5f62 616e 645f 696e 6469  ef set_band_indi
+00007130: 6361 746f 7228 7365 6c66 2c20 6261 6e64  cator(self, band
+00007140: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
+00007150: 2020 2020 2020 2020 2222 2253 6574 2074          """Set t
+00007160: 6865 2062 616e 6420 696e 6469 6361 746f  he band indicato
+00007170: 7222 2222 0a20 2020 2020 2020 2023 206c  r""".        # l
+00007180: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
+00007190: 2c20 6622 6261 6e64 3a7b 6261 6e64 7d20  , f"band:{band} 
+000071a0: 6d6f 6465 3a20 7b73 656c 662e 6375 7272  mode: {self.curr
+000071b0: 656e 745f 6d6f 6465 7d22 290a 2020 2020  ent_mode}").    
+000071c0: 2020 2020 6966 2062 616e 6420 616e 6420      if band and 
+000071d0: 7365 6c66 2e63 7572 7265 6e74 5f6d 6f64  self.current_mod
+000071e0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000071f0: 656c 662e 636c 6561 725f 6261 6e64 5f69  elf.clear_band_i
+00007200: 6e64 6963 6174 6f72 7328 290a 2020 2020  ndicators().    
+00007210: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
+00007220: 7220 3d20 7365 6c66 2e61 6c6c 5f6d 6f64  r = self.all_mod
+00007230: 655f 696e 6469 6361 746f 7273 5b73 656c  e_indicators[sel
+00007240: 662e 6375 7272 656e 745f 6d6f 6465 5d2e  f.current_mode].
+00007250: 6765 7428 6261 6e64 2c20 4e6f 6e65 290a  get(band, None).
+00007260: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00007270: 6e64 6963 6174 6f72 3a0a 2020 2020 2020  ndicator:.      
+00007280: 2020 2020 2020 2020 2020 696e 6469 6361            indica
+00007290: 746f 722e 7365 7446 7261 6d65 5368 6170  tor.setFrameShap
+000072a0: 6528 5174 5769 6467 6574 732e 5146 7261  e(QtWidgets.QFra
+000072b0: 6d65 2e42 6f78 290a 2020 2020 2020 2020  me.Box).        
+000072c0: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
+000072d0: 722e 7365 7453 7479 6c65 5368 6565 7428  r.setStyleSheet(
+000072e0: 2266 6f6e 742d 6661 6d69 6c79 3a20 4a65  "font-family: Je
+000072f0: 7442 7261 696e 7320 4d6f 6e6f 3b20 636f  tBrains Mono; co
+00007300: 6c6f 723a 2067 7265 656e 3b22 290a 0a20  lor: green;").. 
+00007310: 2020 2064 6566 2063 6c6f 7365 4576 656e     def closeEven
+00007320: 7428 7365 6c66 2c20 5f65 7665 6e74 293a  t(self, _event):
+00007330: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007340: 2020 2020 2057 7269 7465 2077 696e 646f       Write windo
+00007350: 7720 7369 7a65 2061 6e64 2070 6f73 6974  w size and posit
+00007360: 696f 6e20 746f 2063 6f6e 6669 6720 6669  ion to config fi
+00007370: 6c65 0a20 2020 2020 2020 2022 2222 0a20  le.        """. 
+00007380: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+00007390: 5b22 7769 6e64 6f77 5f77 6964 7468 225d  ["window_width"]
+000073a0: 203d 2073 656c 662e 7369 7a65 2829 2e77   = self.size().w
+000073b0: 6964 7468 2829 0a20 2020 2020 2020 2073  idth().        s
+000073c0: 656c 662e 7072 6566 5b22 7769 6e64 6f77  elf.pref["window
+000073d0: 5f68 6569 6768 7422 5d20 3d20 7365 6c66  _height"] = self
+000073e0: 2e73 697a 6528 292e 6865 6967 6874 2829  .size().height()
+000073f0: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
+00007400: 6566 5b22 7769 6e64 6f77 5f78 225d 203d  ef["window_x"] =
+00007410: 2073 656c 662e 706f 7328 292e 7828 290a   self.pos().x().
+00007420: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+00007430: 665b 2277 696e 646f 775f 7922 5d20 3d20  f["window_y"] = 
+00007440: 7365 6c66 2e70 6f73 2829 2e79 2829 0a20  self.pos().y(). 
+00007450: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
+00007460: 655f 7072 6566 6572 656e 6365 2829 0a0a  e_preference()..
+00007470: 2020 2020 6465 6620 6374 795f 6c6f 6f6b      def cty_look
+00007480: 7570 2873 656c 662c 2063 616c 6c73 6967  up(self, callsig
+00007490: 6e3a 2073 7472 293a 0a20 2020 2020 2020  n: str):.       
+000074a0: 2022 2222 4c6f 6f6b 7570 2063 616c 6c73   """Lookup calls
+000074b0: 6967 6e20 696e 2063 7479 2e64 6174 2066  ign in cty.dat f
+000074c0: 696c 6522 2222 0a20 2020 2020 2020 2063  ile""".        c
+000074d0: 616c 6c73 6967 6e20 3d20 6361 6c6c 7369  allsign = callsi
+000074e0: 676e 2e75 7070 6572 2829 0a20 2020 2020  gn.upper().     
+000074f0: 2020 2066 6f72 2063 6f75 6e74 2069 6e20     for count in 
+00007500: 7265 7665 7273 6564 2872 616e 6765 286c  reversed(range(l
+00007510: 656e 2863 616c 6c73 6967 6e29 2929 3a0a  en(callsign))):.
+00007520: 2020 2020 2020 2020 2020 2020 7365 6172              sear
+00007530: 6368 6974 656d 203d 2063 616c 6c73 6967  chitem = callsig
+00007540: 6e5b 3a20 636f 756e 7420 2b20 315d 0a20  n[: count + 1]. 
+00007550: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00007560: 7420 3d20 7b6b 6579 3a20 7661 6c20 666f  t = {key: val fo
+00007570: 7220 6b65 792c 2076 616c 2069 6e20 4354  r key, val in CT
+00007580: 5946 494c 452e 6974 656d 7328 2920 6966  YFILE.items() if
+00007590: 206b 6579 203d 3d20 7365 6172 6368 6974   key == searchit
+000075a0: 656d 7d0a 2020 2020 2020 2020 2020 2020  em}.            
+000075b0: 6966 206e 6f74 2072 6573 756c 743a 0a20  if not result:. 
+000075c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000075d0: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+000075e0: 2020 2020 6966 2072 6573 756c 742e 6765      if result.ge
+000075f0: 7428 7365 6172 6368 6974 656d 292e 6765  t(searchitem).ge
+00007600: 7428 2265 7861 6374 5f6d 6174 6368 2229  t("exact_match")
+00007610: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007620: 2020 6966 2073 6561 7263 6869 7465 6d20    if searchitem 
+00007630: 3d3d 2063 616c 6c73 6967 6e3a 0a20 2020  == callsign:.   
+00007640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007650: 2072 6574 7572 6e20 7265 7375 6c74 0a20   return result. 
+00007660: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00007670: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+00007680: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00007690: 740a 0a20 2020 2064 6566 2063 7773 7065  t..    def cwspe
+000076a0: 6564 5f73 7069 6e62 6f78 5f63 6861 6e67  ed_spinbox_chang
+000076b0: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
+000076c0: 2020 2222 2274 7269 6767 6572 6564 2077    """triggered w
+000076d0: 6865 6e20 7661 6c75 6520 6f66 2043 5720  hen value of CW 
+000076e0: 7370 6565 6420 696e 2074 6865 2073 7069  speed in the spi
+000076f0: 6e62 6f78 2063 6861 6e67 6573 2e22 2222  nbox changes."""
+00007700: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00007710: 2e63 772e 7365 7276 6572 7479 7065 203d  .cw.servertype =
+00007720: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+00007730: 2073 656c 662e 6377 2e73 7065 6564 203d   self.cw.speed =
+00007740: 2073 656c 662e 6377 5f73 7065 6564 2e76   self.cw_speed.v
+00007750: 616c 7565 2829 0a20 2020 2020 2020 2020  alue().         
+00007760: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
+00007770: 7728 6622 5c78 3162 327b 7365 6c66 2e63  w(f"\x1b2{self.c
+00007780: 772e 7370 6565 647d 2229 0a20 2020 2020  w.speed}").     
+00007790: 2020 2069 6620 7365 6c66 2e63 772e 7365     if self.cw.se
+000077a0: 7276 6572 7479 7065 203d 3d20 323a 0a20  rvertype == 2:. 
+000077b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000077c0: 6377 2e73 6574 5f77 696e 6b65 7965 725f  cw.set_winkeyer_
+000077d0: 7370 6565 6428 7365 6c66 2e63 775f 7370  speed(self.cw_sp
+000077e0: 6565 642e 7661 6c75 6528 2929 0a0a 2020  eed.value())..  
+000077f0: 2020 6465 6620 6b65 7950 7265 7373 4576    def keyPressEv
+00007800: 656e 7428 7365 6c66 2c20 6576 656e 7429  ent(self, event)
+00007810: 3a20 2023 2070 796c 696e 743a 2064 6973  :  # pylint: dis
+00007820: 6162 6c65 3d69 6e76 616c 6964 2d6e 616d  able=invalid-nam
+00007830: 650a 2020 2020 2020 2020 2222 2254 6869  e.        """Thi
+00007840: 7320 6f76 6572 7269 6465 7320 5174 206b  s overrides Qt k
+00007850: 6579 2065 7665 6e74 2e22 2222 0a20 2020  ey event.""".   
+00007860: 2020 2020 206d 6f64 6966 6965 7220 3d20       modifier = 
+00007870: 6576 656e 742e 6d6f 6469 6669 6572 7328  event.modifiers(
+00007880: 290a 2020 2020 2020 2020 6966 2065 7665  ).        if eve
+00007890: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
+000078a0: 6579 5f53 2061 6e64 206d 6f64 6966 6965  ey_S and modifie
+000078b0: 7220 3d3d 2051 742e 436f 6e74 726f 6c4d  r == Qt.ControlM
+000078c0: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
+000078d0: 2020 2020 2066 7265 7120 3d20 7365 6c66       freq = self
+000078e0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+000078f0: 2822 7666 6f61 2229 0a20 2020 2020 2020  ("vfoa").       
+00007900: 2020 2020 2064 7820 3d20 7365 6c66 2e63       dx = self.c
+00007910: 616c 6c73 6967 6e2e 7465 7874 2829 0a20  allsign.text(). 
+00007920: 2020 2020 2020 2020 2020 2069 6620 6672             if fr
+00007930: 6571 2061 6e64 2064 783a 0a20 2020 2020  eq and dx:.     
+00007940: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+00007950: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+00007960: 2020 2020 636d 645b 2263 6d64 225d 203d      cmd["cmd"] =
+00007970: 2022 5350 4f54 4458 220a 2020 2020 2020   "SPOTDX".      
+00007980: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
+00007990: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+000079a0: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+000079b0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+000079c0: 6478 225d 203d 2064 780a 2020 2020 2020  dx"] = dx.      
+000079d0: 2020 2020 2020 2020 2020 636d 645b 2266            cmd["f
+000079e0: 7265 7122 5d20 3d20 666c 6f61 7428 696e  req"] = float(in
+000079f0: 7428 6672 6571 2920 2f20 3130 3030 290a  t(freq) / 1000).
+00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a10: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+00007a20: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+00007a30: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+00007a40: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00007a50: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
+00007a60: 6579 2829 203d 3d20 5174 2e4b 6579 5f47  ey() == Qt.Key_G
+00007a70: 2061 6e64 206d 6f64 6966 6965 7220 3d3d   and modifier ==
+00007a80: 2051 742e 436f 6e74 726f 6c4d 6f64 6966   Qt.ControlModif
+00007a90: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
+00007aa0: 2064 7820 3d20 7365 6c66 2e63 616c 6c73   dx = self.calls
+00007ab0: 6967 6e2e 7465 7874 2829 0a20 2020 2020  ign.text().     
+00007ac0: 2020 2020 2020 2069 6620 6478 3a0a 2020         if dx:.  
+00007ad0: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00007ae0: 6420 3d20 7b7d 0a20 2020 2020 2020 2020  d = {}.         
+00007af0: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
+00007b00: 5d20 3d20 2246 494e 4444 5822 0a20 2020  ] = "FINDDX".   
+00007b10: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+00007b20: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
+00007b30: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
+00007b40: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00007b50: 645b 2264 7822 5d20 3d20 6478 0a20 2020  d["dx"] = dx.   
+00007b60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007b70: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
+00007b80: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
+00007b90: 6f6e 2863 6d64 290a 2020 2020 2020 2020  on(cmd).        
+00007ba0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00007bb0: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+00007bc0: 2020 2020 6576 656e 742e 6b65 7928 2920      event.key() 
+00007bd0: 3d3d 2051 742e 4b65 792e 4b65 795f 4573  == Qt.Key.Key_Es
+00007be0: 6361 7065 2061 6e64 206d 6f64 6966 6965  cape and modifie
+00007bf0: 7220 213d 2051 742e 436f 6e74 726f 6c4d  r != Qt.ControlM
+00007c00: 6f64 6966 6965 720a 2020 2020 2020 2020  odifier.        
+00007c10: 293a 2020 2320 7079 6c69 6e74 3a20 6469  ):  # pylint: di
+00007c20: 7361 626c 653d 6e6f 2d6d 656d 6265 720a  sable=no-member.
+00007c30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007c40: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
+00007c50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007c60: 6e0a 2020 2020 2020 2020 6966 2065 7665  n.        if eve
+00007c70: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
+00007c80: 6579 2e4b 6579 5f45 7363 6170 6520 616e  ey.Key_Escape an
+00007c90: 6420 6d6f 6469 6669 6572 203d 3d20 5174  d modifier == Qt
+00007ca0: 2e43 6f6e 7472 6f6c 4d6f 6469 6669 6572  .ControlModifier
+00007cb0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00007cc0: 2073 656c 662e 6377 2069 7320 6e6f 7420   self.cw is not 
+00007cd0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00007ce0: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+00007cf0: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
+00007d00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007d10: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+00007d20: 6e64 6377 2822 5c78 3162 3422 290a 2020  ndcw("\x1b4").  
+00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d40: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00007d50: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+00007d60: 3d3d 2051 742e 4b65 792e 4b65 795f 5570  == Qt.Key.Key_Up
+00007d70: 3a0a 2020 2020 2020 2020 2020 2020 636d  :.            cm
+00007d80: 6420 3d20 7b7d 0a20 2020 2020 2020 2020  d = {}.         
+00007d90: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
+00007da0: 2250 5245 5653 504f 5422 0a20 2020 2020  "PREVSPOT".     
+00007db0: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
+00007dc0: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
+00007dd0: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
+00007de0: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
+00007df0: 7374 5f69 6e74 6572 6661 6365 2e73 656e  st_interface.sen
+00007e00: 645f 6173 5f6a 736f 6e28 636d 6429 0a20  d_as_json(cmd). 
+00007e10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007e20: 6e0a 2020 2020 2020 2020 6966 2065 7665  n.        if eve
+00007e30: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
+00007e40: 6579 2e4b 6579 5f44 6f77 6e3a 0a20 2020  ey.Key_Down:.   
+00007e50: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+00007e60: 7d0a 2020 2020 2020 2020 2020 2020 636d  }.            cm
+00007e70: 645b 2263 6d64 225d 203d 2022 4e45 5854  d["cmd"] = "NEXT
+00007e80: 5350 4f54 220a 2020 2020 2020 2020 2020  SPOT".          
+00007e90: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
+00007ea0: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
+00007eb0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00007ec0: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
+00007ed0: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
+00007ee0: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
+00007ef0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00007f00: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
+00007f10: 7928 2920 3d3d 2051 742e 4b65 792e 4b65  y() == Qt.Key.Ke
+00007f20: 795f 5061 6765 5570 2061 6e64 206d 6f64  y_PageUp and mod
+00007f30: 6966 6965 7220 213d 2051 742e 436f 6e74  ifier != Qt.Cont
+00007f40: 726f 6c4d 6f64 6966 6965 723a 0a20 2020  rolModifier:.   
+00007f50: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00007f60: 2e63 7720 6973 206e 6f74 204e 6f6e 653a  .cw is not None:
+00007f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007f80: 2073 656c 662e 6377 2e73 7065 6564 202b   self.cw.speed +
+00007f90: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00007fa0: 2020 2020 7365 6c66 2e63 775f 7370 6565      self.cw_spee
+00007fb0: 642e 7365 7456 616c 7565 2873 656c 662e  d.setValue(self.
+00007fc0: 6377 2e73 7065 6564 290a 2020 2020 2020  cw.speed).      
+00007fd0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00007fe0: 662e 6377 2e73 6572 7665 7274 7970 6520  f.cw.servertype 
+00007ff0: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
+00008000: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00008010: 772e 7365 6e64 6377 2866 225c 7831 6232  w.sendcw(f"\x1b2
+00008020: 7b73 656c 662e 6377 2e73 7065 6564 7d22  {self.cw.speed}"
+00008030: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008040: 2020 6966 2073 656c 662e 6377 2e73 6572    if self.cw.ser
+00008050: 7665 7274 7970 6520 3d3d 2032 3a0a 2020  vertype == 2:.  
+00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008070: 2020 7365 6c66 2e63 772e 7365 745f 7769    self.cw.set_wi
+00008080: 6e6b 6579 6572 5f73 7065 6564 2873 656c  nkeyer_speed(sel
+00008090: 662e 6377 5f73 7065 6564 2e76 616c 7565  f.cw_speed.value
+000080a0: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+000080b0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
+000080c0: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+000080d0: 2051 742e 4b65 792e 4b65 795f 5061 6765   Qt.Key.Key_Page
+000080e0: 446f 776e 2061 6e64 206d 6f64 6966 6965  Down and modifie
+000080f0: 7220 213d 2051 742e 436f 6e74 726f 6c4d  r != Qt.ControlM
+00008100: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
+00008110: 2020 2020 2069 6620 7365 6c66 2e63 7720       if self.cw 
+00008120: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00008130: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00008140: 662e 6377 2e73 7065 6564 202d 3d20 310a  f.cw.speed -= 1.
+00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008160: 7365 6c66 2e63 775f 7370 6565 642e 7365  self.cw_speed.se
+00008170: 7456 616c 7565 2873 656c 662e 6377 2e73  tValue(self.cw.s
+00008180: 7065 6564 290a 2020 2020 2020 2020 2020  peed).          
+00008190: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+000081a0: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
+000081b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000081c0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+000081d0: 6e64 6377 2866 225c 7831 6232 7b73 656c  ndcw(f"\x1b2{sel
+000081e0: 662e 6377 2e73 7065 6564 7d22 290a 2020  f.cw.speed}").  
+000081f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00008200: 2073 656c 662e 6377 2e73 6572 7665 7274   self.cw.servert
+00008210: 7970 6520 3d3d 2032 3a0a 2020 2020 2020  ype == 2:.      
+00008220: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008230: 6c66 2e63 772e 7365 745f 7769 6e6b 6579  lf.cw.set_winkey
+00008240: 6572 5f73 7065 6564 2873 656c 662e 6377  er_speed(self.cw
+00008250: 5f73 7065 6564 2e76 616c 7565 2829 290a  _speed.value()).
+00008260: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00008270: 726e 0a20 2020 2020 2020 2023 2069 6620  rn.        # if 
+00008280: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+00008290: 742e 4b65 792e 4b65 795f 456e 7465 723a  t.Key.Key_Enter:
+000082a0: 0a20 2020 2020 2020 2023 2020 2020 2073  .        #     s
+000082b0: 656c 662e 7361 7665 5f63 6f6e 7461 6374  elf.save_contact
+000082c0: 2829 0a20 2020 2020 2020 2069 6620 6576  ().        if ev
+000082d0: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
+000082e0: 4b65 792e 4b65 795f 5461 6220 6f72 2065  Key.Key_Tab or e
+000082f0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+00008300: 2e4b 6579 2e4b 6579 5f42 6163 6b74 6162  .Key.Key_Backtab
+00008310: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00008320: 2073 656c 662e 7365 6e74 2e68 6173 466f   self.sent.hasFo
+00008330: 6375 7328 293a 0a20 2020 2020 2020 2020  cus():.         
+00008340: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00008350: 6275 6728 2246 726f 6d20 7365 6e74 2229  bug("From sent")
+00008360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008370: 2069 6620 6d6f 6469 6669 6572 203d 3d20   if modifier == 
+00008380: 5174 2e53 6869 6674 4d6f 6469 6669 6572  Qt.ShiftModifier
+00008390: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000083a0: 2020 2020 2020 7072 6576 5f74 6162 203d        prev_tab =
+000083b0: 2073 656c 662e 7461 625f 7072 6576 2e67   self.tab_prev.g
+000083c0: 6574 2873 656c 662e 7365 6e74 290a 2020  et(self.sent).  
+000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083e0: 2020 7072 6576 5f74 6162 2e73 6574 466f    prev_tab.setFo
+000083f0: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
+00008400: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
+00008410: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
+00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008430: 2020 7072 6576 5f74 6162 2e65 6e64 2846    prev_tab.end(F
+00008440: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00008450: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008470: 6e65 7874 5f74 6162 203d 2073 656c 662e  next_tab = self.
+00008480: 7461 625f 6e65 7874 2e67 6574 2873 656c  tab_next.get(sel
+00008490: 662e 7365 6e74 290a 2020 2020 2020 2020  f.sent).        
+000084a0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+000084b0: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
+000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084d0: 2020 2020 6e65 7874 5f74 6162 2e64 6573      next_tab.des
+000084e0: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
+000084f0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00008500: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
+00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008520: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00008530: 2020 2069 6620 7365 6c66 2e72 6563 6569     if self.recei
+00008540: 7665 2e68 6173 466f 6375 7328 293a 0a20  ve.hasFocus():. 
+00008550: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00008560: 6f67 6765 722e 6465 6275 6728 2246 726f  ogger.debug("Fro
+00008570: 6d20 7265 6365 6976 6522 290a 2020 2020  m receive").    
+00008580: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00008590: 6f64 6966 6965 7220 3d3d 2051 742e 5368  odifier == Qt.Sh
+000085a0: 6966 744d 6f64 6966 6965 723a 0a20 2020  iftModifier:.   
+000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085c0: 2070 7265 765f 7461 6220 3d20 7365 6c66   prev_tab = self
+000085d0: 2e74 6162 5f70 7265 762e 6765 7428 7365  .tab_prev.get(se
+000085e0: 6c66 2e72 6563 6569 7665 290a 2020 2020  lf.receive).    
+000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008600: 7072 6576 5f74 6162 2e73 6574 466f 6375  prev_tab.setFocu
+00008610: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00008620: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+00008630: 2e64 6573 656c 6563 7428 290a 2020 2020  .deselect().    
+00008640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008650: 7072 6576 5f74 6162 2e65 6e64 2846 616c  prev_tab.end(Fal
+00008660: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+00008670: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008680: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00008690: 7874 5f74 6162 203d 2073 656c 662e 7461  xt_tab = self.ta
+000086a0: 625f 6e65 7874 2e67 6574 2873 656c 662e  b_next.get(self.
+000086b0: 7265 6365 6976 6529 0a20 2020 2020 2020  receive).       
+000086c0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+000086d0: 745f 7461 622e 7365 7446 6f63 7573 2829  t_tab.setFocus()
+000086e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000086f0: 2020 2020 206e 6578 745f 7461 622e 6465       next_tab.de
+00008700: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
+00008710: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00008720: 745f 7461 622e 656e 6428 4661 6c73 6529  t_tab.end(False)
 00008730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008740: 2020 2020 2070 7265 765f 7461 622e 6465       prev_tab.de
-00008750: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
-00008760: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00008770: 765f 7461 622e 656e 6428 4661 6c73 6529  v_tab.end(False)
-00008780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008790: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000087a0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-000087b0: 7461 6220 3d20 7365 6c66 2e74 6162 5f6e  tab = self.tab_n
-000087c0: 6578 742e 6765 7428 7365 6c66 2e72 6563  ext.get(self.rec
-000087d0: 6569 7665 290a 2020 2020 2020 2020 2020  eive).          
-000087e0: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-000087f0: 6162 2e73 6574 466f 6375 7328 290a 2020  ab.setFocus().  
-00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008810: 2020 6e65 7874 5f74 6162 2e64 6573 656c    next_tab.desel
-00008820: 6563 7428 290a 2020 2020 2020 2020 2020  ect().          
-00008830: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-00008840: 6162 2e65 6e64 2846 616c 7365 290a 2020  ab.end(False).  
-00008850: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00008860: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00008870: 2069 6620 7365 6c66 2e6f 7468 6572 5f31   if self.other_1
-00008880: 2e68 6173 466f 6375 7328 293a 0a20 2020  .hasFocus():.   
-00008890: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-000088a0: 6765 722e 6465 6275 6728 2246 726f 6d20  ger.debug("From 
-000088b0: 6f74 6865 725f 3122 290a 2020 2020 2020  other_1").      
-000088c0: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-000088d0: 6966 6965 7220 3d3d 2051 742e 5368 6966  ifier == Qt.Shif
-000088e0: 744d 6f64 6966 6965 723a 0a20 2020 2020  tModifier:.     
-000088f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00008900: 7265 765f 7461 6220 3d20 7365 6c66 2e74  rev_tab = self.t
-00008910: 6162 5f70 7265 762e 6765 7428 7365 6c66  ab_prev.get(self
-00008920: 2e6f 7468 6572 5f31 290a 2020 2020 2020  .other_1).      
-00008930: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00008940: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
+00008740: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00008750: 2020 2020 6966 2073 656c 662e 6f74 6865      if self.othe
+00008760: 725f 312e 6861 7346 6f63 7573 2829 3a0a  r_1.hasFocus():.
+00008770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008780: 6c6f 6767 6572 2e64 6562 7567 2822 4672  logger.debug("Fr
+00008790: 6f6d 206f 7468 6572 5f31 2229 0a20 2020  om other_1").   
+000087a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000087b0: 6d6f 6469 6669 6572 203d 3d20 5174 2e53  modifier == Qt.S
+000087c0: 6869 6674 4d6f 6469 6669 6572 3a0a 2020  hiftModifier:.  
+000087d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087e0: 2020 7072 6576 5f74 6162 203d 2073 656c    prev_tab = sel
+000087f0: 662e 7461 625f 7072 6576 2e67 6574 2873  f.tab_prev.get(s
+00008800: 656c 662e 6f74 6865 725f 3129 0a20 2020  elf.other_1).   
+00008810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008820: 2070 7265 765f 7461 622e 7365 7446 6f63   prev_tab.setFoc
+00008830: 7573 2829 0a20 2020 2020 2020 2020 2020  us().           
+00008840: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
+00008850: 622e 6465 7365 6c65 6374 2829 0a20 2020  b.deselect().   
+00008860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008870: 2070 7265 765f 7461 622e 656e 6428 4661   prev_tab.end(Fa
+00008880: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+00008890: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000088a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000088b0: 6578 745f 7461 6220 3d20 7365 6c66 2e74  ext_tab = self.t
+000088c0: 6162 5f6e 6578 742e 6765 7428 7365 6c66  ab_next.get(self
+000088d0: 2e6f 7468 6572 5f31 290a 2020 2020 2020  .other_1).      
+000088e0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+000088f0: 7874 5f74 6162 2e73 6574 466f 6375 7328  xt_tab.setFocus(
+00008900: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008910: 2020 2020 2020 6e65 7874 5f74 6162 2e64        next_tab.d
+00008920: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
+00008930: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00008940: 7874 5f74 6162 2e65 6e64 2846 616c 7365  xt_tab.end(False
 00008950: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008960: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
-00008970: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
-00008980: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00008990: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
-000089a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000089b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000089c0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-000089d0: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
-000089e0: 6e65 7874 2e67 6574 2873 656c 662e 6f74  next.get(self.ot
-000089f0: 6865 725f 3129 0a20 2020 2020 2020 2020  her_1).         
-00008a00: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00008a10: 7461 622e 7365 7446 6f63 7573 2829 0a20  tab.setFocus(). 
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a30: 2020 206e 6578 745f 7461 622e 6465 7365     next_tab.dese
-00008a40: 6c65 6374 2829 0a20 2020 2020 2020 2020  lect().         
-00008a50: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00008a60: 7461 622e 656e 6428 4661 6c73 6529 0a20  tab.end(False). 
-00008a70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00008a80: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-00008a90: 2020 6966 2073 656c 662e 6f74 6865 725f    if self.other_
-00008aa0: 322e 6861 7346 6f63 7573 2829 3a0a 2020  2.hasFocus():.  
-00008ab0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00008ac0: 6767 6572 2e64 6562 7567 2822 4672 6f6d  gger.debug("From
-00008ad0: 206f 7468 6572 5f32 2229 0a20 2020 2020   other_2").     
-00008ae0: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
-00008af0: 6469 6669 6572 203d 3d20 5174 2e53 6869  difier == Qt.Shi
-00008b00: 6674 4d6f 6469 6669 6572 3a0a 2020 2020  ftModifier:.    
-00008b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b20: 7072 6576 5f74 6162 203d 2073 656c 662e  prev_tab = self.
-00008b30: 7461 625f 7072 6576 2e67 6574 2873 656c  tab_prev.get(sel
-00008b40: 662e 6f74 6865 725f 3229 0a20 2020 2020  f.other_2).     
-00008b50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00008b60: 7265 765f 7461 622e 7365 7446 6f63 7573  rev_tab.setFocus
-00008b70: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00008b80: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-00008b90: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
-00008ba0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00008bb0: 7265 765f 7461 622e 656e 6428 4661 6c73  rev_tab.end(Fals
-00008bc0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00008bd0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00008be0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00008bf0: 745f 7461 6220 3d20 7365 6c66 2e74 6162  t_tab = self.tab
-00008c00: 5f6e 6578 742e 6765 7428 7365 6c66 2e6f  _next.get(self.o
-00008c10: 7468 6572 5f32 290a 2020 2020 2020 2020  ther_2).        
-00008c20: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00008c30: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
-00008c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c50: 2020 2020 6e65 7874 5f74 6162 2e64 6573      next_tab.des
-00008c60: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
-00008c70: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00008c80: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
-00008c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ca0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-00008cb0: 2020 2069 6620 7365 6c66 2e63 616c 6c73     if self.calls
-00008cc0: 6967 6e2e 6861 7346 6f63 7573 2829 3a0a  ign.hasFocus():.
-00008cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ce0: 6c6f 6767 6572 2e64 6562 7567 2822 4672  logger.debug("Fr
-00008cf0: 6f6d 2063 616c 6c73 6967 6e22 290a 2020  om callsign").  
-00008d00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00008d10: 6c66 2e63 6865 636b 5f63 616c 6c73 6967  lf.check_callsig
-00008d20: 6e28 7365 6c66 2e63 616c 6c73 6967 6e2e  n(self.callsign.
-00008d30: 7465 7874 2829 290a 2020 2020 2020 2020  text()).        
-00008d40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00008d50: 6368 6563 6b5f 6475 7065 2873 656c 662e  check_dupe(self.
-00008d60: 6361 6c6c 7369 676e 2e74 6578 7428 2929  callsign.text())
-00008d70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008d80: 2020 2020 2020 7365 6c66 2e64 7570 655f        self.dupe_
-00008d90: 696e 6469 6361 746f 722e 7368 6f77 2829  indicator.show()
-00008da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008db0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00008dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008dd0: 6475 7065 5f69 6e64 6963 6174 6f72 2e68  dupe_indicator.h
-00008de0: 6964 6528 290a 2020 2020 2020 2020 2020  ide().          
-00008df0: 2020 2020 2020 6966 206d 6f64 6966 6965        if modifie
-00008e00: 7220 3d3d 2051 742e 5368 6966 744d 6f64  r == Qt.ShiftMod
-00008e10: 6966 6965 723a 0a20 2020 2020 2020 2020  ifier:.         
-00008e20: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
-00008e30: 7461 6220 3d20 7365 6c66 2e74 6162 5f70  tab = self.tab_p
-00008e40: 7265 762e 6765 7428 7365 6c66 2e63 616c  rev.get(self.cal
-00008e50: 6c73 6967 6e29 0a20 2020 2020 2020 2020  lsign).         
-00008e60: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
-00008e70: 7461 622e 7365 7446 6f63 7573 2829 0a20  tab.setFocus(). 
-00008e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e90: 2020 2070 7265 765f 7461 622e 6465 7365     prev_tab.dese
-00008ea0: 6c65 6374 2829 0a20 2020 2020 2020 2020  lect().         
-00008eb0: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
-00008ec0: 7461 622e 656e 6428 4661 6c73 6529 0a20  tab.end(False). 
-00008ed0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00008ee0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00008ef0: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
-00008f00: 7365 6c66 2e63 616c 6c73 6967 6e2e 7465  self.callsign.te
-00008f10: 7874 2829 0a20 2020 2020 2020 2020 2020  xt().           
-00008f20: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
-00008f30: 7465 7874 2e75 7070 6572 2829 0a20 2020  text.upper().   
-00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f50: 205f 7468 6574 6872 6561 6420 3d20 7468   _thethread = th
-00008f60: 7265 6164 696e 672e 5468 7265 6164 280a  reading.Thread(.
-00008f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f80: 2020 2020 2020 2020 7461 7267 6574 3d73          target=s
-00008f90: 656c 662e 6368 6563 6b5f 6361 6c6c 7369  elf.check_callsi
-00008fa0: 676e 322c 0a20 2020 2020 2020 2020 2020  gn2,.           
-00008fb0: 2020 2020 2020 2020 2020 2020 2061 7267               arg
-00008fc0: 733d 2874 6578 742c 292c 0a20 2020 2020  s=(text,),.     
-00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fe0: 2020 2064 6165 6d6f 6e3d 5472 7565 2c0a     daemon=True,.
-00008ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009000: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00009010: 2020 2020 2020 2020 2020 5f74 6865 7468            _theth
-00009020: 7265 6164 2e73 7461 7274 2829 0a20 2020  read.start().   
-00009030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009040: 206e 6578 745f 7461 6220 3d20 7365 6c66   next_tab = self
-00009050: 2e74 6162 5f6e 6578 742e 6765 7428 7365  .tab_next.get(se
-00009060: 6c66 2e63 616c 6c73 6967 6e29 0a20 2020  lf.callsign).   
-00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009080: 206e 6578 745f 7461 622e 7365 7446 6f63   next_tab.setFoc
-00009090: 7573 2829 0a20 2020 2020 2020 2020 2020  us().           
-000090a0: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-000090b0: 622e 6465 7365 6c65 6374 2829 0a20 2020  b.deselect().   
-000090c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090d0: 206e 6578 745f 7461 622e 656e 6428 4661   next_tab.end(Fa
-000090e0: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-000090f0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00009100: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
-00009110: 2829 203d 3d20 5174 2e4b 6579 5f46 313a  () == Qt.Key_F1:
-00009120: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00009130: 662e 7365 6e64 6631 2829 0a20 2020 2020  f.sendf1().     
-00009140: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-00009150: 2920 3d3d 2051 742e 4b65 795f 4632 3a0a  ) == Qt.Key_F2:.
-00009160: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009170: 2e73 656e 6466 3228 290a 2020 2020 2020  .sendf2().      
-00009180: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
-00009190: 203d 3d20 5174 2e4b 6579 5f46 333a 0a20   == Qt.Key_F3:. 
-000091a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000091b0: 7365 6e64 6633 2829 0a20 2020 2020 2020  sendf3().       
-000091c0: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
-000091d0: 3d3d 2051 742e 4b65 795f 4634 3a0a 2020  == Qt.Key_F4:.  
-000091e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000091f0: 656e 6466 3428 290a 2020 2020 2020 2020  endf4().        
-00009200: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-00009210: 3d20 5174 2e4b 6579 5f46 353a 0a20 2020  = Qt.Key_F5:.   
-00009220: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00009230: 6e64 6635 2829 0a20 2020 2020 2020 2069  ndf5().        i
-00009240: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-00009250: 2051 742e 4b65 795f 4636 3a0a 2020 2020   Qt.Key_F6:.    
-00009260: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00009270: 6466 3628 290a 2020 2020 2020 2020 6966  df6().        if
-00009280: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00009290: 5174 2e4b 6579 5f46 373a 0a20 2020 2020  Qt.Key_F7:.     
-000092a0: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-000092b0: 6637 2829 0a20 2020 2020 2020 2069 6620  f7().        if 
-000092c0: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-000092d0: 742e 4b65 795f 4638 3a0a 2020 2020 2020  t.Key_F8:.      
-000092e0: 2020 2020 2020 7365 6c66 2e73 656e 6466        self.sendf
-000092f0: 3828 290a 2020 2020 2020 2020 6966 2065  8().        if e
-00009300: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
-00009310: 2e4b 6579 5f46 393a 0a20 2020 2020 2020  .Key_F9:.       
-00009320: 2020 2020 2073 656c 662e 7365 6e64 6639       self.sendf9
-00009330: 2829 0a20 2020 2020 2020 2069 6620 6576  ().        if ev
-00009340: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
-00009350: 4b65 795f 4631 303a 0a20 2020 2020 2020  Key_F10:.       
-00009360: 2020 2020 2073 656c 662e 7365 6e64 6631       self.sendf1
-00009370: 3028 290a 2020 2020 2020 2020 6966 2065  0().        if e
-00009380: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
-00009390: 2e4b 6579 5f46 3131 3a0a 2020 2020 2020  .Key_F11:.      
-000093a0: 2020 2020 2020 7365 6c66 2e73 656e 6466        self.sendf
-000093b0: 3131 2829 0a20 2020 2020 2020 2069 6620  11().        if 
-000093c0: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-000093d0: 742e 4b65 795f 4631 323a 0a20 2020 2020  t.Key_F12:.     
-000093e0: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-000093f0: 6631 3228 290a 0a20 2020 2064 6566 2073  f12()..    def s
-00009400: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
-00009410: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00009420: 2222 5365 7420 7769 6e64 6f77 2074 6974  ""Set window tit
-00009430: 6c65 2222 220a 2020 2020 2020 2020 7666  le""".        vf
-00009440: 6f61 203d 2073 656c 662e 7261 6469 6f5f  oa = self.radio_
-00009450: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
-00009460: 2c20 2222 290a 2020 2020 2020 2020 6966  , "").        if
-00009470: 2076 666f 613a 0a20 2020 2020 2020 2020   vfoa:.         
-00009480: 2020 2076 666f 6120 3d20 696e 7428 7666     vfoa = int(vf
-00009490: 6f61 2920 2f20 3130 3030 0a20 2020 2020  oa) / 1000.     
-000094a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000094b0: 2020 2020 2076 666f 6120 3d20 302e 300a       vfoa = 0.0.
-000094c0: 2020 2020 2020 2020 636f 6e74 6573 745f          contest_
-000094d0: 6e61 6d65 203d 2022 220a 2020 2020 2020  name = "".      
-000094e0: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
-000094f0: 743a 0a20 2020 2020 2020 2020 2020 2063  t:.            c
-00009500: 6f6e 7465 7374 5f6e 616d 6520 3d20 7365  ontest_name = se
-00009510: 6c66 2e63 6f6e 7465 7374 2e6e 616d 650a  lf.contest.name.
-00009520: 2020 2020 2020 2020 6c69 6e65 203d 2028          line = (
-00009530: 0a20 2020 2020 2020 2020 2020 2066 2276  .            f"v
-00009540: 666f 613a 7b72 6f75 6e64 2876 666f 612c  foa:{round(vfoa,
-00009550: 3229 7d20 220a 2020 2020 2020 2020 2020  2)} ".          
-00009560: 2020 6622 6d6f 6465 3a7b 7365 6c66 2e72    f"mode:{self.r
-00009570: 6164 696f 5f73 7461 7465 2e67 6574 2827  adio_state.get('
-00009580: 6d6f 6465 272c 2027 2729 7d20 220a 2020  mode', '')} ".  
-00009590: 2020 2020 2020 2020 2020 6622 4f50 3a7b            f"OP:{
-000095a0: 7365 6c66 2e63 7572 7265 6e74 5f6f 707d  self.current_op}
-000095b0: 207b 636f 6e74 6573 745f 6e61 6d65 7d20   {contest_name} 
-000095c0: 220a 2020 2020 2020 2020 2020 2020 6622  ".            f"
-000095d0: 2d20 4e6f 7431 4d4d 2076 7b5f 5f76 6572  - Not1MM v{__ver
-000095e0: 7369 6f6e 5f5f 7d22 0a20 2020 2020 2020  sion__}".       
-000095f0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00009600: 7365 7457 696e 646f 7754 6974 6c65 286c  setWindowTitle(l
-00009610: 696e 6529 0a0a 2020 2020 6465 6620 636c  ine)..    def cl
-00009620: 6561 7269 6e70 7574 7328 7365 6c66 293a  earinputs(self):
-00009630: 0a20 2020 2020 2020 2022 2222 436c 6561  .        """Clea
-00009640: 7273 2074 6865 2074 6578 7420 696e 7075  rs the text inpu
-00009650: 7420 6669 656c 6473 2061 6e64 2073 6574  t fields and set
-00009660: 7320 666f 6375 7320 746f 2063 616c 6c73  s focus to calls
-00009670: 6967 6e20 6669 656c 642e 2222 220a 2020  ign field.""".  
-00009680: 2020 2020 2020 7365 6c66 2e64 7570 655f        self.dupe_
-00009690: 696e 6469 6361 746f 722e 6869 6465 2829  indicator.hide()
-000096a0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-000096b0: 6e74 6163 7420 3d20 7365 6c66 2e64 6174  ntact = self.dat
-000096c0: 6162 6173 652e 656d 7074 795f 636f 6e74  abase.empty_cont
-000096d0: 6163 740a 2020 2020 2020 2020 7365 6c66  act.        self
-000096e0: 2e68 6561 6469 6e67 5f64 6973 7461 6e63  .heading_distanc
-000096f0: 652e 7365 7454 6578 7428 2222 290a 2020  e.setText("").  
-00009700: 2020 2020 2020 7365 6c66 2e64 785f 656e        self.dx_en
-00009710: 7469 7479 2e73 6574 5465 7874 2822 2229  tity.setText("")
-00009720: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00009730: 2e63 6f6e 7465 7374 3a0a 2020 2020 2020  .contest:.      
-00009740: 2020 2020 2020 6d75 6c74 7320 3d20 7365        mults = se
-00009750: 6c66 2e63 6f6e 7465 7374 2e73 686f 775f  lf.contest.show_
-00009760: 6d75 6c74 7328 7365 6c66 290a 2020 2020  mults(self).    
-00009770: 2020 2020 2020 2020 7173 6f73 203d 2073          qsos = s
-00009780: 656c 662e 636f 6e74 6573 742e 7368 6f77  elf.contest.show
-00009790: 5f71 736f 2873 656c 6629 0a20 2020 2020  _qso(self).     
-000097a0: 2020 2020 2020 206d 756c 7473 7472 696e         multstrin
-000097b0: 6720 3d20 6622 7b71 736f 737d 2f7b 6d75  g = f"{qsos}/{mu
-000097c0: 6c74 737d 220a 2020 2020 2020 2020 2020  lts}".          
-000097d0: 2020 7365 6c66 2e6d 756c 7473 2e73 6574    self.mults.set
-000097e0: 5465 7874 286d 756c 7473 7472 696e 6729  Text(multstring)
-000097f0: 0a20 2020 2020 2020 2020 2020 2073 636f  .            sco
-00009800: 7265 203d 2073 656c 662e 636f 6e74 6573  re = self.contes
-00009810: 742e 6361 6c63 5f73 636f 7265 2873 656c  t.calc_score(sel
-00009820: 6629 0a20 2020 2020 2020 2020 2020 2073  f).            s
-00009830: 656c 662e 7363 6f72 652e 7365 7454 6578  elf.score.setTex
-00009840: 7428 7374 7228 7363 6f72 6529 290a 2020  t(str(score)).  
-00009850: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00009860: 6f6e 7465 7374 2e72 6573 6574 5f6c 6162  ontest.reset_lab
-00009870: 656c 2873 656c 6629 0a20 2020 2020 2020  el(self).       
-00009880: 2073 656c 662e 6361 6c6c 7369 676e 2e63   self.callsign.c
-00009890: 6c65 6172 2829 0a20 2020 2020 2020 2069  lear().        i
-000098a0: 6620 7365 6c66 2e63 7572 7265 6e74 5f6d  f self.current_m
-000098b0: 6f64 6520 3d3d 2022 4357 223a 0a20 2020  ode == "CW":.   
-000098c0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000098d0: 6e74 2e73 6574 5465 7874 2822 3539 3922  nt.setText("599"
-000098e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000098f0: 6c66 2e72 6563 6569 7665 2e73 6574 5465  lf.receive.setTe
-00009900: 7874 2822 3539 3922 290a 2020 2020 2020  xt("599").      
-00009910: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00009920: 2020 2020 7365 6c66 2e73 656e 742e 7365      self.sent.se
-00009930: 7454 6578 7428 2235 3922 290a 2020 2020  tText("59").    
-00009940: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
-00009950: 6569 7665 2e73 6574 5465 7874 2822 3539  eive.setText("59
-00009960: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00009970: 6f74 6865 725f 312e 636c 6561 7228 290a  other_1.clear().
-00009980: 2020 2020 2020 2020 7365 6c66 2e6f 7468          self.oth
-00009990: 6572 5f32 2e63 6c65 6172 2829 0a20 2020  er_2.clear().   
-000099a0: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
-000099b0: 676e 2e73 6574 466f 6375 7328 290a 2020  gn.setFocus().  
-000099c0: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
-000099d0: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
-000099e0: 5d20 3d20 2243 414c 4c43 4841 4e47 4544  ] = "CALLCHANGED
-000099f0: 220a 2020 2020 2020 2020 636d 645b 2273  ".        cmd["s
-00009a00: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
-00009a10: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
-00009a20: 2020 2063 6d64 5b22 6361 6c6c 225d 203d     cmd["call"] =
-00009a30: 2022 220a 2020 2020 2020 2020 7365 6c66   "".        self
-00009a40: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-00009a50: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
-00009a60: 6e28 636d 6429 0a0a 2020 2020 6465 6620  n(cmd)..    def 
-00009a70: 7361 7665 5f63 6f6e 7461 6374 2873 656c  save_contact(sel
-00009a80: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
-00009a90: 6176 6520 746f 2064 6222 2222 0a20 2020  ave to db""".   
-00009aa0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00009ab0: 6728 2273 6176 696e 6720 636f 6e74 6163  g("saving contac
-00009ac0: 7422 290a 2020 2020 2020 2020 6966 2073  t").        if s
-00009ad0: 656c 662e 636f 6e74 6573 7420 6973 204e  elf.contest is N
-00009ae0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00009af0: 2073 656c 662e 7368 6f77 5f6d 6573 7361   self.show_messa
-00009b00: 6765 5f62 6f78 2822 596f 7520 6861 7665  ge_box("You have
-00009b10: 206e 6f20 636f 6e74 6573 7420 6465 6669   no contest defi
-00009b20: 6e65 642e 2229 0a20 2020 2020 2020 2020  ned.").         
-00009b30: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00009b40: 2020 6966 206c 656e 2873 656c 662e 6361    if len(self.ca
-00009b50: 6c6c 7369 676e 2e74 6578 7428 2929 203c  llsign.text()) <
-00009b60: 2033 3a0a 2020 2020 2020 2020 2020 2020   3:.            
-00009b70: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-00009b80: 6620 6e6f 7420 616e 7928 6368 6172 2e69  f not any(char.i
-00009b90: 7364 6967 6974 2829 2066 6f72 2063 6861  sdigit() for cha
-00009ba0: 7220 696e 2073 656c 662e 6361 6c6c 7369  r in self.callsi
-00009bb0: 676e 2e74 6578 7428 2929 3a0a 2020 2020  gn.text()):.    
-00009bc0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00009bd0: 2020 2020 2020 2069 6620 6e6f 7420 616e         if not an
-00009be0: 7928 6368 6172 2e69 7361 6c70 6861 2829  y(char.isalpha()
-00009bf0: 2066 6f72 2063 6861 7220 696e 2073 656c   for char in sel
-00009c00: 662e 6361 6c6c 7369 676e 2e74 6578 7428  f.callsign.text(
-00009c10: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00009c20: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
-00009c30: 7365 6c66 2e63 6f6e 7461 6374 5b22 5453  self.contact["TS
-00009c40: 225d 203d 2064 6174 6574 696d 652e 7574  "] = datetime.ut
-00009c50: 636e 6f77 2829 2e69 736f 666f 726d 6174  cnow().isoformat
-00009c60: 2822 2022 295b 3a31 395d 0a20 2020 2020  (" ")[:19].     
-00009c70: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
-00009c80: 2243 616c 6c22 5d20 3d20 7365 6c66 2e63  "Call"] = self.c
-00009c90: 616c 6c73 6967 6e2e 7465 7874 2829 0a20  allsign.text(). 
-00009ca0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00009cb0: 6163 745b 2246 7265 7122 5d20 3d20 726f  act["Freq"] = ro
-00009cc0: 756e 6428 666c 6f61 7428 7365 6c66 2e72  und(float(self.r
-00009cd0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-00009ce0: 7666 6f61 222c 2030 2e30 2929 202f 2031  vfoa", 0.0)) / 1
-00009cf0: 3030 302c 2032 290a 2020 2020 2020 2020  000, 2).        
-00009d00: 7365 6c66 2e63 6f6e 7461 6374 5b22 5153  self.contact["QS
-00009d10: 5846 7265 7122 5d20 3d20 726f 756e 6428  XFreq"] = round(
-00009d20: 0a20 2020 2020 2020 2020 2020 2066 6c6f  .            flo
-00009d30: 6174 2873 656c 662e 7261 6469 6f5f 7374  at(self.radio_st
-00009d40: 6174 652e 6765 7428 2276 666f 6122 2c20  ate.get("vfoa", 
-00009d50: 302e 3029 2920 2f20 3130 3030 2c20 320a  0.0)) / 1000, 2.
-00009d60: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00009d70: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-00009d80: 4d6f 6465 225d 203d 2073 656c 662e 7261  Mode"] = self.ra
-00009d90: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
-00009da0: 6f64 6522 2c20 2222 290a 2020 2020 2020  ode", "").      
-00009db0: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-00009dc0: 436f 6e74 6573 744e 616d 6522 5d20 3d20  ContestName"] = 
-00009dd0: 7365 6c66 2e63 6f6e 7465 7374 2e63 6162  self.contest.cab
-00009de0: 7269 6c6c 6f5f 6e61 6d65 0a20 2020 2020  rillo_name.     
-00009df0: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
-00009e00: 2243 6f6e 7465 7374 4e52 225d 203d 2073  "ContestNR"] = s
-00009e10: 656c 662e 7072 6566 2e67 6574 2822 636f  elf.pref.get("co
-00009e20: 6e74 6573 7422 2c20 2230 2229 0a20 2020  ntest", "0").   
-00009e30: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-00009e40: 745b 2253 7461 7469 6f6e 5072 6566 6978  t["StationPrefix
-00009e50: 225d 203d 2073 656c 662e 7374 6174 696f  "] = self.statio
-00009e60: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
-00009e70: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00009e80: 6f6e 7461 6374 5b22 5750 5850 7265 6669  ontact["WPXPrefi
-00009e90: 7822 5d20 3d20 6361 6c63 756c 6174 655f  x"] = calculate_
-00009ea0: 7770 785f 7072 6566 6978 2873 656c 662e  wpx_prefix(self.
-00009eb0: 6361 6c6c 7369 676e 2e74 6578 7428 2929  callsign.text())
-00009ec0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00009ed0: 6e74 6163 745b 2249 7352 756e 5153 4f22  ntact["IsRunQSO"
-00009ee0: 5d20 3d20 7365 6c66 2e72 6164 696f 4275  ] = self.radioBu
-00009ef0: 7474 6f6e 5f72 756e 2e69 7343 6865 636b  tton_run.isCheck
-00009f00: 6564 2829 0a20 2020 2020 2020 2073 656c  ed().        sel
-00009f10: 662e 636f 6e74 6163 745b 224f 7065 7261  f.contact["Opera
-00009f20: 746f 7222 5d20 3d20 7365 6c66 2e63 7572  tor"] = self.cur
-00009f30: 7265 6e74 5f6f 700a 2020 2020 2020 2020  rent_op.        
-00009f40: 7365 6c66 2e63 6f6e 7461 6374 5b22 4e65  self.contact["Ne
-00009f50: 7442 696f 734e 616d 6522 5d20 3d20 736f  tBiosName"] = so
-00009f60: 636b 6574 2e67 6574 686f 7374 6e61 6d65  cket.gethostname
-00009f70: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00009f80: 636f 6e74 6163 745b 2249 734f 7269 6769  contact["IsOrigi
-00009f90: 6e61 6c22 5d20 3d20 310a 2020 2020 2020  nal"] = 1.      
-00009fa0: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-00009fb0: 4944 225d 203d 2075 7569 642e 7575 6964  ID"] = uuid.uuid
-00009fc0: 3428 292e 6865 780a 2020 2020 2020 2020  4().hex.        
-00009fd0: 7365 6c66 2e63 6f6e 7465 7374 2e73 6574  self.contest.set
-00009fe0: 5f63 6f6e 7461 6374 5f76 6172 7328 7365  _contact_vars(se
-00009ff0: 6c66 290a 2020 2020 2020 2020 7365 6c66  lf).        self
-0000a000: 2e63 6f6e 7461 6374 5b22 506f 696e 7473  .contact["Points
-0000a010: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-0000a020: 742e 706f 696e 7473 2873 656c 6629 0a20  t.points(self). 
-0000a030: 2020 2020 2020 2064 6562 7567 5f6f 7574         debug_out
-0000a040: 7075 7420 3d20 6622 7b73 656c 662e 636f  put = f"{self.co
-0000a050: 6e74 6163 747d 220a 2020 2020 2020 2020  ntact}".        
-0000a060: 6c6f 6767 6572 2e64 6562 7567 2864 6562  logger.debug(deb
-0000a070: 7567 5f6f 7574 7075 7429 0a0a 2020 2020  ug_output)..    
-0000a080: 2020 2020 6966 2073 656c 662e 6e31 6d6d      if self.n1mm
-0000a090: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-0000a0a0: 6767 6572 2e64 6562 7567 2822 7061 636b  gger.debug("pack
-0000a0b0: 6574 7320 2573 222c 2066 227b 7365 6c66  ets %s", f"{self
-0000a0c0: 2e6e 316d 6d2e 7365 6e64 5f63 6f6e 7461  .n1mm.send_conta
-0000a0d0: 6374 5f70 6163 6b65 7473 7d22 290a 2020  ct_packets}").  
-0000a0e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000a0f0: 662e 6e31 6d6d 2e73 656e 645f 636f 6e74  f.n1mm.send_cont
-0000a100: 6163 745f 7061 636b 6574 733a 0a20 2020  act_packets:.   
-0000a110: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000a120: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
-0000a130: 6e66 6f5b 2274 696d 6573 7461 6d70 225d  nfo["timestamp"]
-0000a140: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
-0000a150: 2254 5322 5d0a 2020 2020 2020 2020 2020  "TS"].          
-0000a160: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000a170: 636f 6e74 6163 745f 696e 666f 5b22 6f6c  contact_info["ol
-0000a180: 6463 616c 6c22 5d20 3d20 7365 6c66 2e6e  dcall"] = self.n
-0000a190: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
-0000a1a0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-0000a1b0: 2020 2020 2020 2263 616c 6c22 0a20 2020        "call".   
-0000a1c0: 2020 2020 2020 2020 2020 2020 205d 203d               ] =
-0000a1d0: 2073 656c 662e 636f 6e74 6163 745b 2243   self.contact["C
-0000a1e0: 616c 6c22 5d0a 2020 2020 2020 2020 2020  all"].          
-0000a1f0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000a200: 636f 6e74 6163 745f 696e 666f 5b22 7478  contact_info["tx
-0000a210: 6672 6571 225d 203d 2073 656c 662e 6e31  freq"] = self.n1
-0000a220: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
-0000a230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a240: 2020 2020 2022 7278 6672 6571 220a 2020       "rxfreq".  
-0000a250: 2020 2020 2020 2020 2020 2020 2020 5d20                ] 
-0000a260: 3d20 7365 6c66 2e6e 316d 6d2e 7261 6469  = self.n1mm.radi
-0000a270: 6f5f 696e 666f 5b22 4672 6571 225d 0a20  o_info["Freq"]. 
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a290: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
-0000a2a0: 5f69 6e66 6f5b 226d 6f64 6522 5d20 3d20  _info["mode"] = 
-0000a2b0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4d6f  self.contact["Mo
-0000a2c0: 6465 225d 0a20 2020 2020 2020 2020 2020  de"].           
-0000a2d0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-0000a2e0: 6f6e 7461 6374 5f69 6e66 6f5b 2263 6f6e  ontact_info["con
-0000a2f0: 7465 7374 6e61 6d65 225d 203d 2073 656c  testname"] = sel
-0000a300: 662e 636f 6e74 6163 745b 0a20 2020 2020  f.contact[.     
-0000a310: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000a320: 436f 6e74 6573 744e 616d 6522 0a20 2020  ContestName".   
-0000a330: 2020 2020 2020 2020 2020 2020 205d 2e72               ].r
-0000a340: 6570 6c61 6365 2822 2d22 2c20 2222 290a  eplace("-", "").
-0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a360: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000a370: 745f 696e 666f 5b22 636f 6e74 6573 746e  t_info["contestn
-0000a380: 7222 5d20 3d20 7365 6c66 2e63 6f6e 7461  r"] = self.conta
-0000a390: 6374 5b22 436f 6e74 6573 744e 5222 5d0a  ct["ContestNR"].
-0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3b0: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000a3c0: 745f 696e 666f 5b22 7374 6174 696f 6e70  t_info["stationp
-0000a3d0: 7265 6669 7822 5d20 3d20 7365 6c66 2e63  refix"] = self.c
-0000a3e0: 6f6e 7461 6374 5b22 5374 6174 696f 6e50  ontact["StationP
-0000a3f0: 7265 6669 7822 5d0a 2020 2020 2020 2020  refix"].        
-0000a400: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-0000a410: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
-0000a420: 7770 7870 7265 6669 7822 5d20 3d20 7365  wpxprefix"] = se
-0000a430: 6c66 2e63 6f6e 7461 6374 5b22 5750 5850  lf.contact["WPXP
-0000a440: 7265 6669 7822 5d0a 2020 2020 2020 2020  refix"].        
-0000a450: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-0000a460: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
-0000a470: 4973 5275 6e51 534f 225d 203d 2073 656c  IsRunQSO"] = sel
-0000a480: 662e 636f 6e74 6163 745b 2249 7352 756e  f.contact["IsRun
-0000a490: 5153 4f22 5d0a 2020 2020 2020 2020 2020  QSO"].          
-0000a4a0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000a4b0: 636f 6e74 6163 745f 696e 666f 5b22 6f70  contact_info["op
-0000a4c0: 6572 6174 6f72 225d 203d 2073 656c 662e  erator"] = self.
-0000a4d0: 636f 6e74 6163 745b 224f 7065 7261 746f  contact["Operato
-0000a4e0: 7222 5d0a 2020 2020 2020 2020 2020 2020  r"].            
-0000a4f0: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
-0000a500: 6e74 6163 745f 696e 666f 5b22 6d79 6361  ntact_info["myca
-0000a510: 6c6c 225d 203d 2073 656c 662e 636f 6e74  ll"] = self.cont
-0000a520: 6163 745b 224f 7065 7261 746f 7222 5d0a  act["Operator"].
-0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a540: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000a550: 745f 696e 666f 5b22 5374 6174 696f 6e4e  t_info["StationN
-0000a560: 616d 6522 5d20 3d20 7365 6c66 2e6e 316d  ame"] = self.n1m
-0000a570: 6d2e 636f 6e74 6163 745f 696e 666f 5b0a  m.contact_info[.
-0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a590: 2020 2020 224e 6574 4269 6f73 4e61 6d65      "NetBiosName
-0000a5a0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000a5b0: 2020 5d20 3d20 7365 6c66 2e63 6f6e 7461    ] = self.conta
-0000a5c0: 6374 5b22 4e65 7442 696f 734e 616d 6522  ct["NetBiosName"
-0000a5d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000a5e0: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
-0000a5f0: 6163 745f 696e 666f 5b22 4973 4f72 6967  act_info["IsOrig
-0000a600: 696e 616c 225d 203d 2073 656c 662e 636f  inal"] = self.co
-0000a610: 6e74 6163 745b 2249 734f 7269 6769 6e61  ntact["IsOrigina
-0000a620: 6c22 5d0a 2020 2020 2020 2020 2020 2020  l"].            
-0000a630: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
-0000a640: 6e74 6163 745f 696e 666f 5b22 4944 225d  ntact_info["ID"]
-0000a650: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
-0000a660: 2249 4422 5d0a 2020 2020 2020 2020 2020  "ID"].          
-0000a670: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000a680: 636f 6e74 6163 745f 696e 666f 5b22 706f  contact_info["po
-0000a690: 696e 7473 225d 203d 2073 656c 662e 636f  ints"] = self.co
-0000a6a0: 6e74 6163 745b 2250 6f69 6e74 7322 5d0a  ntact["Points"].
-0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6c0: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000a6d0: 745f 696e 666f 5b22 736e 7422 5d20 3d20  t_info["snt"] = 
-0000a6e0: 7365 6c66 2e63 6f6e 7461 6374 5b22 534e  self.contact["SN
-0000a6f0: 5422 5d0a 2020 2020 2020 2020 2020 2020  T"].            
-0000a700: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
-0000a710: 6e74 6163 745f 696e 666f 5b22 7263 7622  ntact_info["rcv"
-0000a720: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
-0000a730: 5b22 5243 5622 5d0a 2020 2020 2020 2020  ["RCV"].        
-0000a740: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-0000a750: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
-0000a760: 736e 746e 7222 5d20 3d20 7365 6c66 2e63  sntnr"] = self.c
-0000a770: 6f6e 7461 6374 5b22 5365 6e74 4e72 225d  ontact["SentNr"]
-0000a780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a790: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
-0000a7a0: 6374 5f69 6e66 6f5b 2272 6376 6e72 225d  ct_info["rcvnr"]
-0000a7b0: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
-0000a7c0: 224e 5222 5d0a 2020 2020 2020 2020 2020  "NR"].          
-0000a7d0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000a7e0: 636f 6e74 6163 745f 696e 666f 5b22 6973  contact_info["is
-0000a7f0: 6d75 6c74 6970 6c69 6572 3122 5d20 3d20  multiplier1"] = 
-0000a800: 7365 6c66 2e63 6f6e 7461 6374 2e67 6574  self.contact.get
-0000a810: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000a820: 2020 2020 2020 2249 734d 756c 7469 706c        "IsMultipl
-0000a830: 6965 7231 222c 2030 0a20 2020 2020 2020  ier1", 0.       
-0000a840: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000a850: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a860: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
-0000a870: 6f5b 2269 736d 756c 7469 706c 6965 7232  o["ismultiplier2
-0000a880: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
-0000a890: 742e 6765 7428 0a20 2020 2020 2020 2020  t.get(.         
-0000a8a0: 2020 2020 2020 2020 2020 2022 4973 4d75             "IsMu
-0000a8b0: 6c74 6970 6c69 6572 3222 2c20 300a 2020  ltiplier2", 0.  
-0000a8c0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8e0: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000a8f0: 745f 696e 666f 5b22 6973 6d75 6c74 6970  t_info["ismultip
-0000a900: 6c69 6572 3322 5d20 3d20 7365 6c66 2e63  lier3"] = self.c
-0000a910: 6f6e 7461 6374 2e67 6574 280a 2020 2020  ontact.get(.    
-0000a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a930: 2249 734d 756c 7469 706c 6965 7233 222c  "IsMultiplier3",
-0000a940: 2022 3022 0a20 2020 2020 2020 2020 2020   "0".           
-0000a950: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000a960: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-0000a970: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2273  .contact_info["s
-0000a980: 6563 7469 6f6e 225d 203d 2073 656c 662e  ection"] = self.
-0000a990: 636f 6e74 6163 745b 2253 6563 7422 5d0a  contact["Sect"].
-0000a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9b0: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000a9c0: 745f 696e 666f 5b22 7072 6563 225d 203d  t_info["prec"] =
-0000a9d0: 2073 656c 662e 636f 6e74 6163 745b 2250   self.contact["P
-0000a9e0: 7265 6322 5d0a 2020 2020 2020 2020 2020  rec"].          
-0000a9f0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000aa00: 636f 6e74 6163 745f 696e 666f 5b22 636b  contact_info["ck
-0000aa10: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
-0000aa20: 745b 2243 4b22 5d0a 2020 2020 2020 2020  t["CK"].        
-0000aa30: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-0000aa40: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
-0000aa50: 7a6e 225d 203d 2073 656c 662e 636f 6e74  zn"] = self.cont
-0000aa60: 6163 745b 225a 4e22 5d0a 2020 2020 2020  act["ZN"].      
-0000aa70: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0000aa80: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
-0000aa90: 5b22 706f 7765 7222 5d20 3d20 7365 6c66  ["power"] = self
-0000aaa0: 2e63 6f6e 7461 6374 5b22 506f 7765 7222  .contact["Power"
-0000aab0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000aac0: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
-0000aad0: 6163 745f 696e 666f 5b22 6261 6e64 225d  act_info["band"]
-0000aae0: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
-0000aaf0: 2242 616e 6422 5d0a 2020 2020 2020 2020  "Band"].        
-0000ab00: 2020 2020 2020 2020 2320 7365 6c66 2e6e          # self.n
-0000ab10: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
-0000ab20: 5b27 275d 0a20 2020 2020 2020 2020 2020  [''].           
-0000ab30: 2020 2020 2023 2073 656c 662e 6e31 6d6d       # self.n1mm
-0000ab40: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2727  .contact_info[''
-0000ab50: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000ab60: 2020 2320 7365 6c66 2e6e 316d 6d2e 636f    # self.n1mm.co
-0000ab70: 6e74 6163 745f 696e 666f 5b27 275d 0a20  ntact_info['']. 
-0000ab80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000ab90: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
-0000aba0: 6374 5f69 6e66 6f5b 2727 5d0a 2020 2020  ct_info[''].    
-0000abb0: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-0000abc0: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
-0000abd0: 696e 666f 5b27 275d 0a20 2020 2020 2020  info[''].       
-0000abe0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-0000abf0: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
-0000ac00: 6f5b 2727 5d0a 2020 2020 2020 2020 2020  o[''].          
-0000ac10: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000ac20: 7567 2822 2573 222c 2066 227b 7365 6c66  ug("%s", f"{self
-0000ac30: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-0000ac40: 666f 7d22 290a 2020 2020 2020 2020 2020  fo}").          
-0000ac50: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000ac60: 7365 6e64 5f63 6f6e 7461 6374 5f69 6e66  send_contact_inf
-0000ac70: 6f28 290a 0a20 2020 2020 2020 2073 656c  o()..        sel
-0000ac80: 662e 6461 7461 6261 7365 2e6c 6f67 5f63  f.database.log_c
-0000ac90: 6f6e 7461 6374 2873 656c 662e 636f 6e74  ontact(self.cont
-0000aca0: 6163 7429 0a20 2020 2020 2020 2073 656c  act).        sel
-0000acb0: 662e 636c 6561 7269 6e70 7574 7328 290a  f.clearinputs().
-0000acc0: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
-0000acd0: 0a20 2020 2020 2020 2063 6d64 5b22 636d  .        cmd["cm
-0000ace0: 6422 5d20 3d20 2255 5044 4154 454c 4f47  d"] = "UPDATELOG
-0000acf0: 220a 2020 2020 2020 2020 636d 645b 2273  ".        cmd["s
-0000ad00: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
-0000ad10: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
-0000ad20: 2020 2073 656c 662e 6d75 6c74 6963 6173     self.multicas
-0000ad30: 745f 696e 7465 7266 6163 652e 7365 6e64  t_interface.send
-0000ad40: 5f61 735f 6a73 6f6e 2863 6d64 290a 2020  _as_json(cmd).  
-0000ad50: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-0000ad60: 7461 6374 5b22 436f 6e74 6573 744e 616d  tact["ContestNam
-0000ad70: 6522 5d20 3d20 7365 6c66 2e63 6f6e 7465  e"] = self.conte
-0000ad80: 7374 2e6e 616d 650a 2020 2020 2020 2020  st.name.        
-0000ad90: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-0000ada0: 534e 5422 5d20 3d20 7365 6c66 2e73 656e  SNT"] = self.sen
-0000adb0: 742e 7465 7874 2829 0a20 2020 2020 2020  t.text().       
-0000adc0: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-0000add0: 2252 4356 225d 203d 2073 656c 662e 7265  "RCV"] = self.re
-0000ade0: 6365 6976 652e 7465 7874 2829 0a20 2020  ceive.text().   
-0000adf0: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-0000ae00: 6163 745b 2243 6f75 6e74 7279 5072 6566  act["CountryPref
-0000ae10: 6978 225d 0a20 2020 2020 2020 2023 2073  ix"].        # s
-0000ae20: 656c 662e 636f 6e74 6163 745b 2253 7461  elf.contact["Sta
-0000ae30: 7469 6f6e 5072 6566 6978 225d 203d 2073  tionPrefix"] = s
-0000ae40: 656c 662e 7072 6566 2e67 6574 2822 6361  elf.pref.get("ca
-0000ae50: 6c6c 7369 676e 222c 2022 2229 0a20 2020  llsign", "").   
-0000ae60: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-0000ae70: 6163 745b 2251 5448 225d 0a20 2020 2020  act["QTH"].     
-0000ae80: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-0000ae90: 745b 224e 616d 6522 5d20 3d20 7365 6c66  t["Name"] = self
-0000aea0: 2e6f 7468 6572 5f31 2e74 6578 7428 290a  .other_1.text().
-0000aeb0: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-0000aec0: 6f6e 7461 6374 5b22 436f 6d6d 656e 7422  ontact["Comment"
-0000aed0: 5d20 3d20 7365 6c66 2e6f 7468 6572 5f32  ] = self.other_2
-0000aee0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000aef0: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-0000af00: 4e52 225d 0a20 2020 2020 2020 2023 2073  NR"].        # s
-0000af10: 656c 662e 636f 6e74 6163 745b 2253 6563  elf.contact["Sec
-0000af20: 7422 5d0a 2020 2020 2020 2020 2320 7365  t"].        # se
-0000af30: 6c66 2e63 6f6e 7461 6374 5b22 5072 6563  lf.contact["Prec
-0000af40: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
-0000af50: 662e 636f 6e74 6163 745b 2243 4b22 5d0a  f.contact["CK"].
-0000af60: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-0000af70: 6f6e 7461 6374 5b22 5a4e 225d 0a20 2020  ontact["ZN"].   
-0000af80: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-0000af90: 6163 745b 2253 656e 744e 7222 5d0a 2020  act["SentNr"].  
-0000afa0: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-0000afb0: 7461 6374 5b22 506f 696e 7473 225d 0a20  tact["Points"]. 
-0000afc0: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-0000afd0: 6e74 6163 745b 2249 734d 756c 7469 706c  ntact["IsMultipl
-0000afe0: 6965 7231 225d 0a20 2020 2020 2020 2023  ier1"].        #
-0000aff0: 2073 656c 662e 636f 6e74 6163 745b 2249   self.contact["I
-0000b000: 734d 756c 7469 706c 6965 7232 225d 0a20  sMultiplier2"]. 
-0000b010: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-0000b020: 6e74 6163 745b 2250 6f77 6572 225d 0a20  ntact["Power"]. 
+00008960: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00008970: 2020 2020 2069 6620 7365 6c66 2e6f 7468       if self.oth
+00008980: 6572 5f32 2e68 6173 466f 6375 7328 293a  er_2.hasFocus():
+00008990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000089a0: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+000089b0: 726f 6d20 6f74 6865 725f 3222 290a 2020  rom other_2").  
+000089c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000089d0: 206d 6f64 6966 6965 7220 3d3d 2051 742e   modifier == Qt.
+000089e0: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
+000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a00: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
+00008a10: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
+00008a20: 7365 6c66 2e6f 7468 6572 5f32 290a 2020  self.other_2).  
+00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a40: 2020 7072 6576 5f74 6162 2e73 6574 466f    prev_tab.setFo
+00008a50: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
+00008a60: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
+00008a70: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
+00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a90: 2020 7072 6576 5f74 6162 2e65 6e64 2846    prev_tab.end(F
+00008aa0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00008ab0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ad0: 6e65 7874 5f74 6162 203d 2073 656c 662e  next_tab = self.
+00008ae0: 7461 625f 6e65 7874 2e67 6574 2873 656c  tab_next.get(sel
+00008af0: 662e 6f74 6865 725f 3229 0a20 2020 2020  f.other_2).     
+00008b00: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00008b10: 6578 745f 7461 622e 7365 7446 6f63 7573  ext_tab.setFocus
+00008b20: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00008b30: 2020 2020 2020 206e 6578 745f 7461 622e         next_tab.
+00008b40: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
+00008b50: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00008b60: 6578 745f 7461 622e 656e 6428 4661 6c73  ext_tab.end(Fals
+00008b70: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00008b80: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00008b90: 2020 2020 2020 6966 2073 656c 662e 6361        if self.ca
+00008ba0: 6c6c 7369 676e 2e68 6173 466f 6375 7328  llsign.hasFocus(
+00008bb0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00008bc0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00008bd0: 2246 726f 6d20 6361 6c6c 7369 676e 2229  "From callsign")
+00008be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008bf0: 2073 656c 662e 6368 6563 6b5f 6361 6c6c   self.check_call
+00008c00: 7369 676e 2873 656c 662e 6361 6c6c 7369  sign(self.callsi
+00008c10: 676e 2e74 6578 7428 2929 0a20 2020 2020  gn.text()).     
+00008c20: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00008c30: 6c66 2e63 6865 636b 5f64 7570 6528 7365  lf.check_dupe(se
+00008c40: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
+00008c50: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
+00008c60: 2020 2020 2020 2020 2073 656c 662e 6475           self.du
+00008c70: 7065 5f69 6e64 6963 6174 6f72 2e73 686f  pe_indicator.sho
+00008c80: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
+00008c90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008ca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008cb0: 6c66 2e64 7570 655f 696e 6469 6361 746f  lf.dupe_indicato
+00008cc0: 722e 6869 6465 2829 0a20 2020 2020 2020  r.hide().       
+00008cd0: 2020 2020 2020 2020 2069 6620 6d6f 6469           if modi
+00008ce0: 6669 6572 203d 3d20 5174 2e53 6869 6674  fier == Qt.Shift
+00008cf0: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
+00008d00: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00008d10: 6576 5f74 6162 203d 2073 656c 662e 7461  ev_tab = self.ta
+00008d20: 625f 7072 6576 2e67 6574 2873 656c 662e  b_prev.get(self.
+00008d30: 6361 6c6c 7369 676e 290a 2020 2020 2020  callsign).      
+00008d40: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00008d50: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
+00008d60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008d70: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
+00008d80: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
+00008d90: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00008da0: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
+00008db0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008dc0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008dd0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+00008de0: 203d 2073 656c 662e 6361 6c6c 7369 676e   = self.callsign
+00008df0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+00008e00: 2020 2020 2020 2020 2020 2020 7465 7874              text
+00008e10: 203d 2074 6578 742e 7570 7065 7228 290a   = text.upper().
+00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e30: 2020 2020 5f74 6865 7468 7265 6164 203d      _thethread =
+00008e40: 2074 6872 6561 6469 6e67 2e54 6872 6561   threading.Threa
+00008e50: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+00008e60: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+00008e70: 743d 7365 6c66 2e63 6865 636b 5f63 616c  t=self.check_cal
+00008e80: 6c73 6967 6e32 2c0a 2020 2020 2020 2020  lsign2,.        
+00008e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ea0: 6172 6773 3d28 7465 7874 2c29 2c0a 2020  args=(text,),.  
+00008eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ec0: 2020 2020 2020 6461 656d 6f6e 3d54 7275        daemon=Tru
+00008ed0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00008ee0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00008ef0: 2020 2020 2020 2020 2020 2020 205f 7468               _th
+00008f00: 6574 6872 6561 642e 7374 6172 7428 290a  ethread.start().
+00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f20: 2020 2020 6e65 7874 5f74 6162 203d 2073      next_tab = s
+00008f30: 656c 662e 7461 625f 6e65 7874 2e67 6574  elf.tab_next.get
+00008f40: 2873 656c 662e 6361 6c6c 7369 676e 290a  (self.callsign).
+00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f60: 2020 2020 6e65 7874 5f74 6162 2e73 6574      next_tab.set
+00008f70: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
+00008f80: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00008f90: 5f74 6162 2e64 6573 656c 6563 7428 290a  _tab.deselect().
+00008fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fb0: 2020 2020 6e65 7874 5f74 6162 2e65 6e64      next_tab.end
+00008fc0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+00008fd0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00008fe0: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+00008ff0: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
+00009000: 4631 3a0a 2020 2020 2020 2020 2020 2020  F1:.            
+00009010: 7365 6c66 2e73 656e 6466 3128 290a 2020  self.sendf1().  
+00009020: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
+00009030: 6579 2829 203d 3d20 5174 2e4b 6579 5f46  ey() == Qt.Key_F
+00009040: 323a 0a20 2020 2020 2020 2020 2020 2073  2:.            s
+00009050: 656c 662e 7365 6e64 6632 2829 0a20 2020  elf.sendf2().   
+00009060: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
+00009070: 7928 2920 3d3d 2051 742e 4b65 795f 4633  y() == Qt.Key_F3
+00009080: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00009090: 6c66 2e73 656e 6466 3328 290a 2020 2020  lf.sendf3().    
+000090a0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+000090b0: 2829 203d 3d20 5174 2e4b 6579 5f46 343a  () == Qt.Key_F4:
+000090c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000090d0: 662e 7365 6e64 6634 2829 0a20 2020 2020  f.sendf4().     
+000090e0: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
+000090f0: 2920 3d3d 2051 742e 4b65 795f 4635 3a0a  ) == Qt.Key_F5:.
+00009100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009110: 2e73 656e 6466 3528 290a 2020 2020 2020  .sendf5().      
+00009120: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+00009130: 203d 3d20 5174 2e4b 6579 5f46 363a 0a20   == Qt.Key_F6:. 
+00009140: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009150: 7365 6e64 6636 2829 0a20 2020 2020 2020  sendf6().       
+00009160: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+00009170: 3d3d 2051 742e 4b65 795f 4637 3a0a 2020  == Qt.Key_F7:.  
+00009180: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00009190: 656e 6466 3728 290a 2020 2020 2020 2020  endf7().        
+000091a0: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+000091b0: 3d20 5174 2e4b 6579 5f46 383a 0a20 2020  = Qt.Key_F8:.   
+000091c0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+000091d0: 6e64 6638 2829 0a20 2020 2020 2020 2069  ndf8().        i
+000091e0: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+000091f0: 2051 742e 4b65 795f 4639 3a0a 2020 2020   Qt.Key_F9:.    
+00009200: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+00009210: 6466 3928 290a 2020 2020 2020 2020 6966  df9().        if
+00009220: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+00009230: 5174 2e4b 6579 5f46 3130 3a0a 2020 2020  Qt.Key_F10:.    
+00009240: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+00009250: 6466 3130 2829 0a20 2020 2020 2020 2069  df10().        i
+00009260: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+00009270: 2051 742e 4b65 795f 4631 313a 0a20 2020   Qt.Key_F11:.   
+00009280: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00009290: 6e64 6631 3128 290a 2020 2020 2020 2020  ndf11().        
+000092a0: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+000092b0: 3d20 5174 2e4b 6579 5f46 3132 3a0a 2020  = Qt.Key_F12:.  
+000092c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000092d0: 656e 6466 3132 2829 0a0a 2020 2020 6465  endf12()..    de
+000092e0: 6620 7365 745f 7769 6e64 6f77 5f74 6974  f set_window_tit
+000092f0: 6c65 2873 656c 6629 3a0a 2020 2020 2020  le(self):.      
+00009300: 2020 2222 2253 6574 2077 696e 646f 7720    """Set window 
+00009310: 7469 746c 6522 2222 0a20 2020 2020 2020  title""".       
+00009320: 2076 666f 6120 3d20 7365 6c66 2e72 6164   vfoa = self.rad
+00009330: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
+00009340: 6f61 222c 2022 2229 0a20 2020 2020 2020  oa", "").       
+00009350: 2069 6620 7666 6f61 3a0a 2020 2020 2020   if vfoa:.      
+00009360: 2020 2020 2020 7666 6f61 203d 2069 6e74        vfoa = int
+00009370: 2876 666f 6129 202f 2031 3030 300a 2020  (vfoa) / 1000.  
+00009380: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00009390: 2020 2020 2020 2020 7666 6f61 203d 2030          vfoa = 0
+000093a0: 2e30 0a20 2020 2020 2020 2063 6f6e 7465  .0.        conte
+000093b0: 7374 5f6e 616d 6520 3d20 2222 0a20 2020  st_name = "".   
+000093c0: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+000093d0: 7465 7374 3a0a 2020 2020 2020 2020 2020  test:.          
+000093e0: 2020 636f 6e74 6573 745f 6e61 6d65 203d    contest_name =
+000093f0: 2073 656c 662e 636f 6e74 6573 742e 6e61   self.contest.na
+00009400: 6d65 0a20 2020 2020 2020 206c 696e 6520  me.        line 
+00009410: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00009420: 6622 7666 6f61 3a7b 726f 756e 6428 7666  f"vfoa:{round(vf
+00009430: 6f61 2c32 297d 2022 0a20 2020 2020 2020  oa,2)} ".       
+00009440: 2020 2020 2066 226d 6f64 653a 7b73 656c       f"mode:{sel
+00009450: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+00009460: 7428 276d 6f64 6527 2c20 2727 297d 2022  t('mode', '')} "
+00009470: 0a20 2020 2020 2020 2020 2020 2066 224f  .            f"O
+00009480: 503a 7b73 656c 662e 6375 7272 656e 745f  P:{self.current_
+00009490: 6f70 7d20 7b63 6f6e 7465 7374 5f6e 616d  op} {contest_nam
+000094a0: 657d 2022 0a20 2020 2020 2020 2020 2020  e} ".           
+000094b0: 2066 222d 204e 6f74 314d 4d20 767b 5f5f   f"- Not1MM v{__
+000094c0: 7665 7273 696f 6e5f 5f7d 220a 2020 2020  version__}".    
+000094d0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+000094e0: 6c66 2e73 6574 5769 6e64 6f77 5469 746c  lf.setWindowTitl
+000094f0: 6528 6c69 6e65 290a 0a20 2020 2064 6566  e(line)..    def
+00009500: 2063 6c65 6172 696e 7075 7473 2873 656c   clearinputs(sel
+00009510: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
+00009520: 6c65 6172 7320 7468 6520 7465 7874 2069  lears the text i
+00009530: 6e70 7574 2066 6965 6c64 7320 616e 6420  nput fields and 
+00009540: 7365 7473 2066 6f63 7573 2074 6f20 6361  sets focus to ca
+00009550: 6c6c 7369 676e 2066 6965 6c64 2e22 2222  llsign field."""
+00009560: 0a20 2020 2020 2020 2073 656c 662e 6475  .        self.du
+00009570: 7065 5f69 6e64 6963 6174 6f72 2e68 6964  pe_indicator.hid
+00009580: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+00009590: 2e63 6f6e 7461 6374 203d 2073 656c 662e  .contact = self.
+000095a0: 6461 7461 6261 7365 2e65 6d70 7479 5f63  database.empty_c
+000095b0: 6f6e 7461 6374 0a20 2020 2020 2020 2073  ontact.        s
+000095c0: 656c 662e 6865 6164 696e 675f 6469 7374  elf.heading_dist
+000095d0: 616e 6365 2e73 6574 5465 7874 2822 2229  ance.setText("")
+000095e0: 0a20 2020 2020 2020 2073 656c 662e 6478  .        self.dx
+000095f0: 5f65 6e74 6974 792e 7365 7454 6578 7428  _entity.setText(
+00009600: 2222 290a 2020 2020 2020 2020 6966 2073  "").        if s
+00009610: 656c 662e 636f 6e74 6573 743a 0a20 2020  elf.contest:.   
+00009620: 2020 2020 2020 2020 206d 756c 7473 203d           mults =
+00009630: 2073 656c 662e 636f 6e74 6573 742e 7368   self.contest.sh
+00009640: 6f77 5f6d 756c 7473 2873 656c 6629 0a20  ow_mults(self). 
+00009650: 2020 2020 2020 2020 2020 2071 736f 7320             qsos 
+00009660: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e73  = self.contest.s
+00009670: 686f 775f 7173 6f28 7365 6c66 290a 2020  how_qso(self).  
+00009680: 2020 2020 2020 2020 2020 6d75 6c74 7374            multst
+00009690: 7269 6e67 203d 2066 227b 7173 6f73 7d2f  ring = f"{qsos}/
+000096a0: 7b6d 756c 7473 7d22 0a20 2020 2020 2020  {mults}".       
+000096b0: 2020 2020 2073 656c 662e 6d75 6c74 732e       self.mults.
+000096c0: 7365 7454 6578 7428 6d75 6c74 7374 7269  setText(multstri
+000096d0: 6e67 290a 2020 2020 2020 2020 2020 2020  ng).            
+000096e0: 7363 6f72 6520 3d20 7365 6c66 2e63 6f6e  score = self.con
+000096f0: 7465 7374 2e63 616c 635f 7363 6f72 6528  test.calc_score(
+00009700: 7365 6c66 290a 2020 2020 2020 2020 2020  self).          
+00009710: 2020 7365 6c66 2e73 636f 7265 2e73 6574    self.score.set
+00009720: 5465 7874 2873 7472 2873 636f 7265 2929  Text(str(score))
+00009730: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009740: 662e 636f 6e74 6573 742e 7265 7365 745f  f.contest.reset_
+00009750: 6c61 6265 6c28 7365 6c66 290a 2020 2020  label(self).    
+00009760: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+00009770: 6e2e 636c 6561 7228 290a 2020 2020 2020  n.clear().      
+00009780: 2020 6966 2073 656c 662e 6375 7272 656e    if self.curren
+00009790: 745f 6d6f 6465 203d 3d20 2243 5722 3a0a  t_mode == "CW":.
+000097a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000097b0: 2e73 656e 742e 7365 7454 6578 7428 2235  .sent.setText("5
+000097c0: 3939 2229 0a20 2020 2020 2020 2020 2020  99").           
+000097d0: 2073 656c 662e 7265 6365 6976 652e 7365   self.receive.se
+000097e0: 7454 6578 7428 2235 3939 2229 0a20 2020  tText("599").   
+000097f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00009800: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
+00009810: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
+00009820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009830: 7265 6365 6976 652e 7365 7454 6578 7428  receive.setText(
+00009840: 2235 3922 290a 2020 2020 2020 2020 7365  "59").        se
+00009850: 6c66 2e6f 7468 6572 5f31 2e63 6c65 6172  lf.other_1.clear
+00009860: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00009870: 6f74 6865 725f 322e 636c 6561 7228 290a  other_2.clear().
+00009880: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
+00009890: 6c73 6967 6e2e 7365 7446 6f63 7573 2829  lsign.setFocus()
+000098a0: 0a20 2020 2020 2020 2063 6d64 203d 207b  .        cmd = {
+000098b0: 7d0a 2020 2020 2020 2020 636d 645b 2263  }.        cmd["c
+000098c0: 6d64 225d 203d 2022 4341 4c4c 4348 414e  md"] = "CALLCHAN
+000098d0: 4745 4422 0a20 2020 2020 2020 2063 6d64  GED".        cmd
+000098e0: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
+000098f0: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
+00009900: 2020 2020 2020 636d 645b 2263 616c 6c22        cmd["call"
+00009910: 5d20 3d20 2222 0a20 2020 2020 2020 2073  ] = "".        s
+00009920: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
+00009930: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
+00009940: 6a73 6f6e 2863 6d64 290a 0a20 2020 2064  json(cmd)..    d
+00009950: 6566 2073 6176 655f 636f 6e74 6163 7428  ef save_contact(
+00009960: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00009970: 2222 5361 7665 2074 6f20 6462 2222 220a  ""Save to db""".
+00009980: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00009990: 6562 7567 2822 7361 7669 6e67 2063 6f6e  ebug("saving con
+000099a0: 7461 6374 2229 0a20 2020 2020 2020 2069  tact").        i
+000099b0: 6620 6c65 6e28 7365 6c66 2e63 616c 6c73  f len(self.calls
+000099c0: 6967 6e2e 7465 7874 2829 2920 3c20 333a  ign.text()) < 3:
+000099d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000099e0: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
+000099f0: 6f74 2061 6e79 2863 6861 722e 6973 6469  ot any(char.isdi
+00009a00: 6769 7428 2920 666f 7220 6368 6172 2069  git() for char i
+00009a10: 6e20 7365 6c66 2e63 616c 6c73 6967 6e2e  n self.callsign.
+00009a20: 7465 7874 2829 293a 0a20 2020 2020 2020  text()):.       
+00009a30: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00009a40: 2020 2020 6966 206e 6f74 2061 6e79 2863      if not any(c
+00009a50: 6861 722e 6973 616c 7068 6128 2920 666f  har.isalpha() fo
+00009a60: 7220 6368 6172 2069 6e20 7365 6c66 2e63  r char in self.c
+00009a70: 616c 6c73 6967 6e2e 7465 7874 2829 293a  allsign.text()):
+00009a80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00009a90: 7572 6e0a 0a20 2020 2020 2020 2073 656c  urn..        sel
+00009aa0: 662e 636f 6e74 6163 745b 2254 5322 5d20  f.contact["TS"] 
+00009ab0: 3d20 6461 7465 7469 6d65 2e75 7463 6e6f  = datetime.utcno
+00009ac0: 7728 292e 6973 6f66 6f72 6d61 7428 2220  w().isoformat(" 
+00009ad0: 2229 5b3a 3139 5d0a 2020 2020 2020 2020  ")[:19].        
+00009ae0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4361  self.contact["Ca
+00009af0: 6c6c 225d 203d 2073 656c 662e 6361 6c6c  ll"] = self.call
+00009b00: 7369 676e 2e74 6578 7428 290a 2020 2020  sign.text().    
+00009b10: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+00009b20: 5b22 4672 6571 225d 203d 2072 6f75 6e64  ["Freq"] = round
+00009b30: 2866 6c6f 6174 2873 656c 662e 7261 6469  (float(self.radi
+00009b40: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
+00009b50: 6122 2c20 302e 3029 2920 2f20 3130 3030  a", 0.0)) / 1000
+00009b60: 2c20 3229 0a20 2020 2020 2020 2073 656c  , 2).        sel
+00009b70: 662e 636f 6e74 6163 745b 2251 5358 4672  f.contact["QSXFr
+00009b80: 6571 225d 203d 2072 6f75 6e64 280a 2020  eq"] = round(.  
+00009b90: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+00009ba0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+00009bb0: 2e67 6574 2822 7666 6f61 222c 2030 2e30  .get("vfoa", 0.0
+00009bc0: 2929 202f 2031 3030 302c 2032 0a20 2020  )) / 1000, 2.   
+00009bd0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+00009be0: 656c 662e 636f 6e74 6163 745b 224d 6f64  elf.contact["Mod
+00009bf0: 6522 5d20 3d20 7365 6c66 2e72 6164 696f  e"] = self.radio
+00009c00: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+00009c10: 222c 2022 2229 0a20 2020 2020 2020 2073  ", "").        s
+00009c20: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
+00009c30: 7465 7374 4e61 6d65 225d 203d 2073 656c  testName"] = sel
+00009c40: 662e 636f 6e74 6573 742e 6361 6272 696c  f.contest.cabril
+00009c50: 6c6f 5f6e 616d 650a 2020 2020 2020 2020  lo_name.        
+00009c60: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
+00009c70: 6e74 6573 744e 5222 5d20 3d20 7365 6c66  ntestNR"] = self
+00009c80: 2e70 7265 662e 6765 7428 2263 6f6e 7465  .pref.get("conte
+00009c90: 7374 222c 2022 3022 290a 2020 2020 2020  st", "0").      
+00009ca0: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+00009cb0: 5374 6174 696f 6e50 7265 6669 7822 5d20  StationPrefix"] 
+00009cc0: 3d20 7365 6c66 2e73 7461 7469 6f6e 2e67  = self.station.g
+00009cd0: 6574 2822 4361 6c6c 222c 2022 2229 0a20  et("Call", ""). 
+00009ce0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00009cf0: 6163 745b 2257 5058 5072 6566 6978 225d  act["WPXPrefix"]
+00009d00: 203d 2063 616c 6375 6c61 7465 5f77 7078   = calculate_wpx
+00009d10: 5f70 7265 6669 7828 7365 6c66 2e63 616c  _prefix(self.cal
+00009d20: 6c73 6967 6e2e 7465 7874 2829 290a 2020  lsign.text()).  
+00009d30: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
+00009d40: 6374 5b22 4973 5275 6e51 534f 225d 203d  ct["IsRunQSO"] =
+00009d50: 2073 656c 662e 7261 6469 6f42 7574 746f   self.radioButto
+00009d60: 6e5f 7275 6e2e 6973 4368 6563 6b65 6428  n_run.isChecked(
+00009d70: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00009d80: 6f6e 7461 6374 5b22 4f70 6572 6174 6f72  ontact["Operator
+00009d90: 225d 203d 2073 656c 662e 6375 7272 656e  "] = self.curren
+00009da0: 745f 6f70 0a20 2020 2020 2020 2073 656c  t_op.        sel
+00009db0: 662e 636f 6e74 6163 745b 224e 6574 4269  f.contact["NetBi
+00009dc0: 6f73 4e61 6d65 225d 203d 2073 6f63 6b65  osName"] = socke
+00009dd0: 742e 6765 7468 6f73 746e 616d 6528 290a  t.gethostname().
+00009de0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00009df0: 7461 6374 5b22 4973 4f72 6967 696e 616c  tact["IsOriginal
+00009e00: 225d 203d 2031 0a20 2020 2020 2020 2073  "] = 1.        s
+00009e10: 656c 662e 636f 6e74 6163 745b 2249 4422  elf.contact["ID"
+00009e20: 5d20 3d20 7575 6964 2e75 7569 6434 2829  ] = uuid.uuid4()
+00009e30: 2e68 6578 0a20 2020 2020 2020 2073 656c  .hex.        sel
+00009e40: 662e 636f 6e74 6573 742e 7365 745f 636f  f.contest.set_co
+00009e50: 6e74 6163 745f 7661 7273 2873 656c 6629  ntact_vars(self)
+00009e60: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00009e70: 6e74 6163 745b 2250 6f69 6e74 7322 5d20  ntact["Points"] 
+00009e80: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e70  = self.contest.p
+00009e90: 6f69 6e74 7328 7365 6c66 290a 2020 2020  oints(self).    
+00009ea0: 2020 2020 6465 6275 675f 6f75 7470 7574      debug_output
+00009eb0: 203d 2066 227b 7365 6c66 2e63 6f6e 7461   = f"{self.conta
+00009ec0: 6374 7d22 0a20 2020 2020 2020 206c 6f67  ct}".        log
+00009ed0: 6765 722e 6465 6275 6728 6465 6275 675f  ger.debug(debug_
+00009ee0: 6f75 7470 7574 290a 0a20 2020 2020 2020  output)..       
+00009ef0: 2069 6620 7365 6c66 2e6e 316d 6d3a 0a20   if self.n1mm:. 
+00009f00: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00009f10: 722e 6465 6275 6728 2270 6163 6b65 7473  r.debug("packets
+00009f20: 2025 7322 2c20 6622 7b73 656c 662e 6e31   %s", f"{self.n1
+00009f30: 6d6d 2e73 656e 645f 636f 6e74 6163 745f  mm.send_contact_
+00009f40: 7061 636b 6574 737d 2229 0a20 2020 2020  packets}").     
+00009f50: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+00009f60: 316d 6d2e 7365 6e64 5f63 6f6e 7461 6374  1mm.send_contact
+00009f70: 5f70 6163 6b65 7473 3a0a 2020 2020 2020  _packets:.      
+00009f80: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00009f90: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+00009fa0: 5b22 7469 6d65 7374 616d 7022 5d20 3d20  ["timestamp"] = 
+00009fb0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5453  self.contact["TS
+00009fc0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00009fd0: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+00009fe0: 7461 6374 5f69 6e66 6f5b 226f 6c64 6361  tact_info["oldca
+00009ff0: 6c6c 225d 203d 2073 656c 662e 6e31 6d6d  ll"] = self.n1mm
+0000a000: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 0a20  .contact_info[. 
+0000a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a020: 2020 2022 6361 6c6c 220a 2020 2020 2020     "call".      
+0000a030: 2020 2020 2020 2020 2020 5d20 3d20 7365            ] = se
+0000a040: 6c66 2e63 6f6e 7461 6374 5b22 4361 6c6c  lf.contact["Call
+0000a050: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000a060: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+0000a070: 7461 6374 5f69 6e66 6f5b 2274 7866 7265  tact_info["txfre
+0000a080: 7122 5d20 3d20 7365 6c66 2e6e 316d 6d2e  q"] = self.n1mm.
+0000a090: 636f 6e74 6163 745f 696e 666f 5b0a 2020  contact_info[.  
+0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0b0: 2020 2272 7866 7265 7122 0a20 2020 2020    "rxfreq".     
+0000a0c0: 2020 2020 2020 2020 2020 205d 203d 2073             ] = s
+0000a0d0: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
+0000a0e0: 6e66 6f5b 2246 7265 7122 5d0a 2020 2020  nfo["Freq"].    
+0000a0f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a100: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+0000a110: 666f 5b22 6d6f 6465 225d 203d 2073 656c  fo["mode"] = sel
+0000a120: 662e 636f 6e74 6163 745b 224d 6f64 6522  f.contact["Mode"
+0000a130: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000a140: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
+0000a150: 6163 745f 696e 666f 5b22 636f 6e74 6573  act_info["contes
+0000a160: 746e 616d 6522 5d20 3d20 7365 6c66 2e63  tname"] = self.c
+0000a170: 6f6e 7461 6374 5b0a 2020 2020 2020 2020  ontact[.        
+0000a180: 2020 2020 2020 2020 2020 2020 2243 6f6e              "Con
+0000a190: 7465 7374 4e61 6d65 220a 2020 2020 2020  testName".      
+0000a1a0: 2020 2020 2020 2020 2020 5d2e 7265 706c            ].repl
+0000a1b0: 6163 6528 222d 222c 2022 2229 0a20 2020  ace("-", "").   
+0000a1c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a1d0: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a1e0: 6e66 6f5b 2263 6f6e 7465 7374 6e72 225d  nfo["contestnr"]
+0000a1f0: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
+0000a200: 2243 6f6e 7465 7374 4e52 225d 0a20 2020  "ContestNR"].   
+0000a210: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a220: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a230: 6e66 6f5b 2273 7461 7469 6f6e 7072 6566  nfo["stationpref
+0000a240: 6978 225d 203d 2073 656c 662e 636f 6e74  ix"] = self.cont
+0000a250: 6163 745b 2253 7461 7469 6f6e 5072 6566  act["StationPref
+0000a260: 6978 225d 0a20 2020 2020 2020 2020 2020  ix"].           
+0000a270: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000a280: 6f6e 7461 6374 5f69 6e66 6f5b 2277 7078  ontact_info["wpx
+0000a290: 7072 6566 6978 225d 203d 2073 656c 662e  prefix"] = self.
+0000a2a0: 636f 6e74 6163 745b 2257 5058 5072 6566  contact["WPXPref
+0000a2b0: 6978 225d 0a20 2020 2020 2020 2020 2020  ix"].           
+0000a2c0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000a2d0: 6f6e 7461 6374 5f69 6e66 6f5b 2249 7352  ontact_info["IsR
+0000a2e0: 756e 5153 4f22 5d20 3d20 7365 6c66 2e63  unQSO"] = self.c
+0000a2f0: 6f6e 7461 6374 5b22 4973 5275 6e51 534f  ontact["IsRunQSO
+0000a300: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000a310: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+0000a320: 7461 6374 5f69 6e66 6f5b 226f 7065 7261  tact_info["opera
+0000a330: 746f 7222 5d20 3d20 7365 6c66 2e63 6f6e  tor"] = self.con
+0000a340: 7461 6374 5b22 4f70 6572 6174 6f72 225d  tact["Operator"]
+0000a350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a360: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
+0000a370: 6374 5f69 6e66 6f5b 226d 7963 616c 6c22  ct_info["mycall"
+0000a380: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
+0000a390: 5b22 4f70 6572 6174 6f72 225d 0a20 2020  ["Operator"].   
+0000a3a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a3b0: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a3c0: 6e66 6f5b 2253 7461 7469 6f6e 4e61 6d65  nfo["StationName
+0000a3d0: 225d 203d 2073 656c 662e 6e31 6d6d 2e63  "] = self.n1mm.c
+0000a3e0: 6f6e 7461 6374 5f69 6e66 6f5b 0a20 2020  ontact_info[.   
+0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a400: 2022 4e65 7442 696f 734e 616d 6522 0a20   "NetBiosName". 
+0000a410: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+0000a420: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
+0000a430: 224e 6574 4269 6f73 4e61 6d65 225d 0a20  "NetBiosName"]. 
+0000a440: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a450: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
+0000a460: 5f69 6e66 6f5b 2249 734f 7269 6769 6e61  _info["IsOrigina
+0000a470: 6c22 5d20 3d20 7365 6c66 2e63 6f6e 7461  l"] = self.conta
+0000a480: 6374 5b22 4973 4f72 6967 696e 616c 225d  ct["IsOriginal"]
+0000a490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a4a0: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
+0000a4b0: 6374 5f69 6e66 6f5b 2249 4422 5d20 3d20  ct_info["ID"] = 
+0000a4c0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4944  self.contact["ID
+0000a4d0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000a4e0: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+0000a4f0: 7461 6374 5f69 6e66 6f5b 2270 6f69 6e74  tact_info["point
+0000a500: 7322 5d20 3d20 7365 6c66 2e63 6f6e 7461  s"] = self.conta
+0000a510: 6374 5b22 506f 696e 7473 225d 0a20 2020  ct["Points"].   
+0000a520: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a530: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a540: 6e66 6f5b 2273 6e74 225d 203d 2073 656c  nfo["snt"] = sel
+0000a550: 662e 636f 6e74 6163 745b 2253 4e54 225d  f.contact["SNT"]
+0000a560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a570: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
+0000a580: 6374 5f69 6e66 6f5b 2272 6376 225d 203d  ct_info["rcv"] =
+0000a590: 2073 656c 662e 636f 6e74 6163 745b 2252   self.contact["R
+0000a5a0: 4356 225d 0a20 2020 2020 2020 2020 2020  CV"].           
+0000a5b0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000a5c0: 6f6e 7461 6374 5f69 6e66 6f5b 2273 6e74  ontact_info["snt
+0000a5d0: 6e72 225d 203d 2073 656c 662e 636f 6e74  nr"] = self.cont
+0000a5e0: 6163 745b 2253 656e 744e 7222 5d0a 2020  act["SentNr"].  
+0000a5f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a600: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+0000a610: 696e 666f 5b22 7263 766e 7222 5d20 3d20  info["rcvnr"] = 
+0000a620: 7365 6c66 2e63 6f6e 7461 6374 5b22 4e52  self.contact["NR
+0000a630: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000a640: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+0000a650: 7461 6374 5f69 6e66 6f5b 2269 736d 756c  tact_info["ismul
+0000a660: 7469 706c 6965 7231 225d 203d 2073 656c  tiplier1"] = sel
+0000a670: 662e 636f 6e74 6163 742e 6765 7428 0a20  f.contact.get(. 
+0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a690: 2020 2022 4973 4d75 6c74 6970 6c69 6572     "IsMultiplier
+0000a6a0: 3122 2c20 300a 2020 2020 2020 2020 2020  1", 0.          
+0000a6b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000a6c0: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+0000a6d0: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
+0000a6e0: 6973 6d75 6c74 6970 6c69 6572 3222 5d20  ismultiplier2"] 
+0000a6f0: 3d20 7365 6c66 2e63 6f6e 7461 6374 2e67  = self.contact.g
+0000a700: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+0000a710: 2020 2020 2020 2020 2249 734d 756c 7469          "IsMulti
+0000a720: 706c 6965 7232 222c 2030 0a20 2020 2020  plier2", 0.     
+0000a730: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000a740: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a750: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a760: 6e66 6f5b 2269 736d 756c 7469 706c 6965  nfo["ismultiplie
+0000a770: 7233 225d 203d 2073 656c 662e 636f 6e74  r3"] = self.cont
+0000a780: 6163 742e 6765 7428 0a20 2020 2020 2020  act.get(.       
+0000a790: 2020 2020 2020 2020 2020 2020 2022 4973               "Is
+0000a7a0: 4d75 6c74 6970 6c69 6572 3322 2c20 2230  Multiplier3", "0
+0000a7b0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000a7c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000a7d0: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
+0000a7e0: 6e74 6163 745f 696e 666f 5b22 7365 6374  ntact_info["sect
+0000a7f0: 696f 6e22 5d20 3d20 7365 6c66 2e63 6f6e  ion"] = self.con
+0000a800: 7461 6374 5b22 5365 6374 225d 0a20 2020  tact["Sect"].   
+0000a810: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000a820: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000a830: 6e66 6f5b 2270 7265 6322 5d20 3d20 7365  nfo["prec"] = se
+0000a840: 6c66 2e63 6f6e 7461 6374 5b22 5072 6563  lf.contact["Prec
+0000a850: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000a860: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+0000a870: 7461 6374 5f69 6e66 6f5b 2263 6b22 5d20  tact_info["ck"] 
+0000a880: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b22  = self.contact["
+0000a890: 434b 225d 0a20 2020 2020 2020 2020 2020  CK"].           
+0000a8a0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000a8b0: 6f6e 7461 6374 5f69 6e66 6f5b 227a 6e22  ontact_info["zn"
+0000a8c0: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
+0000a8d0: 5b22 5a4e 225d 0a20 2020 2020 2020 2020  ["ZN"].         
+0000a8e0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+0000a8f0: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2270  .contact_info["p
+0000a900: 6f77 6572 225d 203d 2073 656c 662e 636f  ower"] = self.co
+0000a910: 6e74 6163 745b 2250 6f77 6572 225d 0a20  ntact["Power"]. 
+0000a920: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a930: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
+0000a940: 5f69 6e66 6f5b 2262 616e 6422 5d20 3d20  _info["band"] = 
+0000a950: 7365 6c66 2e63 6f6e 7461 6374 5b22 4261  self.contact["Ba
+0000a960: 6e64 225d 0a20 2020 2020 2020 2020 2020  nd"].           
+0000a970: 2020 2020 2023 2073 656c 662e 6e31 6d6d       # self.n1mm
+0000a980: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2727  .contact_info[''
+0000a990: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000a9a0: 2020 2320 7365 6c66 2e6e 316d 6d2e 636f    # self.n1mm.co
+0000a9b0: 6e74 6163 745f 696e 666f 5b27 275d 0a20  ntact_info['']. 
+0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000a9d0: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
+0000a9e0: 6374 5f69 6e66 6f5b 2727 5d0a 2020 2020  ct_info[''].    
+0000a9f0: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+0000aa00: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+0000aa10: 696e 666f 5b27 275d 0a20 2020 2020 2020  info[''].       
+0000aa20: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+0000aa30: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+0000aa40: 6f5b 2727 5d0a 2020 2020 2020 2020 2020  o[''].          
+0000aa50: 2020 2020 2020 2320 7365 6c66 2e6e 316d        # self.n1m
+0000aa60: 6d2e 636f 6e74 6163 745f 696e 666f 5b27  m.contact_info['
+0000aa70: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
+0000aa80: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000aa90: 2225 7322 2c20 6622 7b73 656c 662e 6e31  "%s", f"{self.n1
+0000aaa0: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f7d  mm.contact_info}
+0000aab0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0000aac0: 2020 2073 656c 662e 6e31 6d6d 2e73 656e     self.n1mm.sen
+0000aad0: 645f 636f 6e74 6163 745f 696e 666f 2829  d_contact_info()
+0000aae0: 0a0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+0000aaf0: 6174 6162 6173 652e 6c6f 675f 636f 6e74  atabase.log_cont
+0000ab00: 6163 7428 7365 6c66 2e63 6f6e 7461 6374  act(self.contact
+0000ab10: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000ab20: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
+0000ab30: 2020 2020 2063 6d64 203d 207b 7d0a 2020       cmd = {}.  
+0000ab40: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
+0000ab50: 203d 2022 5550 4441 5445 4c4f 4722 0a20   = "UPDATELOG". 
+0000ab60: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
+0000ab70: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
+0000ab80: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
+0000ab90: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+0000aba0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+0000abb0: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+0000abc0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000abd0: 745b 2243 6f6e 7465 7374 4e61 6d65 225d  t["ContestName"]
+0000abe0: 203d 2073 656c 662e 636f 6e74 6573 742e   = self.contest.
+0000abf0: 6e61 6d65 0a20 2020 2020 2020 2023 2073  name.        # s
+0000ac00: 656c 662e 636f 6e74 6163 745b 2253 4e54  elf.contact["SNT
+0000ac10: 225d 203d 2073 656c 662e 7365 6e74 2e74  "] = self.sent.t
+0000ac20: 6578 7428 290a 2020 2020 2020 2020 2320  ext().        # 
+0000ac30: 7365 6c66 2e63 6f6e 7461 6374 5b22 5243  self.contact["RC
+0000ac40: 5622 5d20 3d20 7365 6c66 2e72 6563 6569  V"] = self.recei
+0000ac50: 7665 2e74 6578 7428 290a 2020 2020 2020  ve.text().      
+0000ac60: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000ac70: 5b22 436f 756e 7472 7950 7265 6669 7822  ["CountryPrefix"
+0000ac80: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+0000ac90: 2e63 6f6e 7461 6374 5b22 5374 6174 696f  .contact["Statio
+0000aca0: 6e50 7265 6669 7822 5d20 3d20 7365 6c66  nPrefix"] = self
+0000acb0: 2e70 7265 662e 6765 7428 2263 616c 6c73  .pref.get("calls
+0000acc0: 6967 6e22 2c20 2222 290a 2020 2020 2020  ign", "").      
+0000acd0: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000ace0: 5b22 5154 4822 5d0a 2020 2020 2020 2020  ["QTH"].        
+0000acf0: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+0000ad00: 4e61 6d65 225d 203d 2073 656c 662e 6f74  Name"] = self.ot
+0000ad10: 6865 725f 312e 7465 7874 2829 0a20 2020  her_1.text().   
+0000ad20: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+0000ad30: 6163 745b 2243 6f6d 6d65 6e74 225d 203d  act["Comment"] =
+0000ad40: 2073 656c 662e 6f74 6865 725f 322e 7465   self.other_2.te
+0000ad50: 7874 2829 0a20 2020 2020 2020 2023 2073  xt().        # s
+0000ad60: 656c 662e 636f 6e74 6163 745b 224e 5222  elf.contact["NR"
+0000ad70: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+0000ad80: 2e63 6f6e 7461 6374 5b22 5365 6374 225d  .contact["Sect"]
+0000ad90: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+0000ada0: 636f 6e74 6163 745b 2250 7265 6322 5d0a  contact["Prec"].
+0000adb0: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+0000adc0: 6f6e 7461 6374 5b22 434b 225d 0a20 2020  ontact["CK"].   
+0000add0: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+0000ade0: 6163 745b 225a 4e22 5d0a 2020 2020 2020  act["ZN"].      
+0000adf0: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000ae00: 5b22 5365 6e74 4e72 225d 0a20 2020 2020  ["SentNr"].     
+0000ae10: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000ae20: 745b 2250 6f69 6e74 7322 5d0a 2020 2020  t["Points"].    
+0000ae30: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+0000ae40: 6374 5b22 4973 4d75 6c74 6970 6c69 6572  ct["IsMultiplier
+0000ae50: 3122 5d0a 2020 2020 2020 2020 2320 7365  1"].        # se
+0000ae60: 6c66 2e63 6f6e 7461 6374 5b22 4973 4d75  lf.contact["IsMu
+0000ae70: 6c74 6970 6c69 6572 3222 5d0a 2020 2020  ltiplier2"].    
+0000ae80: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+0000ae90: 6374 5b22 506f 7765 7222 5d0a 2020 2020  ct["Power"].    
+0000aea0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+0000aeb0: 6374 5b22 4261 6e64 225d 0a20 2020 2020  ct["Band"].     
+0000aec0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000aed0: 745b 2257 5058 5072 6566 6978 225d 203d  t["WPXPrefix"] =
+0000aee0: 2063 616c 6375 6c61 7465 5f77 7078 5f70   calculate_wpx_p
+0000aef0: 7265 6669 7828 7365 6c66 2e63 616c 6c73  refix(self.calls
+0000af00: 6967 6e2e 7465 7874 2829 290a 2020 2020  ign.text()).    
+0000af10: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+0000af20: 6374 5b22 4578 6368 616e 6765 3122 5d0a  ct["Exchange1"].
+0000af30: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+0000af40: 6f6e 7461 6374 5b22 5261 6469 6f4e 5222  ontact["RadioNR"
+0000af50: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+0000af60: 2e63 6f6e 7461 6374 5b22 6973 4d75 6c74  .contact["isMult
+0000af70: 6970 6c69 6572 3322 5d0a 2020 2020 2020  iplier3"].      
+0000af80: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000af90: 5b22 4d69 7363 5465 7874 225d 0a20 2020  ["MiscText"].   
+0000afa0: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+0000afb0: 6163 745b 2243 6f6e 7461 6374 5479 7065  act["ContactType
+0000afc0: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
+0000afd0: 662e 636f 6e74 6163 745b 2252 756e 3152  f.contact["Run1R
+0000afe0: 756e 3222 5d0a 2020 2020 2020 2020 2320  un2"].        # 
+0000aff0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4772  self.contact["Gr
+0000b000: 6964 5371 7561 7265 225d 0a20 2020 2020  idSquare"].     
+0000b010: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000b020: 745b 2243 6f6e 7469 6e65 6e74 225d 0a20  t["Continent"]. 
 0000b030: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-0000b040: 6e74 6163 745b 2242 616e 6422 5d0a 2020  ntact["Band"].  
-0000b050: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-0000b060: 7461 6374 5b22 5750 5850 7265 6669 7822  tact["WPXPrefix"
-0000b070: 5d20 3d20 6361 6c63 756c 6174 655f 7770  ] = calculate_wp
-0000b080: 785f 7072 6566 6978 2873 656c 662e 6361  x_prefix(self.ca
-0000b090: 6c6c 7369 676e 2e74 6578 7428 2929 0a20  llsign.text()). 
-0000b0a0: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-0000b0b0: 6e74 6163 745b 2245 7863 6861 6e67 6531  ntact["Exchange1
-0000b0c0: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
-0000b0d0: 662e 636f 6e74 6163 745b 2252 6164 696f  f.contact["Radio
-0000b0e0: 4e52 225d 0a20 2020 2020 2020 2023 2073  NR"].        # s
-0000b0f0: 656c 662e 636f 6e74 6163 745b 2269 734d  elf.contact["isM
-0000b100: 756c 7469 706c 6965 7233 225d 0a20 2020  ultiplier3"].   
-0000b110: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-0000b120: 6163 745b 224d 6973 6354 6578 7422 5d0a  act["MiscText"].
-0000b130: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-0000b140: 6f6e 7461 6374 5b22 436f 6e74 6163 7454  ontact["ContactT
-0000b150: 7970 6522 5d0a 2020 2020 2020 2020 2320  ype"].        # 
-0000b160: 7365 6c66 2e63 6f6e 7461 6374 5b22 5275  self.contact["Ru
-0000b170: 6e31 5275 6e32 225d 0a20 2020 2020 2020  n1Run2"].       
-0000b180: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-0000b190: 2247 7269 6453 7175 6172 6522 5d0a 2020  "GridSquare"].  
-0000b1a0: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-0000b1b0: 7461 6374 5b22 436f 6e74 696e 656e 7422  tact["Continent"
-0000b1c0: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
-0000b1d0: 2e63 6f6e 7461 6374 5b22 526f 7665 724c  .contact["RoverL
-0000b1e0: 6f63 6174 696f 6e22 5d0a 2020 2020 2020  ocation"].      
-0000b1f0: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-0000b200: 5b22 5261 6469 6f49 6e74 6572 6661 6365  ["RadioInterface
-0000b210: 6422 5d0a 2020 2020 2020 2020 2320 7365  d"].        # se
-0000b220: 6c66 2e63 6f6e 7461 6374 5b22 4e65 7477  lf.contact["Netw
-0000b230: 6f72 6b65 6443 6f6d 704e 7222 5d0a 2020  orkedCompNr"].  
-0000b240: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-0000b250: 7461 6374 5b22 434c 4149 4d45 4451 534f  tact["CLAIMEDQSO
-0000b260: 225d 0a0a 2020 2020 6465 6620 6e65 775f  "]..    def new_
-0000b270: 636f 6e74 6573 745f 6469 616c 6f67 2873  contest_dialog(s
-0000b280: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000b290: 2253 686f 7720 6e65 7720 636f 6e74 6573  "Show new contes
-0000b2a0: 7420 6469 616c 6f67 2222 220a 2020 2020  t dialog""".    
-0000b2b0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000b2c0: 2822 4e65 7720 636f 6e74 6573 7420 4469  ("New contest Di
-0000b2d0: 616c 6f67 2229 0a20 2020 2020 2020 2073  alog").        s
-0000b2e0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-0000b2f0: 6f67 203d 204e 6577 436f 6e74 6573 7428  og = NewContest(
-0000b300: 574f 524b 494e 475f 5041 5448 290a 2020  WORKING_PATH).  
-0000b310: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-0000b320: 7374 5f64 6961 6c6f 672e 6163 6365 7074  st_dialog.accept
-0000b330: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-0000b340: 7361 7665 5f63 6f6e 7465 7374 290a 2020  save_contest).  
-0000b350: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-0000b360: 7374 5f64 6961 6c6f 672e 6461 7465 5469  st_dialog.dateTi
-0000b370: 6d65 4564 6974 2e73 6574 4461 7465 2851  meEdit.setDate(Q
-0000b380: 7443 6f72 652e 5144 6174 652e 6375 7272  tCore.QDate.curr
-0000b390: 656e 7444 6174 6528 2929 0a20 2020 2020  entDate()).     
-0000b3a0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-0000b3b0: 6469 616c 6f67 2e64 6174 6554 696d 6545  dialog.dateTimeE
-0000b3c0: 6469 742e 7365 7443 616c 656e 6461 7250  dit.setCalendarP
-0000b3d0: 6f70 7570 2854 7275 6529 0a20 2020 2020  opup(True).     
-0000b3e0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-0000b3f0: 6469 616c 6f67 2e64 6174 6554 696d 6545  dialog.dateTimeE
-0000b400: 6469 742e 7365 7454 696d 6528 5174 436f  dit.setTime(QtCo
-0000b410: 7265 2e51 5469 6d65 2830 2c20 3029 290a  re.QTime(0, 0)).
-0000b420: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0000b430: 7465 7374 5f64 6961 6c6f 672e 706f 7765  test_dialog.powe
-0000b440: 722e 7365 7443 7572 7265 6e74 5465 7874  r.setCurrentText
-0000b450: 2822 4c4f 5722 290a 2020 2020 2020 2020  ("LOW").        
-0000b460: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-0000b470: 6c6f 672e 7374 6174 696f 6e2e 7365 7443  log.station.setC
-0000b480: 7572 7265 6e74 5465 7874 2822 4649 5845  urrentText("FIXE
-0000b490: 4422 290a 2020 2020 2020 2020 7365 6c66  D").        self
-0000b4a0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-0000b4b0: 6f70 656e 2829 0a0a 2020 2020 6465 6620  open()..    def 
-0000b4c0: 7361 7665 5f63 6f6e 7465 7374 2873 656c  save_contest(sel
-0000b4d0: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
-0000b4e0: 6176 6520 436f 6e74 6573 7422 2222 0a20  ave Contest""". 
-0000b4f0: 2020 2020 2020 206e 6578 745f 6e75 6d62         next_numb
-0000b500: 6572 203d 2073 656c 662e 6461 7461 6261  er = self.databa
-0000b510: 7365 2e67 6574 5f6e 6578 745f 636f 6e74  se.get_next_cont
-0000b520: 6573 745f 6e72 2829 0a20 2020 2020 2020  est_nr().       
-0000b530: 2063 6f6e 7465 7374 203d 207b 7d0a 2020   contest = {}.  
-0000b540: 2020 2020 2020 636f 6e74 6573 745b 2243        contest["C
-0000b550: 6f6e 7465 7374 4e61 6d65 225d 203d 2028  ontestName"] = (
-0000b560: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000b570: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-0000b580: 2e63 6f6e 7465 7374 2e63 7572 7265 6e74  .contest.current
-0000b590: 5465 7874 2829 2e6c 6f77 6572 2829 2e72  Text().lower().r
-0000b5a0: 6570 6c61 6365 2822 2022 2c20 225f 2229  eplace(" ", "_")
-0000b5b0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000b5c0: 2020 2063 6f6e 7465 7374 5b22 5374 6172     contest["Star
-0000b5d0: 7444 6174 6522 5d20 3d20 7365 6c66 2e63  tDate"] = self.c
-0000b5e0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6461  ontest_dialog.da
-0000b5f0: 7465 5469 6d65 4564 6974 2e64 6174 6554  teTimeEdit.dateT
-0000b600: 696d 6528 292e 746f 5374 7269 6e67 280a  ime().toString(.
-0000b610: 2020 2020 2020 2020 2020 2020 2279 7979              "yyy
-0000b620: 792d 4d4d 2d64 6420 6868 3a6d 6d3a 7373  y-MM-dd hh:mm:ss
-0000b630: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
-0000b640: 2020 2020 636f 6e74 6573 745b 224f 7065      contest["Ope
-0000b650: 7261 746f 7243 6174 6567 6f72 7922 5d20  ratorCategory"] 
-0000b660: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-0000b670: 6961 6c6f 672e 6f70 6572 6174 6f72 5f63  ialog.operator_c
-0000b680: 6c61 7373 2e63 7572 7265 6e74 5465 7874  lass.currentText
-0000b690: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
-0000b6a0: 7374 5b22 4261 6e64 4361 7465 676f 7279  st["BandCategory
-0000b6b0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-0000b6c0: 745f 6469 616c 6f67 2e62 616e 642e 6375  t_dialog.band.cu
-0000b6d0: 7272 656e 7454 6578 7428 290a 2020 2020  rrentText().    
-0000b6e0: 2020 2020 636f 6e74 6573 745b 2250 6f77      contest["Pow
-0000b6f0: 6572 4361 7465 676f 7279 225d 203d 2073  erCategory"] = s
-0000b700: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-0000b710: 6f67 2e70 6f77 6572 2e63 7572 7265 6e74  og.power.current
-0000b720: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
-0000b730: 6f6e 7465 7374 5b22 4d6f 6465 4361 7465  ontest["ModeCate
-0000b740: 676f 7279 225d 203d 2073 656c 662e 636f  gory"] = self.co
-0000b750: 6e74 6573 745f 6469 616c 6f67 2e6d 6f64  ntest_dialog.mod
-0000b760: 652e 6375 7272 656e 7454 6578 7428 290a  e.currentText().
-0000b770: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
-0000b780: 224f 7665 726c 6179 4361 7465 676f 7279  "OverlayCategory
-0000b790: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-0000b7a0: 745f 6469 616c 6f67 2e6f 7665 726c 6179  t_dialog.overlay
-0000b7b0: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
-0000b7c0: 2020 2020 2020 2023 2063 6f6e 7465 7374         # contest
-0000b7d0: 5b27 436c 6169 6d65 6453 636f 7265 275d  ['ClaimedScore']
-0000b7e0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-0000b7f0: 6469 616c 6f67 2e0a 2020 2020 2020 2020  dialog..        
-0000b800: 636f 6e74 6573 745b 224f 7065 7261 746f  contest["Operato
-0000b810: 7273 225d 203d 2073 656c 662e 636f 6e74  rs"] = self.cont
-0000b820: 6573 745f 6469 616c 6f67 2e6f 7065 7261  est_dialog.opera
-0000b830: 746f 7273 2e74 6578 7428 290a 2020 2020  tors.text().    
-0000b840: 2020 2020 636f 6e74 6573 745b 2253 6f61      contest["Soa
-0000b850: 7062 6f78 225d 203d 2073 656c 662e 636f  pbox"] = self.co
-0000b860: 6e74 6573 745f 6469 616c 6f67 2e73 6f61  ntest_dialog.soa
-0000b870: 7062 6f78 2e74 6f50 6c61 696e 5465 7874  pbox.toPlainText
-0000b880: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
-0000b890: 7374 5b22 5365 6e74 4578 6368 616e 6765  st["SentExchange
-0000b8a0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-0000b8b0: 745f 6469 616c 6f67 2e65 7863 6861 6e67  t_dialog.exchang
-0000b8c0: 652e 7465 7874 2829 0a20 2020 2020 2020  e.text().       
-0000b8d0: 2063 6f6e 7465 7374 5b22 436f 6e74 6573   contest["Contes
-0000b8e0: 744e 5222 5d20 3d20 6e65 7874 5f6e 756d  tNR"] = next_num
-0000b8f0: 6265 722e 6765 7428 2263 6f75 6e74 222c  ber.get("count",
-0000b900: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
-0000b910: 2e70 7265 665b 2263 6f6e 7465 7374 225d  .pref["contest"]
-0000b920: 203d 206e 6578 745f 6e75 6d62 6572 2e67   = next_number.g
-0000b930: 6574 2822 636f 756e 7422 2c20 3129 0a20  et("count", 1). 
-0000b940: 2020 2020 2020 2023 2063 6f6e 7465 7374         # contest
-0000b950: 5b27 5375 6254 7970 6527 5d20 3d20 7365  ['SubType'] = se
-0000b960: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-0000b970: 672e 0a20 2020 2020 2020 2063 6f6e 7465  g..        conte
-0000b980: 7374 5b22 5374 6174 696f 6e43 6174 6567  st["StationCateg
-0000b990: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
-0000b9a0: 7465 7374 5f64 6961 6c6f 672e 7374 6174  test_dialog.stat
-0000b9b0: 696f 6e2e 6375 7272 656e 7454 6578 7428  ion.currentText(
-0000b9c0: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-0000b9d0: 745b 2241 7373 6973 7465 6443 6174 6567  t["AssistedCateg
-0000b9e0: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
-0000b9f0: 7465 7374 5f64 6961 6c6f 672e 6173 7369  test_dialog.assi
-0000ba00: 7374 6564 2e63 7572 7265 6e74 5465 7874  sted.currentText
-0000ba10: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
-0000ba20: 7374 5b22 5472 616e 736d 6974 7465 7243  st["TransmitterC
-0000ba30: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
-0000ba40: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-0000ba50: 7472 616e 736d 6974 7465 722e 6375 7272  transmitter.curr
-0000ba60: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
-0000ba70: 2020 2320 636f 6e74 6573 745b 2754 696d    # contest['Tim
-0000ba80: 6543 6174 6567 6f72 7927 5d20 3d20 7365  eCategory'] = se
-0000ba90: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-0000baa0: 672e 0a20 2020 2020 2020 206c 6f67 6765  g..        logge
-0000bab0: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
-0000bac0: 7b63 6f6e 7465 7374 7d22 290a 2020 2020  {contest}").    
-0000bad0: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
-0000bae0: 652e 6164 645f 636f 6e74 6573 7428 636f  e.add_contest(co
-0000baf0: 6e74 6573 7429 0a20 2020 2020 2020 2073  ntest).        s
-0000bb00: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
-0000bb10: 656e 6365 2829 0a20 2020 2020 2020 2073  ence().        s
-0000bb20: 656c 662e 6c6f 6164 5f63 6f6e 7465 7374  elf.load_contest
-0000bb30: 2829 0a0a 2020 2020 6465 6620 6564 6974  ()..    def edit
-0000bb40: 5f73 7461 7469 6f6e 5f73 6574 7469 6e67  _station_setting
-0000bb50: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-0000bb60: 2022 2222 5368 6f77 2073 6574 7469 6e67   """Show setting
-0000bb70: 7320 6469 616c 6f67 2222 220a 2020 2020  s dialog""".    
-0000bb80: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000bb90: 2822 5374 6174 696f 6e20 5365 7474 696e  ("Station Settin
-0000bba0: 6773 2073 656c 6563 7465 6422 290a 2020  gs selected").  
-0000bbb0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-0000bbc0: 6e67 735f 6469 616c 6f67 203d 2045 6469  ngs_dialog = Edi
-0000bbd0: 7453 7461 7469 6f6e 2857 4f52 4b49 4e47  tStation(WORKING
-0000bbe0: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
-0000bbf0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000bc00: 6c6f 672e 6163 6365 7074 6564 2e63 6f6e  log.accepted.con
-0000bc10: 6e65 6374 2873 656c 662e 7361 7665 5f73  nect(self.save_s
-0000bc20: 6574 7469 6e67 7329 0a20 2020 2020 2020  ettings).       
-0000bc30: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000bc40: 6961 6c6f 672e 4361 6c6c 2e73 6574 5465  ialog.Call.setTe
-0000bc50: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000bc60: 6765 7428 2243 616c 6c22 2c20 2222 2929  get("Call", ""))
-0000bc70: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000bc80: 7474 696e 6773 5f64 6961 6c6f 672e 4e61  ttings_dialog.Na
-0000bc90: 6d65 2e73 6574 5465 7874 2873 656c 662e  me.setText(self.
-0000bca0: 7374 6174 696f 6e2e 6765 7428 224e 616d  station.get("Nam
-0000bcb0: 6522 2c20 2222 2929 0a20 2020 2020 2020  e", "")).       
-0000bcc0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000bcd0: 6961 6c6f 672e 4164 6472 6573 7331 2e73  ialog.Address1.s
-0000bce0: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
-0000bcf0: 696f 6e2e 6765 7428 2253 7472 6565 7431  ion.get("Street1
-0000bd00: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
-0000bd10: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000bd20: 616c 6f67 2e41 6464 7265 7373 322e 7365  alog.Address2.se
-0000bd30: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
-0000bd40: 6f6e 2e67 6574 2822 5374 7265 6574 3222  on.get("Street2"
-0000bd50: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-0000bd60: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000bd70: 6c6f 672e 4369 7479 2e73 6574 5465 7874  log.City.setText
-0000bd80: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-0000bd90: 7428 2243 6974 7922 2c20 2222 2929 0a20  t("City", "")). 
-0000bda0: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000bdb0: 696e 6773 5f64 6961 6c6f 672e 5374 6174  ings_dialog.Stat
-0000bdc0: 652e 7365 7454 6578 7428 7365 6c66 2e73  e.setText(self.s
-0000bdd0: 7461 7469 6f6e 2e67 6574 2822 5374 6174  tation.get("Stat
-0000bde0: 6522 2c20 2222 2929 0a20 2020 2020 2020  e", "")).       
-0000bdf0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000be00: 6961 6c6f 672e 5a69 702e 7365 7454 6578  ialog.Zip.setTex
-0000be10: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-0000be20: 6574 2822 5a69 7022 2c20 2222 2929 0a20  et("Zip", "")). 
-0000be30: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000be40: 696e 6773 5f64 6961 6c6f 672e 436f 756e  ings_dialog.Coun
-0000be50: 7472 792e 7365 7454 6578 7428 7365 6c66  try.setText(self
-0000be60: 2e73 7461 7469 6f6e 2e67 6574 2822 436f  .station.get("Co
-0000be70: 756e 7472 7922 2c20 2222 2929 0a20 2020  untry", "")).   
-0000be80: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000be90: 6773 5f64 6961 6c6f 672e 4772 6964 5371  gs_dialog.GridSq
-0000bea0: 7561 7265 2e73 6574 5465 7874 2873 656c  uare.setText(sel
-0000beb0: 662e 7374 6174 696f 6e2e 6765 7428 2247  f.station.get("G
-0000bec0: 7269 6453 7175 6172 6522 2c20 2222 2929  ridSquare", ""))
-0000bed0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000bee0: 7474 696e 6773 5f64 6961 6c6f 672e 4351  ttings_dialog.CQ
-0000bef0: 5a6f 6e65 2e73 6574 5465 7874 2873 7472  Zone.setText(str
-0000bf00: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-0000bf10: 7428 2243 515a 6f6e 6522 2c20 2222 2929  t("CQZone", ""))
-0000bf20: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000bf30: 6574 7469 6e67 735f 6469 616c 6f67 2e49  ettings_dialog.I
-0000bf40: 5455 5a6f 6e65 2e73 6574 5465 7874 2873  TUZone.setText(s
-0000bf50: 7472 2873 656c 662e 7374 6174 696f 6e2e  tr(self.station.
-0000bf60: 6765 7428 2249 4152 555a 6f6e 6522 2c20  get("IARUZone", 
-0000bf70: 2222 2929 290a 2020 2020 2020 2020 7365  ""))).        se
-0000bf80: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000bf90: 6f67 2e4c 6963 656e 7365 2e73 6574 5465  og.License.setTe
-0000bfa0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000bfb0: 6765 7428 224c 6963 656e 7365 436c 6173  get("LicenseClas
-0000bfc0: 7322 2c20 2222 2929 0a20 2020 2020 2020  s", "")).       
-0000bfd0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000bfe0: 6961 6c6f 672e 4c61 7469 7475 6465 2e73  ialog.Latitude.s
-0000bff0: 6574 5465 7874 2873 7472 2873 656c 662e  etText(str(self.
-0000c000: 7374 6174 696f 6e2e 6765 7428 224c 6174  station.get("Lat
-0000c010: 6974 7564 6522 2c20 2222 2929 290a 2020  itude", ""))).  
-0000c020: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-0000c030: 6e67 735f 6469 616c 6f67 2e4c 6f6e 6769  ngs_dialog.Longi
-0000c040: 7475 6465 2e73 6574 5465 7874 2873 7472  tude.setText(str
-0000c050: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-0000c060: 7428 224c 6f6e 6769 7475 6465 222c 2022  t("Longitude", "
-0000c070: 2229 2929 0a20 2020 2020 2020 2073 656c  "))).        sel
-0000c080: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000c090: 672e 5374 6174 696f 6e54 5852 582e 7365  g.StationTXRX.se
-0000c0a0: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
-0000c0b0: 6f6e 2e67 6574 2822 7374 6174 696f 6e74  on.get("stationt
-0000c0c0: 7872 7822 2c20 2222 2929 0a20 2020 2020  xrx", "")).     
-0000c0d0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000c0e0: 5f64 6961 6c6f 672e 506f 7765 722e 7365  _dialog.Power.se
-0000c0f0: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
-0000c100: 6f6e 2e67 6574 2822 5350 6f77 6522 2c20  on.get("SPowe", 
-0000c110: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
-0000c120: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000c130: 672e 416e 7465 6e6e 612e 7365 7454 6578  g.Antenna.setTex
-0000c140: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-0000c150: 6574 2822 5341 6e74 6522 2c20 2222 2929  et("SAnte", ""))
-0000c160: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000c170: 7474 696e 6773 5f64 6961 6c6f 672e 416e  ttings_dialog.An
-0000c180: 7448 6569 6768 742e 7365 7454 6578 7428  tHeight.setText(
-0000c190: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-0000c1a0: 2822 5341 6e74 4831 222c 2022 2229 290a  ("SAntH1", "")).
-0000c1b0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000c1c0: 7469 6e67 735f 6469 616c 6f67 2e41 534c  tings_dialog.ASL
-0000c1d0: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-0000c1e0: 6174 696f 6e2e 6765 7428 2253 416e 7448  ation.get("SAntH
-0000c1f0: 3222 2c20 2222 2929 0a20 2020 2020 2020  2", "")).       
-0000c200: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000c210: 6961 6c6f 672e 4152 524c 5365 6374 696f  ialog.ARRLSectio
-0000c220: 6e2e 7365 7454 6578 7428 7365 6c66 2e73  n.setText(self.s
-0000c230: 7461 7469 6f6e 2e67 6574 2822 4152 524c  tation.get("ARRL
-0000c240: 5365 6374 696f 6e22 2c20 2222 2929 0a20  Section", "")). 
-0000c250: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000c260: 696e 6773 5f64 6961 6c6f 672e 526f 7665  ings_dialog.Rove
-0000c270: 7251 5448 2e73 6574 5465 7874 2873 656c  rQTH.setText(sel
-0000c280: 662e 7374 6174 696f 6e2e 6765 7428 2252  f.station.get("R
-0000c290: 6f76 6572 5154 4822 2c20 2222 2929 0a20  overQTH", "")). 
-0000c2a0: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000c2b0: 696e 6773 5f64 6961 6c6f 672e 436c 7562  ings_dialog.Club
-0000c2c0: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-0000c2d0: 6174 696f 6e2e 6765 7428 2243 6c75 6222  ation.get("Club"
-0000c2e0: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-0000c2f0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000c300: 6c6f 672e 456d 6169 6c2e 7365 7454 6578  log.Email.setTex
-0000c310: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-0000c320: 6574 2822 456d 6169 6c22 2c20 2222 2929  et("Email", ""))
-0000c330: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000c340: 7474 696e 6773 5f64 6961 6c6f 672e 6f70  ttings_dialog.op
-0000c350: 656e 2829 0a0a 2020 2020 6465 6620 7361  en()..    def sa
-0000c360: 7665 5f73 6574 7469 6e67 7328 7365 6c66  ve_settings(self
-0000c370: 293a 0a20 2020 2020 2020 2022 2222 5361  ):.        """Sa
-0000c380: 7665 2073 6574 7469 6e67 7322 2222 0a20  ve settings""". 
-0000c390: 2020 2020 2020 2063 7320 3d20 7365 6c66         cs = self
-0000c3a0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000c3b0: 2e43 616c 6c2e 7465 7874 2829 0a20 2020  .Call.text().   
-0000c3c0: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000c3d0: 6e20 3d20 7b7d 0a20 2020 2020 2020 2073  n = {}.        s
-0000c3e0: 656c 662e 7374 6174 696f 6e5b 2243 616c  elf.station["Cal
-0000c3f0: 6c22 5d20 3d20 6373 2e75 7070 6572 2829  l"] = cs.upper()
-0000c400: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000c410: 6174 696f 6e5b 224e 616d 6522 5d20 3d20  ation["Name"] = 
-0000c420: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000c430: 616c 6f67 2e4e 616d 652e 7465 7874 2829  alog.Name.text()
-0000c440: 2e74 6974 6c65 2829 0a20 2020 2020 2020  .title().       
-0000c450: 2073 656c 662e 7374 6174 696f 6e5b 2253   self.station["S
-0000c460: 7472 6565 7431 225d 203d 2073 656c 662e  treet1"] = self.
-0000c470: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000c480: 4164 6472 6573 7331 2e74 6578 7428 292e  Address1.text().
-0000c490: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
-0000c4a0: 7365 6c66 2e73 7461 7469 6f6e 5b22 5374  self.station["St
-0000c4b0: 7265 6574 3222 5d20 3d20 7365 6c66 2e73  reet2"] = self.s
-0000c4c0: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
-0000c4d0: 6464 7265 7373 322e 7465 7874 2829 2e74  ddress2.text().t
-0000c4e0: 6974 6c65 2829 0a20 2020 2020 2020 2073  itle().        s
-0000c4f0: 656c 662e 7374 6174 696f 6e5b 2243 6974  elf.station["Cit
-0000c500: 7922 5d20 3d20 7365 6c66 2e73 6574 7469  y"] = self.setti
-0000c510: 6e67 735f 6469 616c 6f67 2e43 6974 792e  ngs_dialog.City.
-0000c520: 7465 7874 2829 2e74 6974 6c65 2829 0a20  text().title(). 
-0000c530: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000c540: 696f 6e5b 2253 7461 7465 225d 203d 2073  ion["State"] = s
-0000c550: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000c560: 6c6f 672e 5374 6174 652e 7465 7874 2829  log.State.text()
-0000c570: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
-0000c580: 2073 656c 662e 7374 6174 696f 6e5b 225a   self.station["Z
-0000c590: 6970 225d 203d 2073 656c 662e 7365 7474  ip"] = self.sett
-0000c5a0: 696e 6773 5f64 6961 6c6f 672e 5a69 702e  ings_dialog.Zip.
-0000c5b0: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-0000c5c0: 656c 662e 7374 6174 696f 6e5b 2243 6f75  elf.station["Cou
-0000c5d0: 6e74 7279 225d 203d 2073 656c 662e 7365  ntry"] = self.se
-0000c5e0: 7474 696e 6773 5f64 6961 6c6f 672e 436f  ttings_dialog.Co
-0000c5f0: 756e 7472 792e 7465 7874 2829 2e74 6974  untry.text().tit
-0000c600: 6c65 2829 0a20 2020 2020 2020 2073 656c  le().        sel
-0000c610: 662e 7374 6174 696f 6e5b 2247 7269 6453  f.station["GridS
-0000c620: 7175 6172 6522 5d20 3d20 7365 6c66 2e73  quare"] = self.s
-0000c630: 6574 7469 6e67 735f 6469 616c 6f67 2e47  ettings_dialog.G
-0000c640: 7269 6453 7175 6172 652e 7465 7874 2829  ridSquare.text()
-0000c650: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000c660: 6174 696f 6e5b 2243 515a 6f6e 6522 5d20  ation["CQZone"] 
-0000c670: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-0000c680: 6469 616c 6f67 2e43 515a 6f6e 652e 7465  dialog.CQZone.te
-0000c690: 7874 2829 0a20 2020 2020 2020 2073 656c  xt().        sel
-0000c6a0: 662e 7374 6174 696f 6e5b 2249 4152 555a  f.station["IARUZ
-0000c6b0: 6f6e 6522 5d20 3d20 7365 6c66 2e73 6574  one"] = self.set
-0000c6c0: 7469 6e67 735f 6469 616c 6f67 2e49 5455  tings_dialog.ITU
-0000c6d0: 5a6f 6e65 2e74 6578 7428 290a 2020 2020  Zone.text().    
-0000c6e0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-0000c6f0: 5b22 4c69 6365 6e73 6543 6c61 7373 225d  ["LicenseClass"]
-0000c700: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-0000c710: 5f64 6961 6c6f 672e 4c69 6365 6e73 652e  _dialog.License.
-0000c720: 7465 7874 2829 2e74 6974 6c65 2829 0a20  text().title(). 
-0000c730: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000c740: 696f 6e5b 224c 6174 6974 7564 6522 5d20  ion["Latitude"] 
-0000c750: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-0000c760: 6469 616c 6f67 2e4c 6174 6974 7564 652e  dialog.Latitude.
-0000c770: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-0000c780: 656c 662e 7374 6174 696f 6e5b 224c 6f6e  elf.station["Lon
-0000c790: 6769 7475 6465 225d 203d 2073 656c 662e  gitude"] = self.
-0000c7a0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000c7b0: 4c6f 6e67 6974 7564 652e 7465 7874 2829  Longitude.text()
-0000c7c0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000c7d0: 6174 696f 6e5b 2253 5458 6571 225d 203d  ation["STXeq"] =
-0000c7e0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000c7f0: 6961 6c6f 672e 5374 6174 696f 6e54 5852  ialog.StationTXR
-0000c800: 582e 7465 7874 2829 0a20 2020 2020 2020  X.text().       
-0000c810: 2073 656c 662e 7374 6174 696f 6e5b 2253   self.station["S
-0000c820: 506f 7765 225d 203d 2073 656c 662e 7365  Powe"] = self.se
-0000c830: 7474 696e 6773 5f64 6961 6c6f 672e 506f  ttings_dialog.Po
-0000c840: 7765 722e 7465 7874 2829 0a20 2020 2020  wer.text().     
-0000c850: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
-0000c860: 2253 416e 7465 225d 203d 2073 656c 662e  "SAnte"] = self.
-0000c870: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000c880: 416e 7465 6e6e 612e 7465 7874 2829 0a20  Antenna.text(). 
-0000c890: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000c8a0: 696f 6e5b 2253 416e 7448 3122 5d20 3d20  ion["SAntH1"] = 
-0000c8b0: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000c8c0: 616c 6f67 2e41 6e74 4865 6967 6874 2e74  alog.AntHeight.t
-0000c8d0: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
-0000c8e0: 6c66 2e73 7461 7469 6f6e 5b22 5341 6e74  lf.station["SAnt
-0000c8f0: 4832 225d 203d 2073 656c 662e 7365 7474  H2"] = self.sett
-0000c900: 696e 6773 5f64 6961 6c6f 672e 4153 4c2e  ings_dialog.ASL.
-0000c910: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-0000c920: 656c 662e 7374 6174 696f 6e5b 2241 5252  elf.station["ARR
-0000c930: 4c53 6563 7469 6f6e 225d 203d 2073 656c  LSection"] = sel
-0000c940: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000c950: 672e 4152 524c 5365 6374 696f 6e2e 7465  g.ARRLSection.te
-0000c960: 7874 2829 2e75 7070 6572 2829 0a20 2020  xt().upper().   
-0000c970: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000c980: 6e5b 2252 6f76 6572 5154 4822 5d20 3d20  n["RoverQTH"] = 
-0000c990: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000c9a0: 616c 6f67 2e52 6f76 6572 5154 482e 7465  alog.RoverQTH.te
-0000c9b0: 7874 2829 0a20 2020 2020 2020 2073 656c  xt().        sel
-0000c9c0: 662e 7374 6174 696f 6e5b 2243 6c75 6222  f.station["Club"
-0000c9d0: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
-0000c9e0: 735f 6469 616c 6f67 2e43 6c75 622e 7465  s_dialog.Club.te
-0000c9f0: 7874 2829 2e74 6974 6c65 2829 0a20 2020  xt().title().   
-0000ca00: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000ca10: 6e5b 2245 6d61 696c 225d 203d 2073 656c  n["Email"] = sel
-0000ca20: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000ca30: 672e 456d 6169 6c2e 7465 7874 2829 0a20  g.Email.text(). 
-0000ca40: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-0000ca50: 6261 7365 2e61 6464 5f73 7461 7469 6f6e  base.add_station
-0000ca60: 2873 656c 662e 7374 6174 696f 6e29 0a20  (self.station). 
-0000ca70: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000ca80: 696e 6773 5f64 6961 6c6f 672e 636c 6f73  ings_dialog.clos
-0000ca90: 6528 290a 2020 2020 2020 2020 6966 2073  e().        if s
-0000caa0: 656c 662e 6375 7272 656e 745f 6f70 203d  elf.current_op =
-0000cab0: 3d20 2222 3a0a 2020 2020 2020 2020 2020  = "":.          
-0000cac0: 2020 7365 6c66 2e63 7572 7265 6e74 5f6f    self.current_o
-0000cad0: 7020 3d20 7365 6c66 2e73 7461 7469 6f6e  p = self.station
-0000cae0: 2e67 6574 2822 4361 6c6c 222c 2022 2229  .get("Call", "")
-0000caf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000cb00: 662e 6d61 6b65 5f6f 705f 6469 7228 290a  f.make_op_dir().
-0000cb10: 2020 2020 2020 2020 636f 6e74 6573 745f          contest_
-0000cb20: 636f 756e 7420 3d20 7365 6c66 2e64 6174  count = self.dat
-0000cb30: 6162 6173 652e 6665 7463 685f 616c 6c5f  abase.fetch_all_
-0000cb40: 636f 6e74 6573 7473 2829 0a20 2020 2020  contests().     
-0000cb50: 2020 2069 6620 6c65 6e28 636f 6e74 6573     if len(contes
-0000cb60: 745f 636f 756e 7429 203d 3d20 303a 0a20  t_count) == 0:. 
-0000cb70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cb80: 6e65 775f 636f 6e74 6573 745f 6469 616c  new_contest_dial
-0000cb90: 6f67 2829 0a0a 2020 2020 6465 6620 6564  og()..    def ed
-0000cba0: 6974 5f6d 6163 726f 2873 656c 662c 2066  it_macro(self, f
-0000cbb0: 756e 6374 696f 6e5f 6b65 7929 3a0a 2020  unction_key):.  
-0000cbc0: 2020 2020 2020 2222 2253 686f 7720 6564        """Show ed
-0000cbd0: 6974 206d 6163 726f 2064 6961 6c6f 6722  it macro dialog"
-0000cbe0: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-0000cbf0: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
-0000cc00: 6720 3d20 4564 6974 4d61 6372 6f28 6675  g = EditMacro(fu
-0000cc10: 6e63 7469 6f6e 5f6b 6579 2c20 574f 524b  nction_key, WORK
-0000cc20: 494e 475f 5041 5448 290a 2020 2020 2020  ING_PATH).      
-0000cc30: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
-0000cc40: 6f5f 6469 616c 6f67 2e61 6363 6570 7465  o_dialog.accepte
-0000cc50: 642e 636f 6e6e 6563 7428 7365 6c66 2e65  d.connect(self.e
-0000cc60: 6469 7465 645f 6d61 6372 6f29 0a20 2020  dited_macro).   
-0000cc70: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-0000cc80: 6163 726f 5f64 6961 6c6f 672e 6f70 656e  acro_dialog.open
-0000cc90: 2829 0a0a 2020 2020 6465 6620 6564 6974  ()..    def edit
-0000cca0: 6564 5f6d 6163 726f 2873 656c 6629 3a0a  ed_macro(self):.
-0000ccb0: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
-0000ccc0: 6564 6974 6564 206d 6163 726f 2222 220a  edited macro""".
-0000ccd0: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
-0000cce0: 745f 6d61 6372 6f5f 6469 616c 6f67 2e66  t_macro_dialog.f
-0000ccf0: 756e 6374 696f 6e5f 6b65 792e 7365 7454  unction_key.setT
-0000cd00: 6578 7428 0a20 2020 2020 2020 2020 2020  ext(.           
-0000cd10: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000cd20: 5f64 6961 6c6f 672e 6d61 6372 6f5f 6c61  _dialog.macro_la
-0000cd30: 6265 6c2e 7465 7874 2829 0a20 2020 2020  bel.text().     
-0000cd40: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-0000cd50: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
-0000cd60: 6c6f 672e 6675 6e63 7469 6f6e 5f6b 6579  log.function_key
-0000cd70: 2e73 6574 546f 6f6c 5469 7028 0a20 2020  .setToolTip(.   
-0000cd80: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
-0000cd90: 6974 5f6d 6163 726f 5f64 6961 6c6f 672e  it_macro_dialog.
-0000cda0: 7468 655f 6d61 6372 6f2e 7465 7874 2829  the_macro.text()
-0000cdb0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000cdc0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000cdd0: 726f 5f64 6961 6c6f 672e 636c 6f73 6528  ro_dialog.close(
-0000cde0: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-0000cdf0: 4631 2873 656c 6629 3a0a 2020 2020 2020  F1(self):.      
-0000ce00: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000ce10: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000ce20: 6728 2246 3120 5269 6768 7420 436c 6963  g("F1 Right Clic
-0000ce30: 6b65 642e 2229 0a20 2020 2020 2020 2073  ked.").        s
-0000ce40: 656c 662e 6564 6974 5f6d 6163 726f 2873  elf.edit_macro(s
-0000ce50: 656c 662e 4631 290a 0a20 2020 2064 6566  elf.F1)..    def
-0000ce60: 2065 6469 745f 4632 2873 656c 6629 3a0a   edit_F2(self):.
-0000ce70: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000ce80: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000ce90: 722e 6465 6275 6728 2246 3220 5269 6768  r.debug("F2 Righ
-0000cea0: 7420 436c 6963 6b65 642e 2229 0a20 2020  t Clicked.").   
-0000ceb0: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-0000cec0: 6163 726f 2873 656c 662e 4632 290a 0a20  acro(self.F2).. 
-0000ced0: 2020 2064 6566 2065 6469 745f 4633 2873     def edit_F3(s
-0000cee0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000cef0: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000cf00: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000cf10: 3320 5269 6768 7420 436c 6963 6b65 642e  3 Right Clicked.
-0000cf20: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000cf30: 6564 6974 5f6d 6163 726f 2873 656c 662e  edit_macro(self.
-0000cf40: 4633 290a 0a20 2020 2064 6566 2065 6469  F3)..    def edi
-0000cf50: 745f 4634 2873 656c 6629 3a0a 2020 2020  t_F4(self):.    
-0000cf60: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000cf70: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000cf80: 6275 6728 2246 3420 5269 6768 7420 436c  bug("F4 Right Cl
-0000cf90: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
-0000cfa0: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000cfb0: 2873 656c 662e 4634 290a 0a20 2020 2064  (self.F4)..    d
-0000cfc0: 6566 2065 6469 745f 4635 2873 656c 6629  ef edit_F5(self)
-0000cfd0: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000cfe0: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000cff0: 6765 722e 6465 6275 6728 2246 3520 5269  ger.debug("F5 Ri
-0000d000: 6768 7420 436c 6963 6b65 642e 2229 0a20  ght Clicked."). 
-0000d010: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000d020: 5f6d 6163 726f 2873 656c 662e 4635 290a  _macro(self.F5).
-0000d030: 0a20 2020 2064 6566 2065 6469 745f 4636  .    def edit_F6
-0000d040: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000d050: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000d060: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000d070: 2246 3620 5269 6768 7420 436c 6963 6b65  "F6 Right Clicke
-0000d080: 642e 2229 0a20 2020 2020 2020 2073 656c  d.").        sel
-0000d090: 662e 6564 6974 5f6d 6163 726f 2873 656c  f.edit_macro(sel
-0000d0a0: 662e 4636 290a 0a20 2020 2064 6566 2065  f.F6)..    def e
-0000d0b0: 6469 745f 4637 2873 656c 6629 3a0a 2020  dit_F7(self):.  
-0000d0c0: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000d0d0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000d0e0: 6465 6275 6728 2246 3720 5269 6768 7420  debug("F7 Right 
-0000d0f0: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
-0000d100: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000d110: 726f 2873 656c 662e 4637 290a 0a20 2020  ro(self.F7)..   
-0000d120: 2064 6566 2065 6469 745f 4638 2873 656c   def edit_F8(sel
-0000d130: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000d140: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000d150: 6f67 6765 722e 6465 6275 6728 2246 3820  ogger.debug("F8 
-0000d160: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
-0000d170: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-0000d180: 6974 5f6d 6163 726f 2873 656c 662e 4638  it_macro(self.F8
-0000d190: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-0000d1a0: 4639 2873 656c 6629 3a0a 2020 2020 2020  F9(self):.      
-0000d1b0: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000d1c0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000d1d0: 6728 2246 3920 5269 6768 7420 436c 6963  g("F9 Right Clic
-0000d1e0: 6b65 642e 2229 0a20 2020 2020 2020 2073  ked.").        s
-0000d1f0: 656c 662e 6564 6974 5f6d 6163 726f 2873  elf.edit_macro(s
-0000d200: 656c 662e 4639 290a 0a20 2020 2064 6566  elf.F9)..    def
-0000d210: 2065 6469 745f 4631 3028 7365 6c66 293a   edit_F10(self):
-0000d220: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
-0000d230: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
-0000d240: 6572 2e64 6562 7567 2822 4631 3020 5269  er.debug("F10 Ri
-0000d250: 6768 7420 436c 6963 6b65 642e 2229 0a20  ght Clicked."). 
-0000d260: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000d270: 5f6d 6163 726f 2873 656c 662e 4631 3029  _macro(self.F10)
-0000d280: 0a0a 2020 2020 6465 6620 6564 6974 5f46  ..    def edit_F
-0000d290: 3131 2873 656c 6629 3a0a 2020 2020 2020  11(self):.      
-0000d2a0: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000d2b0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000d2c0: 6728 2246 3131 2052 6967 6874 2043 6c69  g("F11 Right Cli
-0000d2d0: 636b 6564 2e22 290a 2020 2020 2020 2020  cked.").        
-0000d2e0: 7365 6c66 2e65 6469 745f 6d61 6372 6f28  self.edit_macro(
-0000d2f0: 7365 6c66 2e46 3131 290a 0a20 2020 2064  self.F11)..    d
-0000d300: 6566 2065 6469 745f 4631 3228 7365 6c66  ef edit_F12(self
-0000d310: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
-0000d320: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
-0000d330: 6767 6572 2e64 6562 7567 2822 4631 3220  gger.debug("F12 
-0000d340: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
-0000d350: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-0000d360: 6974 5f6d 6163 726f 2873 656c 662e 4631  it_macro(self.F1
-0000d370: 3229 0a0a 2020 2020 6465 6620 7072 6f63  2)..    def proc
-0000d380: 6573 735f 6d61 6372 6f28 7365 6c66 2c20  ess_macro(self, 
-0000d390: 6d61 6372 6f3a 2073 7472 2920 2d3e 2073  macro: str) -> s
-0000d3a0: 7472 3a0a 2020 2020 2020 2020 2222 2250  tr:.        """P
-0000d3b0: 726f 6365 7373 2043 5720 6d61 6372 6f20  rocess CW macro 
-0000d3c0: 7375 6273 7469 7475 7469 6f6e 7322 2222  substitutions"""
-0000d3d0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0000d3e0: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
-0000d3f0: 6765 745f 7365 7269 616c 2829 0a20 2020  get_serial().   
-0000d400: 2020 2020 206e 6578 745f 7365 7269 616c       next_serial
-0000d410: 203d 2073 7472 2872 6573 756c 742e 6765   = str(result.ge
-0000d420: 7428 2273 6572 6961 6c5f 6e72 222c 2022  t("serial_nr", "
-0000d430: 3122 2929 0a20 2020 2020 2020 2069 6620  1")).        if 
-0000d440: 6e65 7874 5f73 6572 6961 6c20 3d3d 2022  next_serial == "
-0000d450: 4e6f 6e65 223a 0a20 2020 2020 2020 2020  None":.         
-0000d460: 2020 206e 6578 745f 7365 7269 616c 203d     next_serial =
-0000d470: 2022 3122 0a20 2020 2020 2020 206d 6163   "1".        mac
-0000d480: 726f 203d 206d 6163 726f 2e75 7070 6572  ro = macro.upper
-0000d490: 2829 0a20 2020 2020 2020 206d 6163 726f  ().        macro
-0000d4a0: 203d 206d 6163 726f 2e72 6570 6c61 6365   = macro.replace
-0000d4b0: 2822 2322 2c20 6e65 7874 5f73 6572 6961  ("#", next_seria
-0000d4c0: 6c29 0a20 2020 2020 2020 206d 6163 726f  l).        macro
+0000b040: 6e74 6163 745b 2252 6f76 6572 4c6f 6361  ntact["RoverLoca
+0000b050: 7469 6f6e 225d 0a20 2020 2020 2020 2023  tion"].        #
+0000b060: 2073 656c 662e 636f 6e74 6163 745b 2252   self.contact["R
+0000b070: 6164 696f 496e 7465 7266 6163 6564 225d  adioInterfaced"]
+0000b080: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+0000b090: 636f 6e74 6163 745b 224e 6574 776f 726b  contact["Network
+0000b0a0: 6564 436f 6d70 4e72 225d 0a20 2020 2020  edCompNr"].     
+0000b0b0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000b0c0: 745b 2243 4c41 494d 4544 5153 4f22 5d0a  t["CLAIMEDQSO"].
+0000b0d0: 0a20 2020 2064 6566 206e 6577 5f63 6f6e  .    def new_con
+0000b0e0: 7465 7374 5f64 6961 6c6f 6728 7365 6c66  test_dialog(self
+0000b0f0: 293a 0a20 2020 2020 2020 2022 2222 5368  ):.        """Sh
+0000b100: 6f77 206e 6577 2063 6f6e 7465 7374 2064  ow new contest d
+0000b110: 6961 6c6f 6722 2222 0a20 2020 2020 2020  ialog""".       
+0000b120: 206c 6f67 6765 722e 6465 6275 6728 224e   logger.debug("N
+0000b130: 6577 2063 6f6e 7465 7374 2044 6961 6c6f  ew contest Dialo
+0000b140: 6722 290a 2020 2020 2020 2020 7365 6c66  g").        self
+0000b150: 2e63 6f6e 7465 7374 5f64 6961 6c6f 6720  .contest_dialog 
+0000b160: 3d20 4e65 7743 6f6e 7465 7374 2857 4f52  = NewContest(WOR
+0000b170: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
+0000b180: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+0000b190: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
+0000b1a0: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
+0000b1b0: 655f 636f 6e74 6573 7429 0a20 2020 2020  e_contest).     
+0000b1c0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+0000b1d0: 6469 616c 6f67 2e64 6174 6554 696d 6545  dialog.dateTimeE
+0000b1e0: 6469 742e 7365 7444 6174 6528 5174 436f  dit.setDate(QtCo
+0000b1f0: 7265 2e51 4461 7465 2e63 7572 7265 6e74  re.QDate.current
+0000b200: 4461 7465 2829 290a 2020 2020 2020 2020  Date()).        
+0000b210: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+0000b220: 6c6f 672e 6461 7465 5469 6d65 4564 6974  log.dateTimeEdit
+0000b230: 2e73 6574 4361 6c65 6e64 6172 506f 7075  .setCalendarPopu
+0000b240: 7028 5472 7565 290a 2020 2020 2020 2020  p(True).        
+0000b250: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+0000b260: 6c6f 672e 6461 7465 5469 6d65 4564 6974  log.dateTimeEdit
+0000b270: 2e73 6574 5469 6d65 2851 7443 6f72 652e  .setTime(QtCore.
+0000b280: 5154 696d 6528 302c 2030 2929 0a20 2020  QTime(0, 0)).   
+0000b290: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+0000b2a0: 745f 6469 616c 6f67 2e70 6f77 6572 2e73  t_dialog.power.s
+0000b2b0: 6574 4375 7272 656e 7454 6578 7428 224c  etCurrentText("L
+0000b2c0: 4f57 2229 0a20 2020 2020 2020 2073 656c  OW").        sel
+0000b2d0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+0000b2e0: 2e73 7461 7469 6f6e 2e73 6574 4375 7272  .station.setCurr
+0000b2f0: 656e 7454 6578 7428 2246 4958 4544 2229  entText("FIXED")
+0000b300: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0000b310: 6e74 6573 745f 6469 616c 6f67 2e6f 7065  ntest_dialog.ope
+0000b320: 6e28 290a 0a20 2020 2064 6566 2073 6176  n()..    def sav
+0000b330: 655f 636f 6e74 6573 7428 7365 6c66 293a  e_contest(self):
+0000b340: 0a20 2020 2020 2020 2022 2222 5361 7665  .        """Save
+0000b350: 2043 6f6e 7465 7374 2222 220a 2020 2020   Contest""".    
+0000b360: 2020 2020 6e65 7874 5f6e 756d 6265 7220      next_number 
+0000b370: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
+0000b380: 6765 745f 6e65 7874 5f63 6f6e 7465 7374  get_next_contest
+0000b390: 5f6e 7228 290a 2020 2020 2020 2020 636f  _nr().        co
+0000b3a0: 6e74 6573 7420 3d20 7b7d 0a20 2020 2020  ntest = {}.     
+0000b3b0: 2020 2063 6f6e 7465 7374 5b22 436f 6e74     contest["Cont
+0000b3c0: 6573 744e 616d 6522 5d20 3d20 280a 2020  estName"] = (.  
+0000b3d0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000b3e0: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
+0000b3f0: 6e74 6573 742e 6375 7272 656e 7454 6578  ntest.currentTex
+0000b400: 7428 292e 6c6f 7765 7228 292e 7265 706c  t().lower().repl
+0000b410: 6163 6528 2220 222c 2022 5f22 290a 2020  ace(" ", "_").  
+0000b420: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000b430: 636f 6e74 6573 745b 2253 7461 7274 4461  contest["StartDa
+0000b440: 7465 225d 203d 2073 656c 662e 636f 6e74  te"] = self.cont
+0000b450: 6573 745f 6469 616c 6f67 2e64 6174 6554  est_dialog.dateT
+0000b460: 696d 6545 6469 742e 6461 7465 5469 6d65  imeEdit.dateTime
+0000b470: 2829 2e74 6f53 7472 696e 6728 0a20 2020  ().toString(.   
+0000b480: 2020 2020 2020 2020 2022 7979 7979 2d4d           "yyyy-M
+0000b490: 4d2d 6464 2068 683a 6d6d 3a73 7322 0a20  M-dd hh:mm:ss". 
+0000b4a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000b4b0: 2063 6f6e 7465 7374 5b22 4f70 6572 6174   contest["Operat
+0000b4c0: 6f72 4361 7465 676f 7279 225d 203d 2073  orCategory"] = s
+0000b4d0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+0000b4e0: 6f67 2e6f 7065 7261 746f 725f 636c 6173  og.operator_clas
+0000b4f0: 732e 6375 7272 656e 7454 6578 7428 290a  s.currentText().
+0000b500: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+0000b510: 2242 616e 6443 6174 6567 6f72 7922 5d20  "BandCategory"] 
+0000b520: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+0000b530: 6961 6c6f 672e 6261 6e64 2e63 7572 7265  ialog.band.curre
+0000b540: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
+0000b550: 2063 6f6e 7465 7374 5b22 506f 7765 7243   contest["PowerC
+0000b560: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
+0000b570: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+0000b580: 706f 7765 722e 6375 7272 656e 7454 6578  power.currentTex
+0000b590: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
+0000b5a0: 6573 745b 224d 6f64 6543 6174 6567 6f72  est["ModeCategor
+0000b5b0: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
+0000b5c0: 7374 5f64 6961 6c6f 672e 6d6f 6465 2e63  st_dialog.mode.c
+0000b5d0: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
+0000b5e0: 2020 2020 2063 6f6e 7465 7374 5b22 4f76       contest["Ov
+0000b5f0: 6572 6c61 7943 6174 6567 6f72 7922 5d20  erlayCategory"] 
+0000b600: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+0000b610: 6961 6c6f 672e 6f76 6572 6c61 792e 6375  ialog.overlay.cu
+0000b620: 7272 656e 7454 6578 7428 290a 2020 2020  rrentText().    
+0000b630: 2020 2020 2320 636f 6e74 6573 745b 2743      # contest['C
+0000b640: 6c61 696d 6564 5363 6f72 6527 5d20 3d20  laimedScore'] = 
+0000b650: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+0000b660: 6c6f 672e 0a20 2020 2020 2020 2063 6f6e  log..        con
+0000b670: 7465 7374 5b22 4f70 6572 6174 6f72 7322  test["Operators"
+0000b680: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+0000b690: 5f64 6961 6c6f 672e 6f70 6572 6174 6f72  _dialog.operator
+0000b6a0: 732e 7465 7874 2829 0a20 2020 2020 2020  s.text().       
+0000b6b0: 2063 6f6e 7465 7374 5b22 536f 6170 626f   contest["Soapbo
+0000b6c0: 7822 5d20 3d20 7365 6c66 2e63 6f6e 7465  x"] = self.conte
+0000b6d0: 7374 5f64 6961 6c6f 672e 736f 6170 626f  st_dialog.soapbo
+0000b6e0: 782e 746f 506c 6169 6e54 6578 7428 290a  x.toPlainText().
+0000b6f0: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+0000b700: 2253 656e 7445 7863 6861 6e67 6522 5d20  "SentExchange"] 
+0000b710: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+0000b720: 6961 6c6f 672e 6578 6368 616e 6765 2e74  ialog.exchange.t
+0000b730: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+0000b740: 6e74 6573 745b 2243 6f6e 7465 7374 4e52  ntest["ContestNR
+0000b750: 225d 203d 206e 6578 745f 6e75 6d62 6572  "] = next_number
+0000b760: 2e67 6574 2822 636f 756e 7422 2c20 3129  .get("count", 1)
+0000b770: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
+0000b780: 6566 5b22 636f 6e74 6573 7422 5d20 3d20  ef["contest"] = 
+0000b790: 6e65 7874 5f6e 756d 6265 722e 6765 7428  next_number.get(
+0000b7a0: 2263 6f75 6e74 222c 2031 290a 2020 2020  "count", 1).    
+0000b7b0: 2020 2020 2320 636f 6e74 6573 745b 2753      # contest['S
+0000b7c0: 7562 5479 7065 275d 203d 2073 656c 662e  ubType'] = self.
+0000b7d0: 636f 6e74 6573 745f 6469 616c 6f67 2e0a  contest_dialog..
+0000b7e0: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+0000b7f0: 2253 7461 7469 6f6e 4361 7465 676f 7279  "StationCategory
+0000b800: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+0000b810: 745f 6469 616c 6f67 2e73 7461 7469 6f6e  t_dialog.station
+0000b820: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
+0000b830: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
+0000b840: 4173 7369 7374 6564 4361 7465 676f 7279  AssistedCategory
+0000b850: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+0000b860: 745f 6469 616c 6f67 2e61 7373 6973 7465  t_dialog.assiste
+0000b870: 642e 6375 7272 656e 7454 6578 7428 290a  d.currentText().
+0000b880: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+0000b890: 2254 7261 6e73 6d69 7474 6572 4361 7465  "TransmitterCate
+0000b8a0: 676f 7279 225d 203d 2073 656c 662e 636f  gory"] = self.co
+0000b8b0: 6e74 6573 745f 6469 616c 6f67 2e74 7261  ntest_dialog.tra
+0000b8c0: 6e73 6d69 7474 6572 2e63 7572 7265 6e74  nsmitter.current
+0000b8d0: 5465 7874 2829 0a20 2020 2020 2020 2023  Text().        #
+0000b8e0: 2063 6f6e 7465 7374 5b27 5469 6d65 4361   contest['TimeCa
+0000b8f0: 7465 676f 7279 275d 203d 2073 656c 662e  tegory'] = self.
+0000b900: 636f 6e74 6573 745f 6469 616c 6f67 2e0a  contest_dialog..
+0000b910: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000b920: 6562 7567 2822 2573 222c 2066 227b 636f  ebug("%s", f"{co
+0000b930: 6e74 6573 747d 2229 0a20 2020 2020 2020  ntest}").       
+0000b940: 2073 656c 662e 6461 7461 6261 7365 2e61   self.database.a
+0000b950: 6464 5f63 6f6e 7465 7374 2863 6f6e 7465  dd_contest(conte
+0000b960: 7374 290a 2020 2020 2020 2020 7365 6c66  st).        self
+0000b970: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
+0000b980: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+0000b990: 2e6c 6f61 645f 636f 6e74 6573 7428 290a  .load_contest().
+0000b9a0: 0a20 2020 2064 6566 2065 6469 745f 7374  .    def edit_st
+0000b9b0: 6174 696f 6e5f 7365 7474 696e 6773 2873  ation_settings(s
+0000b9c0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000b9d0: 2253 686f 7720 7365 7474 696e 6773 2064  "Show settings d
+0000b9e0: 6961 6c6f 6722 2222 0a20 2020 2020 2020  ialog""".       
+0000b9f0: 206c 6f67 6765 722e 6465 6275 6728 2253   logger.debug("S
+0000ba00: 7461 7469 6f6e 2053 6574 7469 6e67 7320  tation Settings 
+0000ba10: 7365 6c65 6374 6564 2229 0a20 2020 2020  selected").     
+0000ba20: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+0000ba30: 5f64 6961 6c6f 6720 3d20 4564 6974 5374  _dialog = EditSt
+0000ba40: 6174 696f 6e28 574f 524b 494e 475f 5041  ation(WORKING_PA
+0000ba50: 5448 290a 2020 2020 2020 2020 7365 6c66  TH).        self
+0000ba60: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000ba70: 2e61 6363 6570 7465 642e 636f 6e6e 6563  .accepted.connec
+0000ba80: 7428 7365 6c66 2e73 6176 655f 7365 7474  t(self.save_sett
+0000ba90: 696e 6773 290a 2020 2020 2020 2020 7365  ings).        se
+0000baa0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000bab0: 6f67 2e43 616c 6c2e 7365 7454 6578 7428  og.Call.setText(
+0000bac0: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+0000bad0: 2822 4361 6c6c 222c 2022 2229 290a 2020  ("Call", "")).  
+0000bae0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000baf0: 6e67 735f 6469 616c 6f67 2e4e 616d 652e  ngs_dialog.Name.
+0000bb00: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+0000bb10: 7469 6f6e 2e67 6574 2822 4e61 6d65 222c  tion.get("Name",
+0000bb20: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000bb30: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000bb40: 6f67 2e41 6464 7265 7373 312e 7365 7454  og.Address1.setT
+0000bb50: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+0000bb60: 2e67 6574 2822 5374 7265 6574 3122 2c20  .get("Street1", 
+0000bb70: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
+0000bb80: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000bb90: 672e 4164 6472 6573 7332 2e73 6574 5465  g.Address2.setTe
+0000bba0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000bbb0: 6765 7428 2253 7472 6565 7432 222c 2022  get("Street2", "
+0000bbc0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000bbd0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000bbe0: 2e43 6974 792e 7365 7454 6578 7428 7365  .City.setText(se
+0000bbf0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000bc00: 4369 7479 222c 2022 2229 290a 2020 2020  City", "")).    
+0000bc10: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000bc20: 735f 6469 616c 6f67 2e53 7461 7465 2e73  s_dialog.State.s
+0000bc30: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000bc40: 696f 6e2e 6765 7428 2253 7461 7465 222c  ion.get("State",
+0000bc50: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000bc60: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000bc70: 6f67 2e5a 6970 2e73 6574 5465 7874 2873  og.Zip.setText(s
+0000bc80: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0000bc90: 225a 6970 222c 2022 2229 290a 2020 2020  "Zip", "")).    
+0000bca0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000bcb0: 735f 6469 616c 6f67 2e43 6f75 6e74 7279  s_dialog.Country
+0000bcc0: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
+0000bcd0: 6174 696f 6e2e 6765 7428 2243 6f75 6e74  ation.get("Count
+0000bce0: 7279 222c 2022 2229 290a 2020 2020 2020  ry", "")).      
+0000bcf0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000bd00: 6469 616c 6f67 2e47 7269 6453 7175 6172  dialog.GridSquar
+0000bd10: 652e 7365 7454 6578 7428 7365 6c66 2e73  e.setText(self.s
+0000bd20: 7461 7469 6f6e 2e67 6574 2822 4772 6964  tation.get("Grid
+0000bd30: 5371 7561 7265 222c 2022 2229 290a 2020  Square", "")).  
+0000bd40: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000bd50: 6e67 735f 6469 616c 6f67 2e43 515a 6f6e  ngs_dialog.CQZon
+0000bd60: 652e 7365 7454 6578 7428 7374 7228 7365  e.setText(str(se
+0000bd70: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000bd80: 4351 5a6f 6e65 222c 2022 2229 2929 0a20  CQZone", ""))). 
+0000bd90: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
+0000bda0: 696e 6773 5f64 6961 6c6f 672e 4954 555a  ings_dialog.ITUZ
+0000bdb0: 6f6e 652e 7365 7454 6578 7428 7374 7228  one.setText(str(
+0000bdc0: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+0000bdd0: 2822 4941 5255 5a6f 6e65 222c 2022 2229  ("IARUZone", "")
+0000bde0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000bdf0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000be00: 4c69 6365 6e73 652e 7365 7454 6578 7428  License.setText(
+0000be10: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+0000be20: 2822 4c69 6365 6e73 6543 6c61 7373 222c  ("LicenseClass",
+0000be30: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000be40: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000be50: 6f67 2e4c 6174 6974 7564 652e 7365 7454  og.Latitude.setT
+0000be60: 6578 7428 7374 7228 7365 6c66 2e73 7461  ext(str(self.sta
+0000be70: 7469 6f6e 2e67 6574 2822 4c61 7469 7475  tion.get("Latitu
+0000be80: 6465 222c 2022 2229 2929 0a20 2020 2020  de", ""))).     
+0000be90: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+0000bea0: 5f64 6961 6c6f 672e 4c6f 6e67 6974 7564  _dialog.Longitud
+0000beb0: 652e 7365 7454 6578 7428 7374 7228 7365  e.setText(str(se
+0000bec0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000bed0: 4c6f 6e67 6974 7564 6522 2c20 2222 2929  Longitude", ""))
+0000bee0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000bef0: 6574 7469 6e67 735f 6469 616c 6f67 2e53  ettings_dialog.S
+0000bf00: 7461 7469 6f6e 5458 5258 2e73 6574 5465  tationTXRX.setTe
+0000bf10: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000bf20: 6765 7428 2273 7461 7469 6f6e 7478 7278  get("stationtxrx
+0000bf30: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
+0000bf40: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000bf50: 616c 6f67 2e50 6f77 6572 2e73 6574 5465  alog.Power.setTe
+0000bf60: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000bf70: 6765 7428 2253 506f 7765 222c 2022 2229  get("SPowe", "")
+0000bf80: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000bf90: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
+0000bfa0: 6e74 656e 6e61 2e73 6574 5465 7874 2873  ntenna.setText(s
+0000bfb0: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0000bfc0: 2253 416e 7465 222c 2022 2229 290a 2020  "SAnte", "")).  
+0000bfd0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000bfe0: 6e67 735f 6469 616c 6f67 2e41 6e74 4865  ngs_dialog.AntHe
+0000bff0: 6967 6874 2e73 6574 5465 7874 2873 656c  ight.setText(sel
+0000c000: 662e 7374 6174 696f 6e2e 6765 7428 2253  f.station.get("S
+0000c010: 416e 7448 3122 2c20 2222 2929 0a20 2020  AntH1", "")).   
+0000c020: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
+0000c030: 6773 5f64 6961 6c6f 672e 4153 4c2e 7365  gs_dialog.ASL.se
+0000c040: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
+0000c050: 6f6e 2e67 6574 2822 5341 6e74 4832 222c  on.get("SAntH2",
+0000c060: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000c070: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000c080: 6f67 2e41 5252 4c53 6563 7469 6f6e 2e73  og.ARRLSection.s
+0000c090: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000c0a0: 696f 6e2e 6765 7428 2241 5252 4c53 6563  ion.get("ARRLSec
+0000c0b0: 7469 6f6e 222c 2022 2229 290a 2020 2020  tion", "")).    
+0000c0c0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000c0d0: 735f 6469 616c 6f67 2e52 6f76 6572 5154  s_dialog.RoverQT
+0000c0e0: 482e 7365 7454 6578 7428 7365 6c66 2e73  H.setText(self.s
+0000c0f0: 7461 7469 6f6e 2e67 6574 2822 526f 7665  tation.get("Rove
+0000c100: 7251 5448 222c 2022 2229 290a 2020 2020  rQTH", "")).    
+0000c110: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000c120: 735f 6469 616c 6f67 2e43 6c75 622e 7365  s_dialog.Club.se
+0000c130: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
+0000c140: 6f6e 2e67 6574 2822 436c 7562 222c 2022  on.get("Club", "
+0000c150: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000c160: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000c170: 2e45 6d61 696c 2e73 6574 5465 7874 2873  .Email.setText(s
+0000c180: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0000c190: 2245 6d61 696c 222c 2022 2229 290a 2020  "Email", "")).  
+0000c1a0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000c1b0: 6e67 735f 6469 616c 6f67 2e6f 7065 6e28  ngs_dialog.open(
+0000c1c0: 290a 0a20 2020 2064 6566 2073 6176 655f  )..    def save_
+0000c1d0: 7365 7474 696e 6773 2873 656c 6629 3a0a  settings(self):.
+0000c1e0: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
+0000c1f0: 7365 7474 696e 6773 2222 220a 2020 2020  settings""".    
+0000c200: 2020 2020 6373 203d 2073 656c 662e 7365      cs = self.se
+0000c210: 7474 696e 6773 5f64 6961 6c6f 672e 4361  ttings_dialog.Ca
+0000c220: 6c6c 2e74 6578 7428 290a 2020 2020 2020  ll.text().      
+0000c230: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
+0000c240: 207b 7d0a 2020 2020 2020 2020 7365 6c66   {}.        self
+0000c250: 2e73 7461 7469 6f6e 5b22 4361 6c6c 225d  .station["Call"]
+0000c260: 203d 2063 732e 7570 7065 7228 290a 2020   = cs.upper().  
+0000c270: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000c280: 6f6e 5b22 4e61 6d65 225d 203d 2073 656c  on["Name"] = sel
+0000c290: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000c2a0: 672e 4e61 6d65 2e74 6578 7428 292e 7469  g.Name.text().ti
+0000c2b0: 746c 6528 290a 2020 2020 2020 2020 7365  tle().        se
+0000c2c0: 6c66 2e73 7461 7469 6f6e 5b22 5374 7265  lf.station["Stre
+0000c2d0: 6574 3122 5d20 3d20 7365 6c66 2e73 6574  et1"] = self.set
+0000c2e0: 7469 6e67 735f 6469 616c 6f67 2e41 6464  tings_dialog.Add
+0000c2f0: 7265 7373 312e 7465 7874 2829 2e74 6974  ress1.text().tit
+0000c300: 6c65 2829 0a20 2020 2020 2020 2073 656c  le().        sel
+0000c310: 662e 7374 6174 696f 6e5b 2253 7472 6565  f.station["Stree
+0000c320: 7432 225d 203d 2073 656c 662e 7365 7474  t2"] = self.sett
+0000c330: 696e 6773 5f64 6961 6c6f 672e 4164 6472  ings_dialog.Addr
+0000c340: 6573 7332 2e74 6578 7428 292e 7469 746c  ess2.text().titl
+0000c350: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+0000c360: 2e73 7461 7469 6f6e 5b22 4369 7479 225d  .station["City"]
+0000c370: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+0000c380: 5f64 6961 6c6f 672e 4369 7479 2e74 6578  _dialog.City.tex
+0000c390: 7428 292e 7469 746c 6528 290a 2020 2020  t().title().    
+0000c3a0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000c3b0: 5b22 5374 6174 6522 5d20 3d20 7365 6c66  ["State"] = self
+0000c3c0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000c3d0: 2e53 7461 7465 2e74 6578 7428 292e 7570  .State.text().up
+0000c3e0: 7065 7228 290a 2020 2020 2020 2020 7365  per().        se
+0000c3f0: 6c66 2e73 7461 7469 6f6e 5b22 5a69 7022  lf.station["Zip"
+0000c400: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+0000c410: 735f 6469 616c 6f67 2e5a 6970 2e74 6578  s_dialog.Zip.tex
+0000c420: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000c430: 2e73 7461 7469 6f6e 5b22 436f 756e 7472  .station["Countr
+0000c440: 7922 5d20 3d20 7365 6c66 2e73 6574 7469  y"] = self.setti
+0000c450: 6e67 735f 6469 616c 6f67 2e43 6f75 6e74  ngs_dialog.Count
+0000c460: 7279 2e74 6578 7428 292e 7469 746c 6528  ry.text().title(
+0000c470: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000c480: 7461 7469 6f6e 5b22 4772 6964 5371 7561  tation["GridSqua
+0000c490: 7265 225d 203d 2073 656c 662e 7365 7474  re"] = self.sett
+0000c4a0: 696e 6773 5f64 6961 6c6f 672e 4772 6964  ings_dialog.Grid
+0000c4b0: 5371 7561 7265 2e74 6578 7428 290a 2020  Square.text().  
+0000c4c0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000c4d0: 6f6e 5b22 4351 5a6f 6e65 225d 203d 2073  on["CQZone"] = s
+0000c4e0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000c4f0: 6c6f 672e 4351 5a6f 6e65 2e74 6578 7428  log.CQZone.text(
+0000c500: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000c510: 7461 7469 6f6e 5b22 4941 5255 5a6f 6e65  tation["IARUZone
+0000c520: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+0000c530: 6773 5f64 6961 6c6f 672e 4954 555a 6f6e  gs_dialog.ITUZon
+0000c540: 652e 7465 7874 2829 0a20 2020 2020 2020  e.text().       
+0000c550: 2073 656c 662e 7374 6174 696f 6e5b 224c   self.station["L
+0000c560: 6963 656e 7365 436c 6173 7322 5d20 3d20  icenseClass"] = 
+0000c570: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000c580: 616c 6f67 2e4c 6963 656e 7365 2e74 6578  alog.License.tex
+0000c590: 7428 292e 7469 746c 6528 290a 2020 2020  t().title().    
+0000c5a0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000c5b0: 5b22 4c61 7469 7475 6465 225d 203d 2073  ["Latitude"] = s
+0000c5c0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000c5d0: 6c6f 672e 4c61 7469 7475 6465 2e74 6578  log.Latitude.tex
+0000c5e0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000c5f0: 2e73 7461 7469 6f6e 5b22 4c6f 6e67 6974  .station["Longit
+0000c600: 7564 6522 5d20 3d20 7365 6c66 2e73 6574  ude"] = self.set
+0000c610: 7469 6e67 735f 6469 616c 6f67 2e4c 6f6e  tings_dialog.Lon
+0000c620: 6769 7475 6465 2e74 6578 7428 290a 2020  gitude.text().  
+0000c630: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000c640: 6f6e 5b22 5354 5865 7122 5d20 3d20 7365  on["STXeq"] = se
+0000c650: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000c660: 6f67 2e53 7461 7469 6f6e 5458 5258 2e74  og.StationTXRX.t
+0000c670: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
+0000c680: 6c66 2e73 7461 7469 6f6e 5b22 5350 6f77  lf.station["SPow
+0000c690: 6522 5d20 3d20 7365 6c66 2e73 6574 7469  e"] = self.setti
+0000c6a0: 6e67 735f 6469 616c 6f67 2e50 6f77 6572  ngs_dialog.Power
+0000c6b0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000c6c0: 7365 6c66 2e73 7461 7469 6f6e 5b22 5341  self.station["SA
+0000c6d0: 6e74 6522 5d20 3d20 7365 6c66 2e73 6574  nte"] = self.set
+0000c6e0: 7469 6e67 735f 6469 616c 6f67 2e41 6e74  tings_dialog.Ant
+0000c6f0: 656e 6e61 2e74 6578 7428 290a 2020 2020  enna.text().    
+0000c700: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000c710: 5b22 5341 6e74 4831 225d 203d 2073 656c  ["SAntH1"] = sel
+0000c720: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000c730: 672e 416e 7448 6569 6768 742e 7465 7874  g.AntHeight.text
+0000c740: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000c750: 7374 6174 696f 6e5b 2253 416e 7448 3222  station["SAntH2"
+0000c760: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+0000c770: 735f 6469 616c 6f67 2e41 534c 2e74 6578  s_dialog.ASL.tex
+0000c780: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000c790: 2e73 7461 7469 6f6e 5b22 4152 524c 5365  .station["ARRLSe
+0000c7a0: 6374 696f 6e22 5d20 3d20 7365 6c66 2e73  ction"] = self.s
+0000c7b0: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
+0000c7c0: 5252 4c53 6563 7469 6f6e 2e74 6578 7428  RRLSection.text(
+0000c7d0: 292e 7570 7065 7228 290a 2020 2020 2020  ).upper().      
+0000c7e0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000c7f0: 526f 7665 7251 5448 225d 203d 2073 656c  RoverQTH"] = sel
+0000c800: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000c810: 672e 526f 7665 7251 5448 2e74 6578 7428  g.RoverQTH.text(
+0000c820: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000c830: 7461 7469 6f6e 5b22 436c 7562 225d 203d  tation["Club"] =
+0000c840: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000c850: 6961 6c6f 672e 436c 7562 2e74 6578 7428  ialog.Club.text(
+0000c860: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
+0000c870: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000c880: 456d 6169 6c22 5d20 3d20 7365 6c66 2e73  Email"] = self.s
+0000c890: 6574 7469 6e67 735f 6469 616c 6f67 2e45  ettings_dialog.E
+0000c8a0: 6d61 696c 2e74 6578 7428 290a 2020 2020  mail.text().    
+0000c8b0: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
+0000c8c0: 652e 6164 645f 7374 6174 696f 6e28 7365  e.add_station(se
+0000c8d0: 6c66 2e73 7461 7469 6f6e 290a 2020 2020  lf.station).    
+0000c8e0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000c8f0: 735f 6469 616c 6f67 2e63 6c6f 7365 2829  s_dialog.close()
+0000c900: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000c910: 2e63 7572 7265 6e74 5f6f 7020 3d3d 2022  .current_op == "
+0000c920: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
+0000c930: 656c 662e 6375 7272 656e 745f 6f70 203d  elf.current_op =
+0000c940: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
+0000c950: 7428 2243 616c 6c22 2c20 2222 290a 2020  t("Call", "").  
+0000c960: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0000c970: 616b 655f 6f70 5f64 6972 2829 0a20 2020  ake_op_dir().   
+0000c980: 2020 2020 2063 6f6e 7465 7374 5f63 6f75       contest_cou
+0000c990: 6e74 203d 2073 656c 662e 6461 7461 6261  nt = self.databa
+0000c9a0: 7365 2e66 6574 6368 5f61 6c6c 5f63 6f6e  se.fetch_all_con
+0000c9b0: 7465 7374 7328 290a 2020 2020 2020 2020  tests().        
+0000c9c0: 6966 206c 656e 2863 6f6e 7465 7374 5f63  if len(contest_c
+0000c9d0: 6f75 6e74 2920 3d3d 2030 3a0a 2020 2020  ount) == 0:.    
+0000c9e0: 2020 2020 2020 2020 7365 6c66 2e6e 6577          self.new
+0000c9f0: 5f63 6f6e 7465 7374 5f64 6961 6c6f 6728  _contest_dialog(
+0000ca00: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
+0000ca10: 6d61 6372 6f28 7365 6c66 2c20 6675 6e63  macro(self, func
+0000ca20: 7469 6f6e 5f6b 6579 293a 0a20 2020 2020  tion_key):.     
+0000ca30: 2020 2022 2222 5368 6f77 2065 6469 7420     """Show edit 
+0000ca40: 6d61 6372 6f20 6469 616c 6f67 2222 220a  macro dialog""".
+0000ca50: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+0000ca60: 745f 6d61 6372 6f5f 6469 616c 6f67 203d  t_macro_dialog =
+0000ca70: 2045 6469 744d 6163 726f 2866 756e 6374   EditMacro(funct
+0000ca80: 696f 6e5f 6b65 792c 2057 4f52 4b49 4e47  ion_key, WORKING
+0000ca90: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
+0000caa0: 656c 662e 6564 6974 5f6d 6163 726f 5f64  elf.edit_macro_d
+0000cab0: 6961 6c6f 672e 6163 6365 7074 6564 2e63  ialog.accepted.c
+0000cac0: 6f6e 6e65 6374 2873 656c 662e 6564 6974  onnect(self.edit
+0000cad0: 6564 5f6d 6163 726f 290a 2020 2020 2020  ed_macro).      
+0000cae0: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000caf0: 6f5f 6469 616c 6f67 2e6f 7065 6e28 290a  o_dialog.open().
+0000cb00: 0a20 2020 2064 6566 2065 6469 7465 645f  .    def edited_
+0000cb10: 6d61 6372 6f28 7365 6c66 293a 0a20 2020  macro(self):.   
+0000cb20: 2020 2020 2022 2222 5361 7665 2065 6469       """Save edi
+0000cb30: 7465 6420 6d61 6372 6f22 2222 0a20 2020  ted macro""".   
+0000cb40: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
+0000cb50: 6163 726f 5f64 6961 6c6f 672e 6675 6e63  acro_dialog.func
+0000cb60: 7469 6f6e 5f6b 6579 2e73 6574 5465 7874  tion_key.setText
+0000cb70: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0000cb80: 6c66 2e65 6469 745f 6d61 6372 6f5f 6469  lf.edit_macro_di
+0000cb90: 616c 6f67 2e6d 6163 726f 5f6c 6162 656c  alog.macro_label
+0000cba0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000cbb0: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000cbc0: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
+0000cbd0: 2e66 756e 6374 696f 6e5f 6b65 792e 7365  .function_key.se
+0000cbe0: 7454 6f6f 6c54 6970 280a 2020 2020 2020  tToolTip(.      
+0000cbf0: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+0000cc00: 6d61 6372 6f5f 6469 616c 6f67 2e74 6865  macro_dialog.the
+0000cc10: 5f6d 6163 726f 2e74 6578 7428 290a 2020  _macro.text().  
+0000cc20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000cc30: 7365 6c66 2e65 6469 745f 6d61 6372 6f5f  self.edit_macro_
+0000cc40: 6469 616c 6f67 2e63 6c6f 7365 2829 0a0a  dialog.close()..
+0000cc50: 2020 2020 6465 6620 6564 6974 5f46 3128      def edit_F1(
+0000cc60: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000cc70: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000cc80: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000cc90: 4631 2052 6967 6874 2043 6c69 636b 6564  F1 Right Clicked
+0000cca0: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
+0000ccb0: 2e65 6469 745f 6d61 6372 6f28 7365 6c66  .edit_macro(self
+0000ccc0: 2e46 3129 0a0a 2020 2020 6465 6620 6564  .F1)..    def ed
+0000ccd0: 6974 5f46 3228 7365 6c66 293a 0a20 2020  it_F2(self):.   
+0000cce0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000ccf0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000cd00: 6562 7567 2822 4632 2052 6967 6874 2043  ebug("F2 Right C
+0000cd10: 6c69 636b 6564 2e22 290a 2020 2020 2020  licked.").      
+0000cd20: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000cd30: 6f28 7365 6c66 2e46 3229 0a0a 2020 2020  o(self.F2)..    
+0000cd40: 6465 6620 6564 6974 5f46 3328 7365 6c66  def edit_F3(self
+0000cd50: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000cd60: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000cd70: 6767 6572 2e64 6562 7567 2822 4633 2052  gger.debug("F3 R
+0000cd80: 6967 6874 2043 6c69 636b 6564 2e22 290a  ight Clicked.").
+0000cd90: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+0000cda0: 745f 6d61 6372 6f28 7365 6c66 2e46 3329  t_macro(self.F3)
+0000cdb0: 0a0a 2020 2020 6465 6620 6564 6974 5f46  ..    def edit_F
+0000cdc0: 3428 7365 6c66 293a 0a20 2020 2020 2020  4(self):.       
+0000cdd0: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000cde0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000cdf0: 2822 4634 2052 6967 6874 2043 6c69 636b  ("F4 Right Click
+0000ce00: 6564 2e22 290a 2020 2020 2020 2020 7365  ed.").        se
+0000ce10: 6c66 2e65 6469 745f 6d61 6372 6f28 7365  lf.edit_macro(se
+0000ce20: 6c66 2e46 3429 0a0a 2020 2020 6465 6620  lf.F4)..    def 
+0000ce30: 6564 6974 5f46 3528 7365 6c66 293a 0a20  edit_F5(self):. 
+0000ce40: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000ce50: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000ce60: 2e64 6562 7567 2822 4635 2052 6967 6874  .debug("F5 Right
+0000ce70: 2043 6c69 636b 6564 2e22 290a 2020 2020   Clicked.").    
+0000ce80: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000ce90: 6372 6f28 7365 6c66 2e46 3529 0a0a 2020  cro(self.F5)..  
+0000cea0: 2020 6465 6620 6564 6974 5f46 3628 7365    def edit_F6(se
+0000ceb0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000cec0: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000ced0: 6c6f 6767 6572 2e64 6562 7567 2822 4636  logger.debug("F6
+0000cee0: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
+0000cef0: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000cf00: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
+0000cf10: 3629 0a0a 2020 2020 6465 6620 6564 6974  6)..    def edit
+0000cf20: 5f46 3728 7365 6c66 293a 0a20 2020 2020  _F7(self):.     
+0000cf30: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000cf40: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000cf50: 7567 2822 4637 2052 6967 6874 2043 6c69  ug("F7 Right Cli
+0000cf60: 636b 6564 2e22 290a 2020 2020 2020 2020  cked.").        
+0000cf70: 7365 6c66 2e65 6469 745f 6d61 6372 6f28  self.edit_macro(
+0000cf80: 7365 6c66 2e46 3729 0a0a 2020 2020 6465  self.F7)..    de
+0000cf90: 6620 6564 6974 5f46 3828 7365 6c66 293a  f edit_F8(self):
+0000cfa0: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
+0000cfb0: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+0000cfc0: 6572 2e64 6562 7567 2822 4638 2052 6967  er.debug("F8 Rig
+0000cfd0: 6874 2043 6c69 636b 6564 2e22 290a 2020  ht Clicked.").  
+0000cfe0: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+0000cff0: 6d61 6372 6f28 7365 6c66 2e46 3829 0a0a  macro(self.F8)..
+0000d000: 2020 2020 6465 6620 6564 6974 5f46 3928      def edit_F9(
+0000d010: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000d020: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000d030: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000d040: 4639 2052 6967 6874 2043 6c69 636b 6564  F9 Right Clicked
+0000d050: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
+0000d060: 2e65 6469 745f 6d61 6372 6f28 7365 6c66  .edit_macro(self
+0000d070: 2e46 3929 0a0a 2020 2020 6465 6620 6564  .F9)..    def ed
+0000d080: 6974 5f46 3130 2873 656c 6629 3a0a 2020  it_F10(self):.  
+0000d090: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
+0000d0a0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000d0b0: 6465 6275 6728 2246 3130 2052 6967 6874  debug("F10 Right
+0000d0c0: 2043 6c69 636b 6564 2e22 290a 2020 2020   Clicked.").    
+0000d0d0: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000d0e0: 6372 6f28 7365 6c66 2e46 3130 290a 0a20  cro(self.F10).. 
+0000d0f0: 2020 2064 6566 2065 6469 745f 4631 3128     def edit_F11(
+0000d100: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000d110: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000d120: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000d130: 4631 3120 5269 6768 7420 436c 6963 6b65  F11 Right Clicke
+0000d140: 642e 2229 0a20 2020 2020 2020 2073 656c  d.").        sel
+0000d150: 662e 6564 6974 5f6d 6163 726f 2873 656c  f.edit_macro(sel
+0000d160: 662e 4631 3129 0a0a 2020 2020 6465 6620  f.F11)..    def 
+0000d170: 6564 6974 5f46 3132 2873 656c 6629 3a0a  edit_F12(self):.
+0000d180: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
+0000d190: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
+0000d1a0: 722e 6465 6275 6728 2246 3132 2052 6967  r.debug("F12 Rig
+0000d1b0: 6874 2043 6c69 636b 6564 2e22 290a 2020  ht Clicked.").  
+0000d1c0: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+0000d1d0: 6d61 6372 6f28 7365 6c66 2e46 3132 290a  macro(self.F12).
+0000d1e0: 0a20 2020 2064 6566 2070 726f 6365 7373  .    def process
+0000d1f0: 5f6d 6163 726f 2873 656c 662c 206d 6163  _macro(self, mac
+0000d200: 726f 3a20 7374 7229 202d 3e20 7374 723a  ro: str) -> str:
+0000d210: 0a20 2020 2020 2020 2022 2222 5072 6f63  .        """Proc
+0000d220: 6573 7320 4357 206d 6163 726f 2073 7562  ess CW macro sub
+0000d230: 7374 6974 7574 696f 6e73 2222 220a 2020  stitutions""".  
+0000d240: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+0000d250: 656c 662e 6461 7461 6261 7365 2e67 6574  elf.database.get
+0000d260: 5f73 6572 6961 6c28 290a 2020 2020 2020  _serial().      
+0000d270: 2020 6e65 7874 5f73 6572 6961 6c20 3d20    next_serial = 
+0000d280: 7374 7228 7265 7375 6c74 2e67 6574 2822  str(result.get("
+0000d290: 7365 7269 616c 5f6e 7222 2c20 2231 2229  serial_nr", "1")
+0000d2a0: 290a 2020 2020 2020 2020 6966 206e 6578  ).        if nex
+0000d2b0: 745f 7365 7269 616c 203d 3d20 224e 6f6e  t_serial == "Non
+0000d2c0: 6522 3a0a 2020 2020 2020 2020 2020 2020  e":.            
+0000d2d0: 6e65 7874 5f73 6572 6961 6c20 3d20 2231  next_serial = "1
+0000d2e0: 220a 2020 2020 2020 2020 6d61 6372 6f20  ".        macro 
+0000d2f0: 3d20 6d61 6372 6f2e 7570 7065 7228 290a  = macro.upper().
+0000d300: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
+0000d310: 6d61 6372 6f2e 7265 706c 6163 6528 2223  macro.replace("#
+0000d320: 222c 206e 6578 745f 7365 7269 616c 290a  ", next_serial).
+0000d330: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
+0000d340: 6d61 6372 6f2e 7265 706c 6163 6528 227b  macro.replace("{
+0000d350: 4d59 4341 4c4c 7d22 2c20 7365 6c66 2e73  MYCALL}", self.s
+0000d360: 7461 7469 6f6e 2e67 6574 2822 4361 6c6c  tation.get("Call
+0000d370: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
+0000d380: 6d61 6372 6f20 3d20 6d61 6372 6f2e 7265  macro = macro.re
+0000d390: 706c 6163 6528 227b 4849 5343 414c 4c7d  place("{HISCALL}
+0000d3a0: 222c 2073 656c 662e 6361 6c6c 7369 676e  ", self.callsign
+0000d3b0: 2e74 6578 7428 2929 0a20 2020 2020 2020  .text()).       
+0000d3c0: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+0000d3d0: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+0000d3e0: 203d 3d20 2243 5722 3a0a 2020 2020 2020   == "CW":.      
+0000d3f0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
+0000d400: 6372 6f2e 7265 706c 6163 6528 227b 534e  cro.replace("{SN
+0000d410: 547d 222c 2073 656c 662e 7365 6e74 2e74  T}", self.sent.t
+0000d420: 6578 7428 292e 7265 706c 6163 6528 2239  ext().replace("9
+0000d430: 222c 2022 6e22 2929 0a20 2020 2020 2020  ", "n")).       
+0000d440: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d450: 2020 206d 6163 726f 203d 206d 6163 726f     macro = macro
+0000d460: 2e72 6570 6c61 6365 2822 7b53 4e54 7d22  .replace("{SNT}"
+0000d470: 2c20 7365 6c66 2e73 656e 742e 7465 7874  , self.sent.text
+0000d480: 2829 290a 2020 2020 2020 2020 6d61 6372  ()).        macr
+0000d490: 6f20 3d20 6d61 6372 6f2e 7265 706c 6163  o = macro.replac
+0000d4a0: 6528 227b 5345 4e54 4e52 7d22 2c20 7365  e("{SENTNR}", se
+0000d4b0: 6c66 2e6f 7468 6572 5f31 2e74 6578 7428  lf.other_1.text(
+0000d4c0: 2929 0a20 2020 2020 2020 206d 6163 726f  )).        macro
 0000d4d0: 203d 206d 6163 726f 2e72 6570 6c61 6365   = macro.replace
-0000d4e0: 2822 7b4d 5943 414c 4c7d 222c 2073 656c  ("{MYCALL}", sel
-0000d4f0: 662e 7374 6174 696f 6e2e 6765 7428 2243  f.station.get("C
-0000d500: 616c 6c22 2c20 2222 2929 0a20 2020 2020  all", "")).     
-0000d510: 2020 206d 6163 726f 203d 206d 6163 726f     macro = macro
-0000d520: 2e72 6570 6c61 6365 2822 7b48 4953 4341  .replace("{HISCA
-0000d530: 4c4c 7d22 2c20 7365 6c66 2e63 616c 6c73  LL}", self.calls
-0000d540: 6967 6e2e 7465 7874 2829 290a 2020 2020  ign.text()).    
-0000d550: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
-0000d560: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
-0000d570: 6522 2920 3d3d 2022 4357 223a 0a20 2020  e") == "CW":.   
-0000d580: 2020 2020 2020 2020 206d 6163 726f 203d           macro =
-0000d590: 206d 6163 726f 2e72 6570 6c61 6365 2822   macro.replace("
-0000d5a0: 7b53 4e54 7d22 2c20 7365 6c66 2e73 656e  {SNT}", self.sen
-0000d5b0: 742e 7465 7874 2829 2e72 6570 6c61 6365  t.text().replace
-0000d5c0: 2822 3922 2c20 226e 2229 290a 2020 2020  ("9", "n")).    
-0000d5d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000d5e0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
-0000d5f0: 6372 6f2e 7265 706c 6163 6528 227b 534e  cro.replace("{SN
-0000d600: 547d 222c 2073 656c 662e 7365 6e74 2e74  T}", self.sent.t
-0000d610: 6578 7428 2929 0a20 2020 2020 2020 206d  ext()).        m
-0000d620: 6163 726f 203d 206d 6163 726f 2e72 6570  acro = macro.rep
-0000d630: 6c61 6365 2822 7b53 454e 544e 527d 222c  lace("{SENTNR}",
-0000d640: 2073 656c 662e 6f74 6865 725f 312e 7465   self.other_1.te
-0000d650: 7874 2829 290a 2020 2020 2020 2020 6d61  xt()).        ma
-0000d660: 6372 6f20 3d20 6d61 6372 6f2e 7265 706c  cro = macro.repl
-0000d670: 6163 6528 0a20 2020 2020 2020 2020 2020  ace(.           
-0000d680: 2022 7b45 5843 487d 222c 2073 656c 662e   "{EXCH}", self.
-0000d690: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
-0000d6a0: 2e67 6574 2822 5365 6e74 4578 6368 616e  .get("SentExchan
-0000d6b0: 6765 222c 2022 7878 7822 290a 2020 2020  ge", "xxx").    
-0000d6c0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-0000d6d0: 7475 726e 206d 6163 726f 0a0a 2020 2020  turn macro..    
-0000d6e0: 6465 6620 766f 6963 655f 7374 7269 6e67  def voice_string
-0000d6f0: 2873 656c 662c 2074 6865 5f73 7472 696e  (self, the_strin
-0000d700: 673a 2073 7472 2920 2d3e 204e 6f6e 653a  g: str) -> None:
-0000d710: 0a20 2020 2020 2020 2022 2222 766f 6963  .        """voic
-0000d720: 6573 2073 7472 696e 6720 7573 696e 6720  es string using 
-0000d730: 6e61 746f 2070 686f 6e65 7469 6373 2222  nato phonetics""
-0000d740: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000d750: 2e64 6562 7567 2822 566f 6963 696e 673a  .debug("Voicing:
-0000d760: 2025 7322 2c20 7468 655f 7374 7269 6e67   %s", the_string
-0000d770: 290a 2020 2020 2020 2020 6f70 5f70 6174  ).        op_pat
-0000d780: 6820 3d20 5061 7468 2844 4154 415f 5041  h = Path(DATA_PA
-0000d790: 5448 2920 2f20 7365 6c66 2e63 7572 7265  TH) / self.curre
-0000d7a0: 6e74 5f6f 700a 2020 2020 2020 2020 6966  nt_op.        if
-0000d7b0: 2022 5b22 2069 6e20 7468 655f 7374 7269   "[" in the_stri
-0000d7c0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-0000d7d0: 7375 625f 7374 7269 6e67 203d 2074 6865  sub_string = the
-0000d7e0: 5f73 7472 696e 672e 7374 7269 7028 225b  _string.strip("[
-0000d7f0: 5d22 292e 6c6f 7765 7228 290a 2020 2020  ]").lower().    
-0000d800: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
-0000d810: 203d 2066 227b 7374 7228 6f70 5f70 6174   = f"{str(op_pat
-0000d820: 6829 7d2f 7b73 7562 5f73 7472 696e 677d  h)}/{sub_string}
-0000d830: 2e77 6176 220a 2020 2020 2020 2020 2020  .wav".          
-0000d840: 2020 6966 2050 6174 6828 6669 6c65 6e61    if Path(filena
-0000d850: 6d65 292e 6973 5f66 696c 6528 293a 0a20  me).is_file():. 
-0000d860: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000d870: 6f67 6765 722e 6465 6275 6728 2256 6f69  ogger.debug("Voi
-0000d880: 6369 6e67 3a20 2573 222c 2066 696c 656e  cing: %s", filen
-0000d890: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-0000d8a0: 2020 2020 2064 6174 612c 205f 6673 203d       data, _fs =
-0000d8b0: 2073 662e 7265 6164 2866 696c 656e 616d   sf.read(filenam
-0000d8c0: 652c 2064 7479 7065 3d22 666c 6f61 7433  e, dtype="float3
-0000d8d0: 3222 290a 2020 2020 2020 2020 2020 2020  2").            
-0000d8e0: 2020 2020 7365 6c66 2e70 7474 5f6f 6e28      self.ptt_on(
-0000d8f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000d900: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0000d910: 2020 2020 2020 2020 2020 2073 642e 6465             sd.de
-0000d920: 6661 756c 742e 6465 7669 6365 203d 2073  fault.device = s
-0000d930: 656c 662e 7072 6566 2e67 6574 2822 736f  elf.pref.get("so
-0000d940: 756e 6464 6576 6963 6522 2c20 2264 6566  unddevice", "def
-0000d950: 6175 6c74 2229 0a20 2020 2020 2020 2020  ault").         
-0000d960: 2020 2020 2020 2020 2020 2073 642e 6465             sd.de
-0000d970: 6661 756c 742e 7361 6d70 6c65 7261 7465  fault.samplerate
-0000d980: 203d 2034 3431 3030 2e30 0a20 2020 2020   = 44100.0.     
-0000d990: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d9a0: 642e 706c 6179 2864 6174 6129 0a20 2020  d.play(data).   
-0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9c0: 205f 7374 6174 7573 203d 2073 642e 7761   _status = sd.wa
-0000d9d0: 6974 2829 0a20 2020 2020 2020 2020 2020  it().           
-0000d9e0: 2020 2020 2020 2020 2023 2068 7474 7073           # https
-0000d9f0: 3a2f 2f73 6e79 6b2e 696f 2f61 6476 6973  ://snyk.io/advis
-0000da00: 6f72 2f70 7974 686f 6e2f 736f 756e 6464  or/python/soundd
-0000da10: 6576 6963 652f 6675 6e63 7469 6f6e 732f  evice/functions/
-0000da20: 736f 756e 6464 6576 6963 652e 506f 7274  sounddevice.Port
-0000da30: 4175 6469 6f45 7272 6f72 0a20 2020 2020  AudioError.     
-0000da40: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-0000da50: 7420 7364 2e50 6f72 7441 7564 696f 4572  t sd.PortAudioEr
-0000da60: 726f 7220 6173 2065 7272 3a0a 2020 2020  ror as err:.    
+0000d4e0: 280a 2020 2020 2020 2020 2020 2020 227b  (.            "{
+0000d4f0: 4558 4348 7d22 2c20 7365 6c66 2e63 6f6e  EXCH}", self.con
+0000d500: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
+0000d510: 7428 2253 656e 7445 7863 6861 6e67 6522  t("SentExchange"
+0000d520: 2c20 2278 7878 2229 0a20 2020 2020 2020  , "xxx").       
+0000d530: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+0000d540: 6e20 6d61 6372 6f0a 0a20 2020 2064 6566  n macro..    def
+0000d550: 2076 6f69 6365 5f73 7472 696e 6728 7365   voice_string(se
+0000d560: 6c66 2c20 7468 655f 7374 7269 6e67 3a20  lf, the_string: 
+0000d570: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
+0000d580: 2020 2020 2020 2222 2276 6f69 6365 7320        """voices 
+0000d590: 7374 7269 6e67 2075 7369 6e67 206e 6174  string using nat
+0000d5a0: 6f20 7068 6f6e 6574 6963 7322 2222 0a20  o phonetics""". 
+0000d5b0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000d5c0: 6275 6728 2256 6f69 6369 6e67 3a20 2573  bug("Voicing: %s
+0000d5d0: 222c 2074 6865 5f73 7472 696e 6729 0a20  ", the_string). 
+0000d5e0: 2020 2020 2020 206f 705f 7061 7468 203d         op_path =
+0000d5f0: 2050 6174 6828 4441 5441 5f50 4154 4829   Path(DATA_PATH)
+0000d600: 202f 2073 656c 662e 6375 7272 656e 745f   / self.current_
+0000d610: 6f70 0a20 2020 2020 2020 2069 6620 225b  op.        if "[
+0000d620: 2220 696e 2074 6865 5f73 7472 696e 673a  " in the_string:
+0000d630: 0a20 2020 2020 2020 2020 2020 2073 7562  .            sub
+0000d640: 5f73 7472 696e 6720 3d20 7468 655f 7374  _string = the_st
+0000d650: 7269 6e67 2e73 7472 6970 2822 5b5d 2229  ring.strip("[]")
+0000d660: 2e6c 6f77 6572 2829 0a20 2020 2020 2020  .lower().       
+0000d670: 2020 2020 2066 696c 656e 616d 6520 3d20       filename = 
+0000d680: 6622 7b73 7472 286f 705f 7061 7468 297d  f"{str(op_path)}
+0000d690: 2f7b 7375 625f 7374 7269 6e67 7d2e 7761  /{sub_string}.wa
+0000d6a0: 7622 0a20 2020 2020 2020 2020 2020 2069  v".            i
+0000d6b0: 6620 5061 7468 2866 696c 656e 616d 6529  f Path(filename)
+0000d6c0: 2e69 735f 6669 6c65 2829 3a0a 2020 2020  .is_file():.    
+0000d6d0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0000d6e0: 6572 2e64 6562 7567 2822 566f 6963 696e  er.debug("Voicin
+0000d6f0: 673a 2025 7322 2c20 6669 6c65 6e61 6d65  g: %s", filename
+0000d700: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000d710: 2020 6461 7461 2c20 5f66 7320 3d20 7366    data, _fs = sf
+0000d720: 2e72 6561 6428 6669 6c65 6e61 6d65 2c20  .read(filename, 
+0000d730: 6474 7970 653d 2266 6c6f 6174 3332 2229  dtype="float32")
+0000d740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d750: 2073 656c 662e 7074 745f 6f6e 2829 0a20   self.ptt_on(). 
+0000d760: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000d770: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000d780: 2020 2020 2020 2020 7364 2e64 6566 6175          sd.defau
+0000d790: 6c74 2e64 6576 6963 6520 3d20 7365 6c66  lt.device = self
+0000d7a0: 2e70 7265 662e 6765 7428 2273 6f75 6e64  .pref.get("sound
+0000d7b0: 6465 7669 6365 222c 2022 6465 6661 756c  device", "defaul
+0000d7c0: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
+0000d7d0: 2020 2020 2020 2020 7364 2e64 6566 6175          sd.defau
+0000d7e0: 6c74 2e73 616d 706c 6572 6174 6520 3d20  lt.samplerate = 
+0000d7f0: 3434 3130 302e 300a 2020 2020 2020 2020  44100.0.        
+0000d800: 2020 2020 2020 2020 2020 2020 7364 2e70              sd.p
+0000d810: 6c61 7928 6461 7461 290a 2020 2020 2020  lay(data).      
+0000d820: 2020 2020 2020 2020 2020 2020 2020 5f73                _s
+0000d830: 7461 7475 7320 3d20 7364 2e77 6169 7428  tatus = sd.wait(
+0000d840: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000d850: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
+0000d860: 736e 796b 2e69 6f2f 6164 7669 736f 722f  snyk.io/advisor/
+0000d870: 7079 7468 6f6e 2f73 6f75 6e64 6465 7669  python/sounddevi
+0000d880: 6365 2f66 756e 6374 696f 6e73 2f73 6f75  ce/functions/sou
+0000d890: 6e64 6465 7669 6365 2e50 6f72 7441 7564  nddevice.PortAud
+0000d8a0: 696f 4572 726f 720a 2020 2020 2020 2020  ioError.        
+0000d8b0: 2020 2020 2020 2020 6578 6365 7074 2073          except s
+0000d8c0: 642e 506f 7274 4175 6469 6f45 7272 6f72  d.PortAudioError
+0000d8d0: 2061 7320 6572 723a 0a20 2020 2020 2020   as err:.       
+0000d8e0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+0000d8f0: 6765 722e 7761 726e 696e 6728 2225 7322  ger.warning("%s"
+0000d900: 2c20 6622 7b65 7272 7d22 290a 0a20 2020  , f"{err}")..   
+0000d910: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d920: 662e 7074 745f 6f66 6628 290a 2020 2020  f.ptt_off().    
+0000d930: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000d940: 2020 2020 2020 2073 656c 662e 7074 745f         self.ptt_
+0000d950: 6f6e 2829 0a20 2020 2020 2020 2066 6f72  on().        for
+0000d960: 206c 6574 7465 7220 696e 2074 6865 5f73   letter in the_s
+0000d970: 7472 696e 672e 6c6f 7765 7228 293a 0a20  tring.lower():. 
+0000d980: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+0000d990: 7474 6572 2069 6e20 2261 6263 6465 6667  tter in "abcdefg
+0000d9a0: 6869 6a6b 6c6d 6e6f 7071 7273 7475 7677  hijklmnopqrstuvw
+0000d9b0: 7879 7a20 3132 3334 3536 3738 3930 223a  xyz 1234567890":
+0000d9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d9d0: 2069 6620 6c65 7474 6572 203d 3d20 2220   if letter == " 
+0000d9e0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000d9f0: 2020 2020 2020 206c 6574 7465 7220 3d20         letter = 
+0000da00: 2273 7061 6365 220a 2020 2020 2020 2020  "space".        
+0000da10: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+0000da20: 203d 2066 227b 7374 7228 6f70 5f70 6174   = f"{str(op_pat
+0000da30: 6829 7d2f 7b6c 6574 7465 727d 2e77 6176  h)}/{letter}.wav
+0000da40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000da50: 2020 6966 2050 6174 6828 6669 6c65 6e61    if Path(filena
+0000da60: 6d65 292e 6973 5f66 696c 6528 293a 0a20  me).is_file():. 
 0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da80: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
-0000da90: 2573 222c 2066 227b 6572 727d 2229 0a0a  %s", f"{err}")..
-0000daa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dab0: 7365 6c66 2e70 7474 5f6f 6666 2829 0a20  self.ptt_off(). 
-0000dac0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000dad0: 6e0a 2020 2020 2020 2020 7365 6c66 2e70  n.        self.p
-0000dae0: 7474 5f6f 6e28 290a 2020 2020 2020 2020  tt_on().        
-0000daf0: 666f 7220 6c65 7474 6572 2069 6e20 7468  for letter in th
-0000db00: 655f 7374 7269 6e67 2e6c 6f77 6572 2829  e_string.lower()
-0000db10: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000db20: 206c 6574 7465 7220 696e 2022 6162 6364   letter in "abcd
-0000db30: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
-0000db40: 7576 7778 797a 2031 3233 3435 3637 3839  uvwxyz 123456789
-0000db50: 3022 3a0a 2020 2020 2020 2020 2020 2020  0":.            
-0000db60: 2020 2020 6966 206c 6574 7465 7220 3d3d      if letter ==
-0000db70: 2022 2022 3a0a 2020 2020 2020 2020 2020   " ":.          
-0000db80: 2020 2020 2020 2020 2020 6c65 7474 6572            letter
-0000db90: 203d 2022 7370 6163 6522 0a20 2020 2020   = "space".     
-0000dba0: 2020 2020 2020 2020 2020 2066 696c 656e             filen
-0000dbb0: 616d 6520 3d20 6622 7b73 7472 286f 705f  ame = f"{str(op_
-0000dbc0: 7061 7468 297d 2f7b 6c65 7474 6572 7d2e  path)}/{letter}.
-0000dbd0: 7761 7622 0a20 2020 2020 2020 2020 2020  wav".           
-0000dbe0: 2020 2020 2069 6620 5061 7468 2866 696c       if Path(fil
-0000dbf0: 656e 616d 6529 2e69 735f 6669 6c65 2829  ename).is_file()
-0000dc00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000dc10: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000dc20: 7567 2822 566f 6963 696e 673a 2025 7322  ug("Voicing: %s"
-0000dc30: 2c20 6669 6c65 6e61 6d65 290a 2020 2020  , filename).    
-0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc50: 6461 7461 2c20 5f66 7320 3d20 7366 2e72  data, _fs = sf.r
-0000dc60: 6561 6428 6669 6c65 6e61 6d65 2c20 6474  ead(filename, dt
-0000dc70: 7970 653d 2266 6c6f 6174 3332 2229 0a20  ype="float32"). 
-0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc90: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcb0: 7364 2e64 6566 6175 6c74 2e64 6576 6963  sd.default.devic
-0000dcc0: 6520 3d20 7365 6c66 2e70 7265 662e 6765  e = self.pref.ge
-0000dcd0: 7428 2273 6f75 6e64 6465 7669 6365 222c  t("sounddevice",
-0000dce0: 2022 6465 6661 756c 7422 290a 2020 2020   "default").    
-0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd00: 2020 2020 7364 2e64 6566 6175 6c74 2e73      sd.default.s
-0000dd10: 616d 706c 6572 6174 6520 3d20 3434 3130  amplerate = 4410
-0000dd20: 302e 300a 2020 2020 2020 2020 2020 2020  0.0.            
-0000dd30: 2020 2020 2020 2020 2020 2020 7364 2e70              sd.p
-0000dd40: 6c61 7928 6461 7461 290a 2020 2020 2020  lay(data).      
-0000dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd60: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0000dd70: 2573 222c 2066 227b 7364 2e77 6169 7428  %s", f"{sd.wait(
-0000dd80: 297d 2229 0a20 2020 2020 2020 2020 2020  )}").           
-0000dd90: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-0000dda0: 7364 2e50 6f72 7441 7564 696f 4572 726f  sd.PortAudioErro
-0000ddb0: 7220 6173 2065 7272 3a0a 2020 2020 2020  r as err:.      
-0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddd0: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
-0000dde0: 2822 2573 222c 2066 227b 6572 727d 2229  ("%s", f"{err}")
-0000ddf0: 0a20 2020 2020 2020 2073 656c 662e 7074  .        self.pt
-0000de00: 745f 6f66 6628 290a 0a20 2020 2064 6566  t_off()..    def
-0000de10: 2070 7474 5f6f 6e28 7365 6c66 293a 0a20   ptt_on(self):. 
-0000de20: 2020 2020 2020 2022 2222 7475 726e 206f         """turn o
-0000de30: 6e20 7074 7422 2222 0a20 2020 2020 2020  n ptt""".       
-0000de40: 2069 6620 7365 6c66 2e72 6967 5f63 6f6e   if self.rig_con
-0000de50: 7472 6f6c 3a0a 2020 2020 2020 2020 2020  trol:.          
-0000de60: 2020 7365 6c66 2e6c 6566 7464 6f74 2e73    self.leftdot.s
-0000de70: 6574 5069 786d 6170 2873 656c 662e 6772  etPixmap(self.gr
-0000de80: 6565 6e64 6f74 290a 2020 2020 2020 2020  eendot).        
-0000de90: 2020 2020 6170 702e 7072 6f63 6573 7345      app.processE
-0000dea0: 7665 6e74 7328 290a 2020 2020 2020 2020  vents().        
-0000deb0: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
-0000dec0: 7472 6f6c 2e70 7474 5f6f 6e28 290a 0a20  trol.ptt_on().. 
-0000ded0: 2020 2064 6566 2070 7474 5f6f 6666 2873     def ptt_off(s
-0000dee0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000def0: 2274 7572 6e20 6f66 6620 7074 7422 2222  "turn off ptt"""
-0000df00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000df10: 2e72 6967 5f63 6f6e 7472 6f6c 3a0a 2020  .rig_control:.  
-0000df20: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-0000df30: 6566 7464 6f74 2e73 6574 5069 786d 6170  eftdot.setPixmap
-0000df40: 2873 656c 662e 7265 6464 6f74 290a 2020  (self.reddot).  
-0000df50: 2020 2020 2020 2020 2020 6170 702e 7072            app.pr
-0000df60: 6f63 6573 7345 7665 6e74 7328 290a 2020  ocessEvents().  
-0000df70: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000df80: 6967 5f63 6f6e 7472 6f6c 2e70 7474 5f6f  ig_control.ptt_o
-0000df90: 6666 2829 0a0a 2020 2020 6465 6620 7365  ff()..    def se
-0000dfa0: 6e64 6631 2873 656c 6629 3a0a 2020 2020  ndf1(self):.    
-0000dfb0: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000dfc0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000dfd0: 6275 6728 2246 3120 436c 6963 6b65 6422  bug("F1 Clicked"
-0000dfe0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000dff0: 662e 6e31 6d6d 3a0a 2020 2020 2020 2020  f.n1mm:.        
-0000e000: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
-0000e010: 6469 6f5f 696e 666f 5b22 4675 6e63 7469  dio_info["Functi
-0000e020: 6f6e 4b65 7943 6170 7469 6f6e 225d 203d  onKeyCaption"] =
-0000e030: 2073 656c 662e 4631 2e74 6f6f 6c54 6970   self.F1.toolTip
-0000e040: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0000e050: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000e060: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
-0000e070: 4c53 4222 2c20 2255 5342 222c 2022 5353  LSB", "USB", "SS
-0000e080: 4222 5d3a 0a20 2020 2020 2020 2020 2020  B"]:.           
-0000e090: 2073 656c 662e 766f 6963 655f 7374 7269   self.voice_stri
-0000e0a0: 6e67 2873 656c 662e 7072 6f63 6573 735f  ng(self.process_
-0000e0b0: 6d61 6372 6f28 7365 6c66 2e46 312e 746f  macro(self.F1.to
-0000e0c0: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
-0000e0d0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000e0e0: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
-0000e0f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000e100: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
-0000e110: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000e120: 656c 662e 4631 2e74 6f6f 6c54 6970 2829  elf.F1.toolTip()
-0000e130: 2929 0a0a 2020 2020 6465 6620 7365 6e64  ))..    def send
-0000e140: 6632 2873 656c 6629 3a0a 2020 2020 2020  f2(self):.      
-0000e150: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000e160: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000e170: 6728 2246 3220 436c 6963 6b65 6422 290a  g("F2 Clicked").
-0000e180: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000e190: 6e31 6d6d 3a0a 2020 2020 2020 2020 2020  n1mm:.          
-0000e1a0: 2020 7365 6c66 2e6e 316d 6d2e 7261 6469    self.n1mm.radi
-0000e1b0: 6f5f 696e 666f 5b22 4675 6e63 7469 6f6e  o_info["Function
-0000e1c0: 4b65 7943 6170 7469 6f6e 225d 203d 2073  KeyCaption"] = s
-0000e1d0: 656c 662e 4632 2e74 6f6f 6c54 6970 2829  elf.F2.toolTip()
-0000e1e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000e1f0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-0000e200: 2822 6d6f 6465 2229 2069 6e20 5b22 4c53  ("mode") in ["LS
-0000e210: 4222 2c20 2255 5342 222c 2022 5353 4222  B", "USB", "SSB"
-0000e220: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
-0000e230: 656c 662e 766f 6963 655f 7374 7269 6e67  elf.voice_string
-0000e240: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
-0000e250: 6372 6f28 7365 6c66 2e46 322e 746f 6f6c  cro(self.F2.tool
-0000e260: 5469 7028 2929 290a 2020 2020 2020 2020  Tip())).        
-0000e270: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000e280: 2020 2069 6620 7365 6c66 2e63 773a 0a20     if self.cw:. 
-0000e290: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e2a0: 6377 2e73 656e 6463 7728 7365 6c66 2e70  cw.sendcw(self.p
-0000e2b0: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
-0000e2c0: 662e 4632 2e74 6f6f 6c54 6970 2829 2929  f.F2.toolTip()))
-0000e2d0: 0a0a 2020 2020 6465 6620 7365 6e64 6633  ..    def sendf3
-0000e2e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000e2f0: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000e300: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000e310: 2246 3320 436c 6963 6b65 6422 290a 2020  "F3 Clicked").  
-0000e320: 2020 2020 2020 6966 2073 656c 662e 6e31        if self.n1
-0000e330: 6d6d 3a0a 2020 2020 2020 2020 2020 2020  mm:.            
-0000e340: 7365 6c66 2e6e 316d 6d2e 7261 6469 6f5f  self.n1mm.radio_
-0000e350: 696e 666f 5b22 4675 6e63 7469 6f6e 4b65  info["FunctionKe
-0000e360: 7943 6170 7469 6f6e 225d 203d 2073 656c  yCaption"] = sel
-0000e370: 662e 4633 2e74 6f6f 6c54 6970 2829 0a20  f.F3.toolTip(). 
-0000e380: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000e390: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-0000e3a0: 6d6f 6465 2229 2069 6e20 5b22 4c53 4222  mode") in ["LSB"
-0000e3b0: 2c20 2255 5342 222c 2022 5353 4222 5d3a  , "USB", "SSB"]:
-0000e3c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000e3d0: 662e 766f 6963 655f 7374 7269 6e67 2873  f.voice_string(s
-0000e3e0: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
-0000e3f0: 6f28 7365 6c66 2e46 332e 746f 6f6c 5469  o(self.F3.toolTi
-0000e400: 7028 2929 290a 2020 2020 2020 2020 2020  p())).          
-0000e410: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000e420: 2069 6620 7365 6c66 2e63 773a 0a20 2020   if self.cw:.   
-0000e430: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
-0000e440: 2e73 656e 6463 7728 7365 6c66 2e70 726f  .sendcw(self.pro
-0000e450: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
-0000e460: 4633 2e74 6f6f 6c54 6970 2829 2929 0a0a  F3.toolTip()))..
-0000e470: 2020 2020 6465 6620 7365 6e64 6634 2873      def sendf4(s
-0000e480: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000e490: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000e4a0: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000e4b0: 3420 436c 6963 6b65 6422 290a 2020 2020  4 Clicked").    
-0000e4c0: 2020 2020 6966 2073 656c 662e 6e31 6d6d      if self.n1mm
-0000e4d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000e4e0: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
-0000e4f0: 666f 5b22 4675 6e63 7469 6f6e 4b65 7943  fo["FunctionKeyC
-0000e500: 6170 7469 6f6e 225d 203d 2073 656c 662e  aption"] = self.
-0000e510: 4634 2e74 6f6f 6c54 6970 2829 0a20 2020  F4.toolTip().   
-0000e520: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
-0000e530: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
-0000e540: 6465 2229 2069 6e20 5b22 4c53 4222 2c20  de") in ["LSB", 
-0000e550: 2255 5342 222c 2022 5353 4222 5d3a 0a20  "USB", "SSB"]:. 
-0000e560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e570: 766f 6963 655f 7374 7269 6e67 2873 656c  voice_string(sel
-0000e580: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
-0000e590: 7365 6c66 2e46 342e 746f 6f6c 5469 7028  self.F4.toolTip(
-0000e5a0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-0000e5b0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0000e5c0: 6620 7365 6c66 2e63 773a 0a20 2020 2020  f self.cw:.     
-0000e5d0: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-0000e5e0: 656e 6463 7728 7365 6c66 2e70 726f 6365  endcw(self.proce
-0000e5f0: 7373 5f6d 6163 726f 2873 656c 662e 4634  ss_macro(self.F4
-0000e600: 2e74 6f6f 6c54 6970 2829 2929 0a0a 2020  .toolTip()))..  
-0000e610: 2020 6465 6620 7365 6e64 6635 2873 656c    def sendf5(sel
-0000e620: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000e630: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000e640: 6f67 6765 722e 6465 6275 6728 2246 3520  ogger.debug("F5 
-0000e650: 436c 6963 6b65 6422 290a 2020 2020 2020  Clicked").      
-0000e660: 2020 6966 2073 656c 662e 6e31 6d6d 3a0a    if self.n1mm:.
-0000e670: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e680: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
-0000e690: 5b22 4675 6e63 7469 6f6e 4b65 7943 6170  ["FunctionKeyCap
-0000e6a0: 7469 6f6e 225d 203d 2073 656c 662e 4635  tion"] = self.F5
-0000e6b0: 2e74 6f6f 6c54 6970 2829 0a20 2020 2020  .toolTip().     
-0000e6c0: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
-0000e6d0: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
-0000e6e0: 2229 2069 6e20 5b22 4c53 4222 2c20 2255  ") in ["LSB", "U
-0000e6f0: 5342 222c 2022 5353 4222 5d3a 0a20 2020  SB", "SSB"]:.   
-0000e700: 2020 2020 2020 2020 2073 656c 662e 766f           self.vo
-0000e710: 6963 655f 7374 7269 6e67 2873 656c 662e  ice_string(self.
-0000e720: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
-0000e730: 6c66 2e46 352e 746f 6f6c 5469 7028 2929  lf.F5.toolTip())
-0000e740: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0000e750: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
-0000e760: 7365 6c66 2e63 773a 0a20 2020 2020 2020  self.cw:.       
-0000e770: 2020 2020 2073 656c 662e 6377 2e73 656e       self.cw.sen
-0000e780: 6463 7728 7365 6c66 2e70 726f 6365 7373  dcw(self.process
-0000e790: 5f6d 6163 726f 2873 656c 662e 4635 2e74  _macro(self.F5.t
-0000e7a0: 6f6f 6c54 6970 2829 2929 0a0a 2020 2020  oolTip()))..    
-0000e7b0: 6465 6620 7365 6e64 6636 2873 656c 6629  def sendf6(self)
-0000e7c0: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000e7d0: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000e7e0: 6765 722e 6465 6275 6728 2246 3620 436c  ger.debug("F6 Cl
-0000e7f0: 6963 6b65 6422 290a 2020 2020 2020 2020  icked").        
-0000e800: 6966 2073 656c 662e 6e31 6d6d 3a0a 2020  if self.n1mm:.  
-0000e810: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0000e820: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
-0000e830: 4675 6e63 7469 6f6e 4b65 7943 6170 7469  FunctionKeyCapti
-0000e840: 6f6e 225d 203d 2073 656c 662e 4636 2e74  on"] = self.F6.t
-0000e850: 6f6f 6c54 6970 2829 0a20 2020 2020 2020  oolTip().       
-0000e860: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0000e870: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-0000e880: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
-0000e890: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
-0000e8a0: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
-0000e8b0: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
-0000e8c0: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000e8d0: 2e46 362e 746f 6f6c 5469 7028 2929 290a  .F6.toolTip())).
-0000e8e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000e8f0: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
-0000e900: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
-0000e910: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
-0000e920: 7728 7365 6c66 2e70 726f 6365 7373 5f6d  w(self.process_m
-0000e930: 6163 726f 2873 656c 662e 4636 2e74 6f6f  acro(self.F6.too
-0000e940: 6c54 6970 2829 2929 0a0a 2020 2020 6465  lTip()))..    de
-0000e950: 6620 7365 6e64 6637 2873 656c 6629 3a0a  f sendf7(self):.
-0000e960: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000e970: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000e980: 722e 6465 6275 6728 2246 3720 436c 6963  r.debug("F7 Clic
-0000e990: 6b65 6422 290a 2020 2020 2020 2020 6966  ked").        if
-0000e9a0: 2073 656c 662e 6e31 6d6d 3a0a 2020 2020   self.n1mm:.    
-0000e9b0: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-0000e9c0: 6d2e 7261 6469 6f5f 696e 666f 5b22 4675  m.radio_info["Fu
-0000e9d0: 6e63 7469 6f6e 4b65 7943 6170 7469 6f6e  nctionKeyCaption
-0000e9e0: 225d 203d 2073 656c 662e 4637 2e74 6f6f  "] = self.F7.too
-0000e9f0: 6c54 6970 2829 0a20 2020 2020 2020 2069  lTip().        i
-0000ea00: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
-0000ea10: 7465 2e67 6574 2822 6d6f 6465 2229 2069  te.get("mode") i
-0000ea20: 6e20 5b22 4c53 4222 2c20 2255 5342 222c  n ["LSB", "USB",
-0000ea30: 2022 5353 4222 5d3a 0a20 2020 2020 2020   "SSB"]:.       
-0000ea40: 2020 2020 2073 656c 662e 766f 6963 655f       self.voice_
-0000ea50: 7374 7269 6e67 2873 656c 662e 7072 6f63  string(self.proc
-0000ea60: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
-0000ea70: 372e 746f 6f6c 5469 7028 2929 290a 2020  7.toolTip())).  
-0000ea80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000ea90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000eaa0: 2e63 773a 0a20 2020 2020 2020 2020 2020  .cw:.           
-0000eab0: 2073 656c 662e 6377 2e73 656e 6463 7728   self.cw.sendcw(
-0000eac0: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
-0000ead0: 726f 2873 656c 662e 4637 2e74 6f6f 6c54  ro(self.F7.toolT
-0000eae0: 6970 2829 2929 0a0a 2020 2020 6465 6620  ip()))..    def 
-0000eaf0: 7365 6e64 6638 2873 656c 6629 3a0a 2020  sendf8(self):.  
-0000eb00: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000eb10: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000eb20: 6465 6275 6728 2246 3820 436c 6963 6b65  debug("F8 Clicke
-0000eb30: 6422 290a 2020 2020 2020 2020 6966 2073  d").        if s
-0000eb40: 656c 662e 6e31 6d6d 3a0a 2020 2020 2020  elf.n1mm:.      
-0000eb50: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000eb60: 7261 6469 6f5f 696e 666f 5b22 4675 6e63  radio_info["Func
-0000eb70: 7469 6f6e 4b65 7943 6170 7469 6f6e 225d  tionKeyCaption"]
-0000eb80: 203d 2073 656c 662e 4638 2e74 6f6f 6c54   = self.F8.toolT
-0000eb90: 6970 2829 0a20 2020 2020 2020 2069 6620  ip().        if 
-0000eba0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0000ebb0: 2e67 6574 2822 6d6f 6465 2229 2069 6e20  .get("mode") in 
-0000ebc0: 5b22 4c53 4222 2c20 2255 5342 222c 2022  ["LSB", "USB", "
-0000ebd0: 5353 4222 5d3a 0a20 2020 2020 2020 2020  SSB"]:.         
-0000ebe0: 2020 2073 656c 662e 766f 6963 655f 7374     self.voice_st
-0000ebf0: 7269 6e67 2873 656c 662e 7072 6f63 6573  ring(self.proces
-0000ec00: 735f 6d61 6372 6f28 7365 6c66 2e46 382e  s_macro(self.F8.
-0000ec10: 746f 6f6c 5469 7028 2929 290a 2020 2020  toolTip())).    
-0000ec20: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000ec30: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0000ec40: 773a 0a20 2020 2020 2020 2020 2020 2073  w:.            s
-0000ec50: 656c 662e 6377 2e73 656e 6463 7728 7365  elf.cw.sendcw(se
-0000ec60: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
-0000ec70: 2873 656c 662e 4638 2e74 6f6f 6c54 6970  (self.F8.toolTip
-0000ec80: 2829 2929 0a0a 2020 2020 6465 6620 7365  ()))..    def se
-0000ec90: 6e64 6639 2873 656c 6629 3a0a 2020 2020  ndf9(self):.    
-0000eca0: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000ecb0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000ecc0: 6275 6728 2246 3920 436c 6963 6b65 6422  bug("F9 Clicked"
-0000ecd0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000ece0: 662e 6e31 6d6d 3a0a 2020 2020 2020 2020  f.n1mm:.        
-0000ecf0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
-0000ed00: 6469 6f5f 696e 666f 5b22 4675 6e63 7469  dio_info["Functi
-0000ed10: 6f6e 4b65 7943 6170 7469 6f6e 225d 203d  onKeyCaption"] =
-0000ed20: 2073 656c 662e 4639 2e74 6f6f 6c54 6970   self.F9.toolTip
-0000ed30: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0000ed40: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000ed50: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
-0000ed60: 4c53 4222 2c20 2255 5342 222c 2022 5353  LSB", "USB", "SS
-0000ed70: 4222 5d3a 0a20 2020 2020 2020 2020 2020  B"]:.           
-0000ed80: 2073 656c 662e 766f 6963 655f 7374 7269   self.voice_stri
-0000ed90: 6e67 2873 656c 662e 7072 6f63 6573 735f  ng(self.process_
-0000eda0: 6d61 6372 6f28 7365 6c66 2e46 392e 746f  macro(self.F9.to
-0000edb0: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
-0000edc0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000edd0: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
-0000ede0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000edf0: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
-0000ee00: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000ee10: 656c 662e 4639 2e74 6f6f 6c54 6970 2829  elf.F9.toolTip()
-0000ee20: 2929 0a0a 2020 2020 6465 6620 7365 6e64  ))..    def send
-0000ee30: 6631 3028 7365 6c66 293a 0a20 2020 2020  f10(self):.     
-0000ee40: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
-0000ee50: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000ee60: 7567 2822 4631 3020 436c 6963 6b65 6422  ug("F10 Clicked"
-0000ee70: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000ee80: 662e 6e31 6d6d 3a0a 2020 2020 2020 2020  f.n1mm:.        
-0000ee90: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
-0000eea0: 6469 6f5f 696e 666f 5b22 4675 6e63 7469  dio_info["Functi
-0000eeb0: 6f6e 4b65 7943 6170 7469 6f6e 225d 203d  onKeyCaption"] =
-0000eec0: 2073 656c 662e 4631 302e 746f 6f6c 5469   self.F10.toolTi
-0000eed0: 7028 290a 2020 2020 2020 2020 6966 2073  p().        if s
-0000eee0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-0000eef0: 6765 7428 226d 6f64 6522 2920 696e 205b  get("mode") in [
-0000ef00: 224c 5342 222c 2022 5553 4222 2c20 2253  "LSB", "USB", "S
-0000ef10: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
-0000ef20: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
-0000ef30: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
-0000ef40: 5f6d 6163 726f 2873 656c 662e 4631 302e  _macro(self.F10.
-0000ef50: 746f 6f6c 5469 7028 2929 290a 2020 2020  toolTip())).    
-0000ef60: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000ef70: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0000ef80: 773a 0a20 2020 2020 2020 2020 2020 2073  w:.            s
-0000ef90: 656c 662e 6377 2e73 656e 6463 7728 7365  elf.cw.sendcw(se
-0000efa0: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
-0000efb0: 2873 656c 662e 4631 302e 746f 6f6c 5469  (self.F10.toolTi
-0000efc0: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
-0000efd0: 656e 6466 3131 2873 656c 6629 3a0a 2020  endf11(self):.  
-0000efe0: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000eff0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000f000: 6465 6275 6728 2246 3131 2043 6c69 636b  debug("F11 Click
-0000f010: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
-0000f020: 7365 6c66 2e6e 316d 6d3a 0a20 2020 2020  self.n1mm:.     
-0000f030: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-0000f040: 2e72 6164 696f 5f69 6e66 6f5b 2246 756e  .radio_info["Fun
-0000f050: 6374 696f 6e4b 6579 4361 7074 696f 6e22  ctionKeyCaption"
-0000f060: 5d20 3d20 7365 6c66 2e46 3131 2e74 6f6f  ] = self.F11.too
-0000f070: 6c54 6970 2829 0a20 2020 2020 2020 2069  lTip().        i
-0000f080: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
-0000f090: 7465 2e67 6574 2822 6d6f 6465 2229 2069  te.get("mode") i
-0000f0a0: 6e20 5b22 4c53 4222 2c20 2255 5342 222c  n ["LSB", "USB",
-0000f0b0: 2022 5353 4222 5d3a 0a20 2020 2020 2020   "SSB"]:.       
-0000f0c0: 2020 2020 2073 656c 662e 766f 6963 655f       self.voice_
-0000f0d0: 7374 7269 6e67 2873 656c 662e 7072 6f63  string(self.proc
-0000f0e0: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
-0000f0f0: 3131 2e74 6f6f 6c54 6970 2829 2929 0a20  11.toolTip())). 
-0000f100: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000f110: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-0000f120: 662e 6377 3a0a 2020 2020 2020 2020 2020  f.cw:.          
-0000f130: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
-0000f140: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
-0000f150: 6372 6f28 7365 6c66 2e46 3131 2e74 6f6f  cro(self.F11.too
-0000f160: 6c54 6970 2829 2929 0a0a 2020 2020 6465  lTip()))..    de
-0000f170: 6620 7365 6e64 6631 3228 7365 6c66 293a  f sendf12(self):
-0000f180: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
-0000f190: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
-0000f1a0: 6572 2e64 6562 7567 2822 4631 3220 436c  er.debug("F12 Cl
-0000f1b0: 6963 6b65 6422 290a 2020 2020 2020 2020  icked").        
-0000f1c0: 6966 2073 656c 662e 6e31 6d6d 3a0a 2020  if self.n1mm:.  
-0000f1d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0000f1e0: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
-0000f1f0: 4675 6e63 7469 6f6e 4b65 7943 6170 7469  FunctionKeyCapti
-0000f200: 6f6e 225d 203d 2073 656c 662e 4631 322e  on"] = self.F12.
-0000f210: 746f 6f6c 5469 7028 290a 2020 2020 2020  toolTip().      
-0000f220: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
-0000f230: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
-0000f240: 2920 696e 205b 224c 5342 222c 2022 5553  ) in ["LSB", "US
-0000f250: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
-0000f260: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
-0000f270: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
-0000f280: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
-0000f290: 662e 4631 322e 746f 6f6c 5469 7028 2929  f.F12.toolTip())
-0000f2a0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0000f2b0: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
-0000f2c0: 7365 6c66 2e63 773a 0a20 2020 2020 2020  self.cw:.       
-0000f2d0: 2020 2020 2073 656c 662e 6377 2e73 656e       self.cw.sen
-0000f2e0: 6463 7728 7365 6c66 2e70 726f 6365 7373  dcw(self.process
-0000f2f0: 5f6d 6163 726f 2873 656c 662e 4631 322e  _macro(self.F12.
-0000f300: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
-0000f310: 2064 6566 2072 756e 5f73 705f 6275 7474   def run_sp_butt
-0000f320: 6f6e 735f 636c 6963 6b65 6428 7365 6c66  ons_clicked(self
-0000f330: 293a 0a20 2020 2020 2020 2022 2222 4861  ):.        """Ha
-0000f340: 6e64 6c65 2072 756e 2f73 2670 206d 6f64  ndle run/s&p mod
-0000f350: 6522 2222 0a20 2020 2020 2020 2073 656c  e""".        sel
-0000f360: 662e 7072 6566 5b22 7275 6e5f 7374 6174  f.pref["run_stat
-0000f370: 6522 5d20 3d20 7365 6c66 2e72 6164 696f  e"] = self.radio
-0000f380: 4275 7474 6f6e 5f72 756e 2e69 7343 6865  Button_run.isChe
-0000f390: 636b 6564 2829 0a20 2020 2020 2020 2073  cked().        s
-0000f3a0: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
-0000f3b0: 656e 6365 2829 0a20 2020 2020 2020 2073  ence().        s
-0000f3c0: 656c 662e 7265 6164 5f63 775f 6d61 6372  elf.read_cw_macr
-0000f3d0: 6f73 2829 0a0a 2020 2020 6465 6620 7772  os()..    def wr
-0000f3e0: 6974 655f 7072 6566 6572 656e 6365 2873  ite_preference(s
-0000f3f0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000f400: 220a 2020 2020 2020 2020 5772 6974 6520  ".        Write 
-0000f410: 7072 6566 6572 656e 6365 7320 746f 206a  preferences to j
-0000f420: 736f 6e20 6669 6c65 2e0a 2020 2020 2020  son file..      
-0000f430: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
-0000f440: 793a 0a20 2020 2020 2020 2020 2020 2077  y:.            w
-0000f450: 6974 6820 6f70 656e 280a 2020 2020 2020  ith open(.      
-0000f460: 2020 2020 2020 2020 2020 434f 4e46 4947            CONFIG
-0000f470: 5f50 4154 4820 2b20 222f 6e6f 7431 6d6d  _PATH + "/not1mm
-0000f480: 2e6a 736f 6e22 2c20 2277 7422 2c20 656e  .json", "wt", en
-0000f490: 636f 6469 6e67 3d22 7574 662d 3822 0a20  coding="utf-8". 
-0000f4a0: 2020 2020 2020 2020 2020 2029 2061 7320             ) as 
-0000f4b0: 6669 6c65 5f64 6573 6372 6970 746f 723a  file_descriptor:
-0000f4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f4d0: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
-0000f4e0: 2e77 7269 7465 2864 756d 7073 2873 656c  .write(dumps(sel
-0000f4f0: 662e 7072 6566 2c20 696e 6465 6e74 3d34  f.pref, indent=4
-0000f500: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0000f510: 2020 206c 6f67 6765 722e 696e 666f 2822     logger.info("
-0000f520: 7772 6974 696e 673a 2025 7322 2c20 7365  writing: %s", se
-0000f530: 6c66 2e70 7265 6629 0a20 2020 2020 2020  lf.pref).       
-0000f540: 2065 7863 6570 7420 494f 4572 726f 7220   except IOError 
-0000f550: 6173 2065 7863 6570 7469 6f6e 3a0a 2020  as exception:.  
-0000f560: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000f570: 2e63 7269 7469 6361 6c28 2277 7269 7465  .critical("write
-0000f580: 7072 6566 6572 656e 6365 733a 2025 7322  preferences: %s"
-0000f590: 2c20 6578 6365 7074 696f 6e29 0a0a 2020  , exception)..  
-0000f5a0: 2020 6465 6620 7265 6164 7072 6566 6572    def readprefer
-0000f5b0: 656e 6365 7328 7365 6c66 293a 0a20 2020  ences(self):.   
-0000f5c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000f5d0: 2052 6573 746f 7265 2070 7265 6665 7265   Restore prefere
-0000f5e0: 6e63 6573 2069 6620 7468 6579 2065 7869  nces if they exi
-0000f5f0: 7374 2c20 6f74 6865 7277 6973 6520 6372  st, otherwise cr
-0000f600: 6561 7465 2073 6f6d 6520 7361 6e65 2064  eate some sane d
-0000f610: 6566 6175 6c74 732e 0a20 2020 2020 2020  efaults..       
-0000f620: 2022 2222 0a20 2020 2020 2020 2074 7279   """.        try
-0000f630: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000f640: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
-0000f650: 434f 4e46 4947 5f50 4154 4820 2b20 222f  CONFIG_PATH + "/
-0000f660: 6e6f 7431 6d6d 2e6a 736f 6e22 293a 0a20  not1mm.json"):. 
-0000f670: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000f680: 6974 6820 6f70 656e 280a 2020 2020 2020  ith open(.      
-0000f690: 2020 2020 2020 2020 2020 2020 2020 434f                CO
-0000f6a0: 4e46 4947 5f50 4154 4820 2b20 222f 6e6f  NFIG_PATH + "/no
-0000f6b0: 7431 6d6d 2e6a 736f 6e22 2c20 2272 7422  t1mm.json", "rt"
-0000f6c0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-0000f6d0: 3822 0a20 2020 2020 2020 2020 2020 2020  8".             
-0000f6e0: 2020 2029 2061 7320 6669 6c65 5f64 6573     ) as file_des
-0000f6f0: 6372 6970 746f 723a 0a20 2020 2020 2020  criptor:.       
-0000f700: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f710: 662e 7072 6566 203d 206c 6f61 6473 2866  f.pref = loads(f
-0000f720: 696c 655f 6465 7363 7269 7074 6f72 2e72  ile_descriptor.r
-0000f730: 6561 6428 2929 0a20 2020 2020 2020 2020  ead()).         
-0000f740: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000f750: 722e 696e 666f 2822 2573 222c 2073 656c  r.info("%s", sel
-0000f760: 662e 7072 6566 290a 2020 2020 2020 2020  f.pref).        
-0000f770: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000f780: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000f790: 2e69 6e66 6f28 224e 6f20 7072 6566 6572  .info("No prefer
-0000f7a0: 656e 6365 2066 696c 652e 2057 7269 7469  ence file. Writi
-0000f7b0: 6e67 2070 7265 6665 7265 6e63 652e 2229  ng preference.")
-0000f7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f7d0: 2077 6974 6820 6f70 656e 280a 2020 2020   with open(.    
-0000f7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7f0: 434f 4e46 4947 5f50 4154 4820 2b20 222f  CONFIG_PATH + "/
-0000f800: 6e6f 7431 6d6d 2e6a 736f 6e22 2c20 2277  not1mm.json", "w
-0000f810: 7422 2c20 656e 636f 6469 6e67 3d22 7574  t", encoding="ut
-0000f820: 662d 3822 0a20 2020 2020 2020 2020 2020  f-8".           
-0000f830: 2020 2020 2029 2061 7320 6669 6c65 5f64       ) as file_d
-0000f840: 6573 6372 6970 746f 723a 0a20 2020 2020  escriptor:.     
-0000f850: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f860: 656c 662e 7072 6566 203d 2073 656c 662e  elf.pref = self.
-0000f870: 7072 6566 5f72 6566 2e63 6f70 7928 290a  pref_ref.copy().
-0000f880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f890: 2020 2020 6669 6c65 5f64 6573 6372 6970      file_descrip
-0000f8a0: 746f 722e 7772 6974 6528 6475 6d70 7328  tor.write(dumps(
-0000f8b0: 7365 6c66 2e70 7265 662c 2069 6e64 656e  self.pref, inden
-0000f8c0: 743d 3429 290a 2020 2020 2020 2020 2020  t=4)).          
-0000f8d0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000f8e0: 2e69 6e66 6f28 2225 7322 2c20 7365 6c66  .info("%s", self
-0000f8f0: 2e70 7265 6629 0a20 2020 2020 2020 2065  .pref).        e
-0000f900: 7863 6570 7420 494f 4572 726f 7220 6173  xcept IOError as
-0000f910: 2065 7863 6570 7469 6f6e 3a0a 2020 2020   exception:.    
-0000f920: 2020 2020 2020 2020 6c6f 6767 6572 2e63          logger.c
-0000f930: 7269 7469 6361 6c28 2245 7272 6f72 3a20  ritical("Error: 
-0000f940: 2573 222c 2065 7863 6570 7469 6f6e 290a  %s", exception).
-0000f950: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
-0000f960: 6f6b 5f75 7020 3d20 4e6f 6e65 0a20 2020  ok_up = None.   
-0000f970: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
-0000f980: 662e 6765 7428 2275 7365 7172 7a22 293a  f.get("useqrz"):
-0000f990: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f9a0: 662e 6c6f 6f6b 5f75 7020 3d20 5152 5a6c  f.look_up = QRZl
-0000f9b0: 6f6f 6b75 7028 0a20 2020 2020 2020 2020  ookup(.         
-0000f9c0: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-0000f9d0: 2e67 6574 2822 6c6f 6f6b 7570 7573 6572  .get("lookupuser
-0000f9e0: 6e61 6d65 2229 2c0a 2020 2020 2020 2020  name"),.        
-0000f9f0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-0000fa00: 662e 6765 7428 226c 6f6f 6b75 7070 6173  f.get("lookuppas
-0000fa10: 7377 6f72 6422 292c 0a20 2020 2020 2020  sword"),.       
-0000fa20: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
-0000fa30: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
-0000fa40: 7428 2275 7365 6861 6d64 6222 293a 0a20  t("usehamdb"):. 
-0000fa50: 2020 2020 2020 2023 2020 2020 2073 656c         #     sel
-0000fa60: 662e 6c6f 6f6b 5f75 7020 3d20 4861 6d44  f.look_up = HamD
-0000fa70: 426c 6f6f 6b75 7028 290a 2020 2020 2020  Blookup().      
-0000fa80: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-0000fa90: 6574 2822 7573 6568 616d 7174 6822 293a  et("usehamqth"):
-0000faa0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fab0: 662e 6c6f 6f6b 5f75 7020 3d20 4861 6d51  f.look_up = HamQ
-0000fac0: 5448 280a 2020 2020 2020 2020 2020 2020  TH(.            
-0000fad0: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
-0000fae0: 7428 226c 6f6f 6b75 7075 7365 726e 616d  t("lookupusernam
-0000faf0: 6522 292c 0a20 2020 2020 2020 2020 2020  e"),.           
-0000fb00: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
-0000fb10: 6574 2822 6c6f 6f6b 7570 7061 7373 776f  et("lookuppasswo
-0000fb20: 7264 2229 2c0a 2020 2020 2020 2020 2020  rd"),.          
-0000fb30: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
-0000fb40: 7365 6c66 2e70 7265 662e 6765 7428 2272  self.pref.get("r
-0000fb50: 756e 5f73 7461 7465 2229 3a0a 2020 2020  un_state"):.    
-0000fb60: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-0000fb70: 696f 4275 7474 6f6e 5f72 756e 2e73 6574  ioButton_run.set
-0000fb80: 4368 6563 6b65 6428 5472 7565 290a 2020  Checked(True).  
-0000fb90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000fba0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-0000fbb0: 696f 4275 7474 6f6e 5f73 702e 7365 7443  ioButton_sp.setC
-0000fbc0: 6865 636b 6564 2854 7275 6529 0a0a 2020  hecked(True)..  
-0000fbd0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000fbe0: 6566 2e67 6574 2822 636f 6d6d 616e 645f  ef.get("command_
-0000fbf0: 6275 7474 6f6e 7322 293a 0a20 2020 2020  buttons"):.     
-0000fc00: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-0000fc10: 6f6e 436f 6d6d 616e 645f 4275 7474 6f6e  onCommand_Button
-0000fc20: 732e 7365 7443 6865 636b 6564 2854 7275  s.setChecked(Tru
-0000fc30: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
-0000fc40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fc50: 662e 6163 7469 6f6e 436f 6d6d 616e 645f  f.actionCommand_
-0000fc60: 4275 7474 6f6e 732e 7365 7443 6865 636b  Buttons.setCheck
-0000fc70: 6564 2846 616c 7365 290a 0a20 2020 2020  ed(False)..     
-0000fc80: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
-0000fc90: 6765 7428 2263 775f 6d61 6372 6f73 2229  get("cw_macros")
-0000fca0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000fcb0: 6c66 2e61 6374 696f 6e43 575f 4d61 6372  lf.actionCW_Macr
-0000fcc0: 6f73 2e73 6574 4368 6563 6b65 6428 5472  os.setChecked(Tr
-0000fcd0: 7565 290a 2020 2020 2020 2020 656c 7365  ue).        else
-0000fce0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000fcf0: 6c66 2e61 6374 696f 6e43 575f 4d61 6372  lf.actionCW_Macr
-0000fd00: 6f73 2e73 6574 4368 6563 6b65 6428 4661  os.setChecked(Fa
-0000fd10: 6c73 6529 0a0a 2020 2020 2020 2020 6966  lse)..        if
-0000fd20: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-0000fd30: 6261 6e64 735f 6d6f 6465 7322 293a 0a20  bands_modes"):. 
-0000fd40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fd50: 6163 7469 6f6e 4d6f 6465 5f61 6e64 5f42  actionMode_and_B
-0000fd60: 616e 6473 2e73 6574 4368 6563 6b65 6428  ands.setChecked(
-0000fd70: 5472 7565 290a 2020 2020 2020 2020 656c  True).        el
-0000fd80: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000fd90: 7365 6c66 2e61 6374 696f 6e4d 6f64 655f  self.actionMode_
-0000fda0: 616e 645f 4261 6e64 732e 7365 7443 6865  and_Bands.setChe
-0000fdb0: 636b 6564 2846 616c 7365 290a 0a20 2020  cked(False)..   
-0000fdc0: 2020 2020 206d 756c 7469 6361 7374 5f67       multicast_g
-0000fdd0: 726f 7570 203d 2073 656c 662e 7072 6566  roup = self.pref
-0000fde0: 2e67 6574 2822 6d75 6c74 6963 6173 745f  .get("multicast_
-0000fdf0: 6772 6f75 7022 2c20 2232 3339 2e31 2e31  group", "239.1.1
-0000fe00: 2e31 2229 0a20 2020 2020 2020 206d 756c  .1").        mul
-0000fe10: 7469 6361 7374 5f70 6f72 7420 3d20 7365  ticast_port = se
-0000fe20: 6c66 2e70 7265 662e 6765 7428 226d 756c  lf.pref.get("mul
-0000fe30: 7469 6361 7374 5f70 6f72 7422 2c20 3232  ticast_port", 22
-0000fe40: 3339 290a 2020 2020 2020 2020 696e 7465  39).        inte
-0000fe50: 7266 6163 655f 6970 203d 2073 656c 662e  rface_ip = self.
-0000fe60: 7072 6566 2e67 6574 2822 696e 7465 7266  pref.get("interf
-0000fe70: 6163 655f 6970 222c 2022 302e 302e 302e  ace_ip", "0.0.0.
-0000fe80: 3022 290a 2020 2020 2020 2020 7365 6c66  0").        self
-0000fe90: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-0000fea0: 6661 6365 203d 204d 756c 7469 6361 7374  face = Multicast
-0000feb0: 280a 2020 2020 2020 2020 2020 2020 6d75  (.            mu
-0000fec0: 6c74 6963 6173 745f 6772 6f75 702c 206d  lticast_group, m
-0000fed0: 756c 7469 6361 7374 5f70 6f72 742c 2069  ulticast_port, i
-0000fee0: 6e74 6572 6661 6365 5f69 700a 2020 2020  nterface_ip.    
-0000fef0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-0000ff00: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-0000ff10: 6572 6661 6365 2e72 6561 6479 5f72 6561  erface.ready_rea
-0000ff20: 645f 636f 6e6e 6563 7428 7365 6c66 2e77  d_connect(self.w
-0000ff30: 6174 6368 5f75 6470 290a 0a20 2020 2020  atch_udp)..     
-0000ff40: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
-0000ff50: 726f 6c20 3d20 4e6f 6e65 0a0a 2020 2020  rol = None..    
-0000ff60: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
-0000ff70: 2e67 6574 2822 7573 6566 6c72 6967 222c  .get("useflrig",
-0000ff80: 2046 616c 7365 293a 0a20 2020 2020 2020   False):.       
-0000ff90: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000ffa0: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
-0000ffb0: 2020 2022 5573 696e 6720 666c 7269 673a     "Using flrig:
-0000ffc0: 2025 7322 2c0a 2020 2020 2020 2020 2020   %s",.          
-0000ffd0: 2020 2020 2020 6622 7b73 656c 662e 7072        f"{self.pr
-0000ffe0: 6566 2e67 6574 2827 4341 545f 6970 2729  ef.get('CAT_ip')
-0000fff0: 7d20 7b73 656c 662e 7072 6566 2e67 6574  } {self.pref.get
-00010000: 2827 4341 545f 706f 7274 2729 7d22 2c0a  ('CAT_port')}",.
-00010010: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00010020: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00010030: 6967 5f63 6f6e 7472 6f6c 203d 2043 4154  ig_control = CAT
-00010040: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010050: 2020 2266 6c72 6967 222c 0a20 2020 2020    "flrig",.     
-00010060: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010070: 7072 6566 2e67 6574 2822 4341 545f 6970  pref.get("CAT_ip
-00010080: 222c 2022 3132 372e 302e 302e 3122 292c  ", "127.0.0.1"),
-00010090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000100a0: 2069 6e74 2873 656c 662e 7072 6566 2e67   int(self.pref.g
-000100b0: 6574 2822 4341 545f 706f 7274 222c 2031  et("CAT_port", 1
-000100c0: 3233 3435 2929 2c0a 2020 2020 2020 2020  2345)),.        
-000100d0: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
-000100e0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-000100f0: 7573 6572 6967 6374 6c64 222c 2046 616c  userigctld", Fal
-00010100: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
-00010110: 206c 6f67 6765 722e 6465 6275 6728 0a20   logger.debug(. 
-00010120: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00010130: 5573 696e 6720 7269 6763 746c 643a 2025  Using rigctld: %
-00010140: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00010150: 2020 2020 6622 7b73 656c 662e 7072 6566      f"{self.pref
-00010160: 2e67 6574 2827 4341 545f 6970 2729 7d20  .get('CAT_ip')} 
-00010170: 7b73 656c 662e 7072 6566 2e67 6574 2827  {self.pref.get('
-00010180: 4341 545f 706f 7274 2729 7d22 2c0a 2020  CAT_port')}",.  
-00010190: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000101a0: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
-000101b0: 5f63 6f6e 7472 6f6c 203d 2043 4154 280a  _control = CAT(.
-000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101d0: 2272 6967 6374 6c64 222c 0a20 2020 2020  "rigctld",.     
-000101e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000101f0: 7072 6566 2e67 6574 2822 4341 545f 6970  pref.get("CAT_ip
-00010200: 222c 2022 3132 372e 302e 302e 3122 292c  ", "127.0.0.1"),
-00010210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010220: 2069 6e74 2873 656c 662e 7072 6566 2e67   int(self.pref.g
-00010230: 6574 2822 4341 545f 706f 7274 222c 2034  et("CAT_port", 4
-00010240: 3533 3229 292c 0a20 2020 2020 2020 2020  532)),.         
-00010250: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-00010260: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00010270: 6377 7479 7065 222c 2030 2920 3d3d 2030  cwtype", 0) == 0
-00010280: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00010290: 6c66 2e63 7720 3d20 4e6f 6e65 0a20 2020  lf.cw = None.   
-000102a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000102b0: 2020 2020 2020 2073 656c 662e 6377 203d         self.cw =
-000102c0: 2043 5728 0a20 2020 2020 2020 2020 2020   CW(.           
-000102d0: 2020 2020 2069 6e74 2873 656c 662e 7072       int(self.pr
-000102e0: 6566 2e67 6574 2822 6377 7479 7065 2229  ef.get("cwtype")
-000102f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00010300: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
-00010310: 2822 6377 6970 2229 2c0a 2020 2020 2020  ("cwip"),.      
-00010320: 2020 2020 2020 2020 2020 696e 7428 7365            int(se
-00010330: 6c66 2e70 7265 662e 6765 7428 2263 7770  lf.pref.get("cwp
-00010340: 6f72 7422 2c20 3637 3839 2929 2c0a 2020  ort", 6789)),.  
-00010350: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00010360: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-00010370: 7370 6565 6420 3d20 3230 0a20 2020 2020  speed = 20.     
-00010380: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00010390: 772e 7365 7276 6572 7479 7065 203d 3d20  w.servertype == 
-000103a0: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
-000103b0: 2020 2073 656c 662e 6377 2e73 6574 5f77     self.cw.set_w
-000103c0: 696e 6b65 7965 725f 7370 6565 6428 3230  inkeyer_speed(20
-000103d0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000103e0: 6e31 6d6d 203d 204e 6f6e 650a 2020 2020  n1mm = None.    
-000103f0: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
-00010400: 2e67 6574 2822 7365 6e64 5f6e 316d 6d5f  .get("send_n1mm_
-00010410: 7061 636b 6574 7322 2c20 4661 6c73 6529  packets", False)
-00010420: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-00010430: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00010440: 2020 2073 656c 662e 6e31 6d6d 203d 204e     self.n1mm = N
-00010450: 314d 4d28 0a20 2020 2020 2020 2020 2020  1MM(.           
-00010460: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00010470: 6566 2e67 6574 2822 6e31 6d6d 5f72 6164  ef.get("n1mm_rad
-00010480: 696f 706f 7274 222c 2022 3132 372e 302e  ioport", "127.0.
-00010490: 302e 313a 3132 3036 3022 292c 0a20 2020  0.1:12060"),.   
-000104a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104b0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-000104c0: 6e31 6d6d 5f63 6f6e 7461 6374 706f 7274  n1mm_contactport
-000104d0: 222c 2022 3132 372e 302e 302e 313a 3132  ", "127.0.0.1:12
-000104e0: 3036 3122 292c 0a20 2020 2020 2020 2020  061"),.         
-000104f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010500: 7072 6566 2e67 6574 2822 6e31 6d6d 5f6c  pref.get("n1mm_l
-00010510: 6f6f 6b75 7070 6f72 7422 2c20 2231 3237  ookupport", "127
-00010520: 2e30 2e30 2e31 3a31 3230 3630 2229 2c0a  .0.0.1:12060"),.
-00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010540: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
-00010550: 7428 226e 316d 6d5f 7363 6f72 6570 6f72  t("n1mm_scorepor
-00010560: 7422 2c20 2231 3237 2e30 2e30 2e31 3a31  t", "127.0.0.1:1
-00010570: 3230 3630 2229 2c0a 2020 2020 2020 2020  2060"),.        
-00010580: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00010590: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
-000105a0: 7565 4572 726f 723a 0a20 2020 2020 2020  ueError:.       
-000105b0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-000105c0: 7761 726e 696e 6728 2225 7322 2c20 6622  warning("%s", f"
-000105d0: 7b56 616c 7565 4572 726f 727d 2229 0a20  {ValueError}"). 
-000105e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000105f0: 6e31 6d6d 2e73 656e 645f 7261 6469 6f5f  n1mm.send_radio_
-00010600: 7061 636b 6574 7320 3d20 7365 6c66 2e70  packets = self.p
-00010610: 7265 662e 6765 7428 2273 656e 645f 6e31  ref.get("send_n1
-00010620: 6d6d 5f72 6164 696f 222c 2046 616c 7365  mm_radio", False
-00010630: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00010640: 6c66 2e6e 316d 6d2e 7365 6e64 5f63 6f6e  lf.n1mm.send_con
-00010650: 7461 6374 5f70 6163 6b65 7473 203d 2073  tact_packets = s
-00010660: 656c 662e 7072 6566 2e67 6574 2822 7365  elf.pref.get("se
-00010670: 6e64 5f6e 316d 6d5f 636f 6e74 6163 7422  nd_n1mm_contact"
-00010680: 2c20 4661 6c73 6529 0a20 2020 2020 2020  , False).       
-00010690: 2020 2020 2073 656c 662e 6e31 6d6d 2e73       self.n1mm.s
-000106a0: 656e 645f 6c6f 6f6b 7570 5f70 6163 6b65  end_lookup_packe
-000106b0: 7473 203d 2073 656c 662e 7072 6566 2e67  ts = self.pref.g
-000106c0: 6574 2822 7365 6e64 5f6e 316d 6d5f 6c6f  et("send_n1mm_lo
-000106d0: 6f6b 7570 222c 2046 616c 7365 290a 2020  okup", False).  
-000106e0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000106f0: 316d 6d2e 7365 6e64 5f73 636f 7265 5f70  1mm.send_score_p
-00010700: 6163 6b65 7473 203d 2073 656c 662e 7072  ackets = self.pr
-00010710: 6566 2e67 6574 2822 7365 6e64 5f6e 316d  ef.get("send_n1m
-00010720: 6d5f 7363 6f72 6522 2c20 4661 6c73 6529  m_score", False)
-00010730: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010740: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
-00010750: 6f5b 2253 7461 7469 6f6e 4e61 6d65 225d  o["StationName"]
-00010760: 203d 2073 656c 662e 7072 6566 2e67 6574   = self.pref.get
-00010770: 2822 6e31 6d6d 5f73 7461 7469 6f6e 5f6e  ("n1mm_station_n
-00010780: 616d 6522 2c20 2222 290a 0a20 2020 2020  ame", "")..     
-00010790: 2020 2073 656c 662e 7368 6f77 5f63 6f6d     self.show_com
-000107a0: 6d61 6e64 5f62 7574 746f 6e73 2829 0a20  mand_buttons(). 
-000107b0: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
-000107c0: 5f43 575f 6d61 6372 6f73 2829 0a20 2020  _CW_macros().   
-000107d0: 2020 2020 2023 2073 656c 662e 7368 6f77       # self.show
-000107e0: 5f62 616e 645f 6d6f 6465 2829 0a0a 2020  _band_mode()..  
-000107f0: 2020 6465 6620 7761 7463 685f 7564 7028    def watch_udp(
-00010800: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00010810: 2222 5072 6f63 6573 7320 5544 5020 6461  ""Process UDP da
-00010820: 7461 6772 616d 732e 2222 220a 2020 2020  tagrams.""".    
-00010830: 2020 2020 7768 696c 6520 7365 6c66 2e6d      while self.m
-00010840: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
-00010850: 6365 2e73 6572 7665 725f 7564 702e 6861  ce.server_udp.ha
-00010860: 7350 656e 6469 6e67 4461 7461 6772 616d  sPendingDatagram
-00010870: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00010880: 2062 756e 646c 6520 3d20 7365 6c66 2e6d   bundle = self.m
-00010890: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
-000108a0: 6365 2e73 6572 7665 725f 7564 702e 7265  ce.server_udp.re
-000108b0: 6164 4461 7461 6772 616d 280a 2020 2020  adDatagram(.    
-000108c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000108d0: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-000108e0: 6661 6365 2e73 6572 7665 725f 7564 702e  face.server_udp.
-000108f0: 7065 6e64 696e 6744 6174 6167 7261 6d53  pendingDatagramS
-00010900: 697a 6528 290a 2020 2020 2020 2020 2020  ize().          
-00010910: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00010920: 6461 7461 6772 616d 2c20 5f2c 205f 203d  datagram, _, _ =
-00010930: 2062 756e 646c 650a 2020 2020 2020 2020   bundle.        
-00010940: 2020 2020 2320 6c6f 6767 6572 2e64 6562      # logger.deb
-00010950: 7567 2864 6174 6167 7261 6d2e 6465 636f  ug(datagram.deco
-00010960: 6465 2829 290a 2020 2020 2020 2020 2020  de()).          
-00010970: 2020 6966 2064 6174 6167 7261 6d3a 0a20    if datagram:. 
-00010980: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00010990: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-000109a0: 2020 2020 2020 2020 2320 6465 6275 675f          # debug_
-000109b0: 696e 666f 203d 2066 227b 6461 7461 6772  info = f"{datagr
-000109c0: 616d 2e64 6563 6f64 6528 297d 220a 2020  am.decode()}".  
+0000da80: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000da90: 2256 6f69 6369 6e67 3a20 2573 222c 2066  "Voicing: %s", f
+0000daa0: 696c 656e 616d 6529 0a20 2020 2020 2020  ilename).       
+0000dab0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+0000dac0: 612c 205f 6673 203d 2073 662e 7265 6164  a, _fs = sf.read
+0000dad0: 2866 696c 656e 616d 652c 2064 7479 7065  (filename, dtype
+0000dae0: 3d22 666c 6f61 7433 3222 290a 2020 2020  ="float32").    
+0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db00: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000db10: 2020 2020 2020 2020 2020 2020 2073 642e               sd.
+0000db20: 6465 6661 756c 742e 6465 7669 6365 203d  default.device =
+0000db30: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000db40: 736f 756e 6464 6576 6963 6522 2c20 2264  sounddevice", "d
+0000db50: 6566 6175 6c74 2229 0a20 2020 2020 2020  efault").       
+0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db70: 2073 642e 6465 6661 756c 742e 7361 6d70   sd.default.samp
+0000db80: 6c65 7261 7465 203d 2034 3431 3030 2e30  lerate = 44100.0
+0000db90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dba0: 2020 2020 2020 2020 2073 642e 706c 6179           sd.play
+0000dbb0: 2864 6174 6129 0a20 2020 2020 2020 2020  (data).         
+0000dbc0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000dbd0: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
+0000dbe0: 2c20 6622 7b73 642e 7761 6974 2829 7d22  , f"{sd.wait()}"
+0000dbf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000dc00: 2020 2020 2020 6578 6365 7074 2073 642e        except sd.
+0000dc10: 506f 7274 4175 6469 6f45 7272 6f72 2061  PortAudioError a
+0000dc20: 7320 6572 723a 0a20 2020 2020 2020 2020  s err:.         
+0000dc30: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000dc40: 6f67 6765 722e 7761 726e 696e 6728 2225  ogger.warning("%
+0000dc50: 7322 2c20 6622 7b65 7272 7d22 290a 2020  s", f"{err}").  
+0000dc60: 2020 2020 2020 7365 6c66 2e70 7474 5f6f        self.ptt_o
+0000dc70: 6666 2829 0a0a 2020 2020 6465 6620 7074  ff()..    def pt
+0000dc80: 745f 6f6e 2873 656c 6629 3a0a 2020 2020  t_on(self):.    
+0000dc90: 2020 2020 2222 2274 7572 6e20 6f6e 2070      """turn on p
+0000dca0: 7474 2222 220a 2020 2020 2020 2020 6966  tt""".        if
+0000dcb0: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+0000dcc0: 6c3a 0a20 2020 2020 2020 2020 2020 2073  l:.            s
+0000dcd0: 656c 662e 6c65 6674 646f 742e 7365 7450  elf.leftdot.setP
+0000dce0: 6978 6d61 7028 7365 6c66 2e67 7265 656e  ixmap(self.green
+0000dcf0: 646f 7429 0a20 2020 2020 2020 2020 2020  dot).           
+0000dd00: 2061 7070 2e70 726f 6365 7373 4576 656e   app.processEven
+0000dd10: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
+0000dd20: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+0000dd30: 6c2e 7074 745f 6f6e 2829 0a0a 2020 2020  l.ptt_on()..    
+0000dd40: 6465 6620 7074 745f 6f66 6628 7365 6c66  def ptt_off(self
+0000dd50: 293a 0a20 2020 2020 2020 2022 2222 7475  ):.        """tu
+0000dd60: 726e 206f 6666 2070 7474 2222 220a 2020  rn off ptt""".  
+0000dd70: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
+0000dd80: 675f 636f 6e74 726f 6c3a 0a20 2020 2020  g_control:.     
+0000dd90: 2020 2020 2020 2073 656c 662e 6c65 6674         self.left
+0000dda0: 646f 742e 7365 7450 6978 6d61 7028 7365  dot.setPixmap(se
+0000ddb0: 6c66 2e72 6564 646f 7429 0a20 2020 2020  lf.reddot).     
+0000ddc0: 2020 2020 2020 2061 7070 2e70 726f 6365         app.proce
+0000ddd0: 7373 4576 656e 7473 2829 0a20 2020 2020  ssEvents().     
+0000dde0: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+0000ddf0: 636f 6e74 726f 6c2e 7074 745f 6f66 6628  control.ptt_off(
+0000de00: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
+0000de10: 3128 7365 6c66 293a 0a20 2020 2020 2020  1(self):.       
+0000de20: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000de30: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000de40: 2822 4631 2043 6c69 636b 6564 2229 0a20  ("F1 Clicked"). 
+0000de50: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+0000de60: 316d 6d3a 0a20 2020 2020 2020 2020 2020  1mm:.           
+0000de70: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
+0000de80: 5f69 6e66 6f5b 2246 756e 6374 696f 6e4b  _info["FunctionK
+0000de90: 6579 4361 7074 696f 6e22 5d20 3d20 7365  eyCaption"] = se
+0000dea0: 6c66 2e46 312e 746f 6f6c 5469 7028 290a  lf.F1.toolTip().
+0000deb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000dec0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000ded0: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
+0000dee0: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
+0000def0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000df00: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
+0000df10: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
+0000df20: 726f 2873 656c 662e 4631 2e74 6f6f 6c54  ro(self.F1.toolT
+0000df30: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
+0000df40: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000df50: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
+0000df60: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000df70: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
+0000df80: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000df90: 2e46 312e 746f 6f6c 5469 7028 2929 290a  .F1.toolTip())).
+0000dfa0: 0a20 2020 2064 6566 2073 656e 6466 3228  .    def sendf2(
+0000dfb0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000dfc0: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000dfd0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000dfe0: 4632 2043 6c69 636b 6564 2229 0a20 2020  F2 Clicked").   
+0000dff0: 2020 2020 2069 6620 7365 6c66 2e6e 316d       if self.n1m
+0000e000: 6d3a 0a20 2020 2020 2020 2020 2020 2073  m:.            s
+0000e010: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
+0000e020: 6e66 6f5b 2246 756e 6374 696f 6e4b 6579  nfo["FunctionKey
+0000e030: 4361 7074 696f 6e22 5d20 3d20 7365 6c66  Caption"] = self
+0000e040: 2e46 322e 746f 6f6c 5469 7028 290a 2020  .F2.toolTip().  
+0000e050: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
+0000e060: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
+0000e070: 6f64 6522 2920 696e 205b 224c 5342 222c  ode") in ["LSB",
+0000e080: 2022 5553 4222 2c20 2253 5342 225d 3a0a   "USB", "SSB"]:.
+0000e090: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e0a0: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
+0000e0b0: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+0000e0c0: 2873 656c 662e 4632 2e74 6f6f 6c54 6970  (self.F2.toolTip
+0000e0d0: 2829 2929 0a20 2020 2020 2020 2020 2020  ())).           
+0000e0e0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000e0f0: 6966 2073 656c 662e 6377 3a0a 2020 2020  if self.cw:.    
+0000e100: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
+0000e110: 7365 6e64 6377 2873 656c 662e 7072 6f63  sendcw(self.proc
+0000e120: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
+0000e130: 322e 746f 6f6c 5469 7028 2929 290a 0a20  2.toolTip())).. 
+0000e140: 2020 2064 6566 2073 656e 6466 3328 7365     def sendf3(se
+0000e150: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000e160: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000e170: 6c6f 6767 6572 2e64 6562 7567 2822 4633  logger.debug("F3
+0000e180: 2043 6c69 636b 6564 2229 0a20 2020 2020   Clicked").     
+0000e190: 2020 2069 6620 7365 6c66 2e6e 316d 6d3a     if self.n1mm:
+0000e1a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e1b0: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
+0000e1c0: 6f5b 2246 756e 6374 696f 6e4b 6579 4361  o["FunctionKeyCa
+0000e1d0: 7074 696f 6e22 5d20 3d20 7365 6c66 2e46  ption"] = self.F
+0000e1e0: 332e 746f 6f6c 5469 7028 290a 2020 2020  3.toolTip().    
+0000e1f0: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
+0000e200: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
+0000e210: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
+0000e220: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
+0000e230: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+0000e240: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
+0000e250: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
+0000e260: 656c 662e 4633 2e74 6f6f 6c54 6970 2829  elf.F3.toolTip()
+0000e270: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0000e280: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+0000e290: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
+0000e2a0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+0000e2b0: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
+0000e2c0: 735f 6d61 6372 6f28 7365 6c66 2e46 332e  s_macro(self.F3.
+0000e2d0: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
+0000e2e0: 2064 6566 2073 656e 6466 3428 7365 6c66   def sendf4(self
+0000e2f0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000e300: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000e310: 6767 6572 2e64 6562 7567 2822 4634 2043  gger.debug("F4 C
+0000e320: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
+0000e330: 2069 6620 7365 6c66 2e6e 316d 6d3a 0a20   if self.n1mm:. 
+0000e340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e350: 6e31 6d6d 2e72 6164 696f 5f69 6e66 6f5b  n1mm.radio_info[
+0000e360: 2246 756e 6374 696f 6e4b 6579 4361 7074  "FunctionKeyCapt
+0000e370: 696f 6e22 5d20 3d20 7365 6c66 2e46 342e  ion"] = self.F4.
+0000e380: 746f 6f6c 5469 7028 290a 2020 2020 2020  toolTip().      
+0000e390: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
+0000e3a0: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
+0000e3b0: 2920 696e 205b 224c 5342 222c 2022 5553  ) in ["LSB", "US
+0000e3c0: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
+0000e3d0: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
+0000e3e0: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
+0000e3f0: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
+0000e400: 662e 4634 2e74 6f6f 6c54 6970 2829 2929  f.F4.toolTip()))
+0000e410: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000e420: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
+0000e430: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
+0000e440: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
+0000e450: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
+0000e460: 6d61 6372 6f28 7365 6c66 2e46 342e 746f  macro(self.F4.to
+0000e470: 6f6c 5469 7028 2929 290a 0a20 2020 2064  olTip()))..    d
+0000e480: 6566 2073 656e 6466 3528 7365 6c66 293a  ef sendf5(self):
+0000e490: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
+0000e4a0: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+0000e4b0: 6572 2e64 6562 7567 2822 4635 2043 6c69  er.debug("F5 Cli
+0000e4c0: 636b 6564 2229 0a20 2020 2020 2020 2069  cked").        i
+0000e4d0: 6620 7365 6c66 2e6e 316d 6d3a 0a20 2020  f self.n1mm:.   
+0000e4e0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+0000e4f0: 6d6d 2e72 6164 696f 5f69 6e66 6f5b 2246  mm.radio_info["F
+0000e500: 756e 6374 696f 6e4b 6579 4361 7074 696f  unctionKeyCaptio
+0000e510: 6e22 5d20 3d20 7365 6c66 2e46 352e 746f  n"] = self.F5.to
+0000e520: 6f6c 5469 7028 290a 2020 2020 2020 2020  olTip().        
+0000e530: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
+0000e540: 6174 652e 6765 7428 226d 6f64 6522 2920  ate.get("mode") 
+0000e550: 696e 205b 224c 5342 222c 2022 5553 4222  in ["LSB", "USB"
+0000e560: 2c20 2253 5342 225d 3a0a 2020 2020 2020  , "SSB"]:.      
+0000e570: 2020 2020 2020 7365 6c66 2e76 6f69 6365        self.voice
+0000e580: 5f73 7472 696e 6728 7365 6c66 2e70 726f  _string(self.pro
+0000e590: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
+0000e5a0: 4635 2e74 6f6f 6c54 6970 2829 2929 0a20  F5.toolTip())). 
+0000e5b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e5c0: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
+0000e5d0: 662e 6377 3a0a 2020 2020 2020 2020 2020  f.cw:.          
+0000e5e0: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
+0000e5f0: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
+0000e600: 6372 6f28 7365 6c66 2e46 352e 746f 6f6c  cro(self.F5.tool
+0000e610: 5469 7028 2929 290a 0a20 2020 2064 6566  Tip()))..    def
+0000e620: 2073 656e 6466 3628 7365 6c66 293a 0a20   sendf6(self):. 
+0000e630: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000e640: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000e650: 2e64 6562 7567 2822 4636 2043 6c69 636b  .debug("F6 Click
+0000e660: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
+0000e670: 7365 6c66 2e6e 316d 6d3a 0a20 2020 2020  self.n1mm:.     
+0000e680: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+0000e690: 2e72 6164 696f 5f69 6e66 6f5b 2246 756e  .radio_info["Fun
+0000e6a0: 6374 696f 6e4b 6579 4361 7074 696f 6e22  ctionKeyCaption"
+0000e6b0: 5d20 3d20 7365 6c66 2e46 362e 746f 6f6c  ] = self.F6.tool
+0000e6c0: 5469 7028 290a 2020 2020 2020 2020 6966  Tip().        if
+0000e6d0: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+0000e6e0: 652e 6765 7428 226d 6f64 6522 2920 696e  e.get("mode") in
+0000e6f0: 205b 224c 5342 222c 2022 5553 4222 2c20   ["LSB", "USB", 
+0000e700: 2253 5342 225d 3a0a 2020 2020 2020 2020  "SSB"]:.        
+0000e710: 2020 2020 7365 6c66 2e76 6f69 6365 5f73      self.voice_s
+0000e720: 7472 696e 6728 7365 6c66 2e70 726f 6365  tring(self.proce
+0000e730: 7373 5f6d 6163 726f 2873 656c 662e 4636  ss_macro(self.F6
+0000e740: 2e74 6f6f 6c54 6970 2829 2929 0a20 2020  .toolTip())).   
+0000e750: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000e760: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000e770: 6377 3a0a 2020 2020 2020 2020 2020 2020  cw:.            
+0000e780: 7365 6c66 2e63 772e 7365 6e64 6377 2873  self.cw.sendcw(s
+0000e790: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
+0000e7a0: 6f28 7365 6c66 2e46 362e 746f 6f6c 5469  o(self.F6.toolTi
+0000e7b0: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
+0000e7c0: 656e 6466 3728 7365 6c66 293a 0a20 2020  endf7(self):.   
+0000e7d0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000e7e0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000e7f0: 6562 7567 2822 4637 2043 6c69 636b 6564  ebug("F7 Clicked
+0000e800: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
+0000e810: 6c66 2e6e 316d 6d3a 0a20 2020 2020 2020  lf.n1mm:.       
+0000e820: 2020 2020 2073 656c 662e 6e31 6d6d 2e72       self.n1mm.r
+0000e830: 6164 696f 5f69 6e66 6f5b 2246 756e 6374  adio_info["Funct
+0000e840: 696f 6e4b 6579 4361 7074 696f 6e22 5d20  ionKeyCaption"] 
+0000e850: 3d20 7365 6c66 2e46 372e 746f 6f6c 5469  = self.F7.toolTi
+0000e860: 7028 290a 2020 2020 2020 2020 6966 2073  p().        if s
+0000e870: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+0000e880: 6765 7428 226d 6f64 6522 2920 696e 205b  get("mode") in [
+0000e890: 224c 5342 222c 2022 5553 4222 2c20 2253  "LSB", "USB", "S
+0000e8a0: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
+0000e8b0: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
+0000e8c0: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
+0000e8d0: 5f6d 6163 726f 2873 656c 662e 4637 2e74  _macro(self.F7.t
+0000e8e0: 6f6f 6c54 6970 2829 2929 0a20 2020 2020  oolTip())).     
+0000e8f0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000e900: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+0000e910: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000e920: 6c66 2e63 772e 7365 6e64 6377 2873 656c  lf.cw.sendcw(sel
+0000e930: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
+0000e940: 7365 6c66 2e46 372e 746f 6f6c 5469 7028  self.F7.toolTip(
+0000e950: 2929 290a 0a20 2020 2064 6566 2073 656e  )))..    def sen
+0000e960: 6466 3828 7365 6c66 293a 0a20 2020 2020  df8(self):.     
+0000e970: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000e980: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000e990: 7567 2822 4638 2043 6c69 636b 6564 2229  ug("F8 Clicked")
+0000e9a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000e9b0: 2e6e 316d 6d3a 0a20 2020 2020 2020 2020  .n1mm:.         
+0000e9c0: 2020 2073 656c 662e 6e31 6d6d 2e72 6164     self.n1mm.rad
+0000e9d0: 696f 5f69 6e66 6f5b 2246 756e 6374 696f  io_info["Functio
+0000e9e0: 6e4b 6579 4361 7074 696f 6e22 5d20 3d20  nKeyCaption"] = 
+0000e9f0: 7365 6c66 2e46 382e 746f 6f6c 5469 7028  self.F8.toolTip(
+0000ea00: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000ea10: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+0000ea20: 7428 226d 6f64 6522 2920 696e 205b 224c  t("mode") in ["L
+0000ea30: 5342 222c 2022 5553 4222 2c20 2253 5342  SB", "USB", "SSB
+0000ea40: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+0000ea50: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
+0000ea60: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
+0000ea70: 6163 726f 2873 656c 662e 4638 2e74 6f6f  acro(self.F8.too
+0000ea80: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
+0000ea90: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000eaa0: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
+0000eab0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000eac0: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
+0000ead0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000eae0: 6c66 2e46 382e 746f 6f6c 5469 7028 2929  lf.F8.toolTip())
+0000eaf0: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
+0000eb00: 3928 7365 6c66 293a 0a20 2020 2020 2020  9(self):.       
+0000eb10: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000eb20: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000eb30: 2822 4639 2043 6c69 636b 6564 2229 0a20  ("F9 Clicked"). 
+0000eb40: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+0000eb50: 316d 6d3a 0a20 2020 2020 2020 2020 2020  1mm:.           
+0000eb60: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
+0000eb70: 5f69 6e66 6f5b 2246 756e 6374 696f 6e4b  _info["FunctionK
+0000eb80: 6579 4361 7074 696f 6e22 5d20 3d20 7365  eyCaption"] = se
+0000eb90: 6c66 2e46 392e 746f 6f6c 5469 7028 290a  lf.F9.toolTip().
+0000eba0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000ebb0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000ebc0: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
+0000ebd0: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
+0000ebe0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000ebf0: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
+0000ec00: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
+0000ec10: 726f 2873 656c 662e 4639 2e74 6f6f 6c54  ro(self.F9.toolT
+0000ec20: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
+0000ec30: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000ec40: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
+0000ec50: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000ec60: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
+0000ec70: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000ec80: 2e46 392e 746f 6f6c 5469 7028 2929 290a  .F9.toolTip())).
+0000ec90: 0a20 2020 2064 6566 2073 656e 6466 3130  .    def sendf10
+0000eca0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000ecb0: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
+0000ecc0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000ecd0: 2246 3130 2043 6c69 636b 6564 2229 0a20  "F10 Clicked"). 
+0000ece0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+0000ecf0: 316d 6d3a 0a20 2020 2020 2020 2020 2020  1mm:.           
+0000ed00: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
+0000ed10: 5f69 6e66 6f5b 2246 756e 6374 696f 6e4b  _info["FunctionK
+0000ed20: 6579 4361 7074 696f 6e22 5d20 3d20 7365  eyCaption"] = se
+0000ed30: 6c66 2e46 3130 2e74 6f6f 6c54 6970 2829  lf.F10.toolTip()
+0000ed40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000ed50: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+0000ed60: 2822 6d6f 6465 2229 2069 6e20 5b22 4c53  ("mode") in ["LS
+0000ed70: 4222 2c20 2255 5342 222c 2022 5353 4222  B", "USB", "SSB"
+0000ed80: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
+0000ed90: 656c 662e 766f 6963 655f 7374 7269 6e67  elf.voice_string
+0000eda0: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
+0000edb0: 6372 6f28 7365 6c66 2e46 3130 2e74 6f6f  cro(self.F10.too
+0000edc0: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
+0000edd0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000ede0: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
+0000edf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ee00: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
+0000ee10: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000ee20: 6c66 2e46 3130 2e74 6f6f 6c54 6970 2829  lf.F10.toolTip()
+0000ee30: 2929 0a0a 2020 2020 6465 6620 7365 6e64  ))..    def send
+0000ee40: 6631 3128 7365 6c66 293a 0a20 2020 2020  f11(self):.     
+0000ee50: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000ee60: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000ee70: 7567 2822 4631 3120 436c 6963 6b65 6422  ug("F11 Clicked"
+0000ee80: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000ee90: 662e 6e31 6d6d 3a0a 2020 2020 2020 2020  f.n1mm:.        
+0000eea0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
+0000eeb0: 6469 6f5f 696e 666f 5b22 4675 6e63 7469  dio_info["Functi
+0000eec0: 6f6e 4b65 7943 6170 7469 6f6e 225d 203d  onKeyCaption"] =
+0000eed0: 2073 656c 662e 4631 312e 746f 6f6c 5469   self.F11.toolTi
+0000eee0: 7028 290a 2020 2020 2020 2020 6966 2073  p().        if s
+0000eef0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+0000ef00: 6765 7428 226d 6f64 6522 2920 696e 205b  get("mode") in [
+0000ef10: 224c 5342 222c 2022 5553 4222 2c20 2253  "LSB", "USB", "S
+0000ef20: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
+0000ef30: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
+0000ef40: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
+0000ef50: 5f6d 6163 726f 2873 656c 662e 4631 312e  _macro(self.F11.
+0000ef60: 746f 6f6c 5469 7028 2929 290a 2020 2020  toolTip())).    
+0000ef70: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000ef80: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000ef90: 773a 0a20 2020 2020 2020 2020 2020 2073  w:.            s
+0000efa0: 656c 662e 6377 2e73 656e 6463 7728 7365  elf.cw.sendcw(se
+0000efb0: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+0000efc0: 2873 656c 662e 4631 312e 746f 6f6c 5469  (self.F11.toolTi
+0000efd0: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
+0000efe0: 656e 6466 3132 2873 656c 6629 3a0a 2020  endf12(self):.  
+0000eff0: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
+0000f000: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000f010: 6465 6275 6728 2246 3132 2043 6c69 636b  debug("F12 Click
+0000f020: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
+0000f030: 7365 6c66 2e6e 316d 6d3a 0a20 2020 2020  self.n1mm:.     
+0000f040: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+0000f050: 2e72 6164 696f 5f69 6e66 6f5b 2246 756e  .radio_info["Fun
+0000f060: 6374 696f 6e4b 6579 4361 7074 696f 6e22  ctionKeyCaption"
+0000f070: 5d20 3d20 7365 6c66 2e46 3132 2e74 6f6f  ] = self.F12.too
+0000f080: 6c54 6970 2829 0a20 2020 2020 2020 2069  lTip().        i
+0000f090: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
+0000f0a0: 7465 2e67 6574 2822 6d6f 6465 2229 2069  te.get("mode") i
+0000f0b0: 6e20 5b22 4c53 4222 2c20 2255 5342 222c  n ["LSB", "USB",
+0000f0c0: 2022 5353 4222 5d3a 0a20 2020 2020 2020   "SSB"]:.       
+0000f0d0: 2020 2020 2073 656c 662e 766f 6963 655f       self.voice_
+0000f0e0: 7374 7269 6e67 2873 656c 662e 7072 6f63  string(self.proc
+0000f0f0: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
+0000f100: 3132 2e74 6f6f 6c54 6970 2829 2929 0a20  12.toolTip())). 
+0000f110: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000f120: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
+0000f130: 662e 6377 3a0a 2020 2020 2020 2020 2020  f.cw:.          
+0000f140: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
+0000f150: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
+0000f160: 6372 6f28 7365 6c66 2e46 3132 2e74 6f6f  cro(self.F12.too
+0000f170: 6c54 6970 2829 2929 0a0a 2020 2020 6465  lTip()))..    de
+0000f180: 6620 7275 6e5f 7370 5f62 7574 746f 6e73  f run_sp_buttons
+0000f190: 5f63 6c69 636b 6564 2873 656c 6629 3a0a  _clicked(self):.
+0000f1a0: 2020 2020 2020 2020 2222 2248 616e 646c          """Handl
+0000f1b0: 6520 7275 6e2f 7326 7020 6d6f 6465 2222  e run/s&p mode""
+0000f1c0: 220a 2020 2020 2020 2020 7365 6c66 2e70  ".        self.p
+0000f1d0: 7265 665b 2272 756e 5f73 7461 7465 225d  ref["run_state"]
+0000f1e0: 203d 2073 656c 662e 7261 6469 6f42 7574   = self.radioBut
+0000f1f0: 746f 6e5f 7275 6e2e 6973 4368 6563 6b65  ton_run.isChecke
+0000f200: 6428 290a 2020 2020 2020 2020 7365 6c66  d().        self
+0000f210: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
+0000f220: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+0000f230: 2e72 6561 645f 6377 5f6d 6163 726f 7328  .read_cw_macros(
+0000f240: 290a 0a20 2020 2064 6566 2077 7269 7465  )..    def write
+0000f250: 5f70 7265 6665 7265 6e63 6528 7365 6c66  _preference(self
+0000f260: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000f270: 2020 2020 2020 2057 7269 7465 2070 7265         Write pre
+0000f280: 6665 7265 6e63 6573 2074 6f20 6a73 6f6e  ferences to json
+0000f290: 2066 696c 652e 0a20 2020 2020 2020 2022   file..        "
+0000f2a0: 2222 0a20 2020 2020 2020 2074 7279 3a0a  "".        try:.
+0000f2b0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000f2c0: 206f 7065 6e28 0a20 2020 2020 2020 2020   open(.         
+0000f2d0: 2020 2020 2020 2043 4f4e 4649 475f 5041         CONFIG_PA
+0000f2e0: 5448 202b 2022 2f6e 6f74 316d 6d2e 6a73  TH + "/not1mm.js
+0000f2f0: 6f6e 222c 2022 7774 222c 2065 6e63 6f64  on", "wt", encod
+0000f300: 696e 673d 2275 7466 2d38 220a 2020 2020  ing="utf-8".    
+0000f310: 2020 2020 2020 2020 2920 6173 2066 696c          ) as fil
+0000f320: 655f 6465 7363 7269 7074 6f72 3a0a 2020  e_descriptor:.  
+0000f330: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0000f340: 6c65 5f64 6573 6372 6970 746f 722e 7772  le_descriptor.wr
+0000f350: 6974 6528 6475 6d70 7328 7365 6c66 2e70  ite(dumps(self.p
+0000f360: 7265 662c 2069 6e64 656e 743d 3429 290a  ref, indent=4)).
+0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f380: 6c6f 6767 6572 2e69 6e66 6f28 2277 7269  logger.info("wri
+0000f390: 7469 6e67 3a20 2573 222c 2073 656c 662e  ting: %s", self.
+0000f3a0: 7072 6566 290a 2020 2020 2020 2020 6578  pref).        ex
+0000f3b0: 6365 7074 2049 4f45 7272 6f72 2061 7320  cept IOError as 
+0000f3c0: 6578 6365 7074 696f 6e3a 0a20 2020 2020  exception:.     
+0000f3d0: 2020 2020 2020 206c 6f67 6765 722e 6372         logger.cr
+0000f3e0: 6974 6963 616c 2822 7772 6974 6570 7265  itical("writepre
+0000f3f0: 6665 7265 6e63 6573 3a20 2573 222c 2065  ferences: %s", e
+0000f400: 7863 6570 7469 6f6e 290a 0a20 2020 2064  xception)..    d
+0000f410: 6566 2072 6561 6470 7265 6665 7265 6e63  ef readpreferenc
+0000f420: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
+0000f430: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+0000f440: 7374 6f72 6520 7072 6566 6572 656e 6365  store preference
+0000f450: 7320 6966 2074 6865 7920 6578 6973 742c  s if they exist,
+0000f460: 206f 7468 6572 7769 7365 2063 7265 6174   otherwise creat
+0000f470: 6520 736f 6d65 2073 616e 6520 6465 6661  e some sane defa
+0000f480: 756c 7473 2e0a 2020 2020 2020 2020 2222  ults..        ""
+0000f490: 220a 2020 2020 2020 2020 7472 793a 0a20  ".        try:. 
+0000f4a0: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
+0000f4b0: 2e70 6174 682e 6578 6973 7473 2843 4f4e  .path.exists(CON
+0000f4c0: 4649 475f 5041 5448 202b 2022 2f6e 6f74  FIG_PATH + "/not
+0000f4d0: 316d 6d2e 6a73 6f6e 2229 3a0a 2020 2020  1mm.json"):.    
+0000f4e0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000f4f0: 206f 7065 6e28 0a20 2020 2020 2020 2020   open(.         
+0000f500: 2020 2020 2020 2020 2020 2043 4f4e 4649             CONFI
+0000f510: 475f 5041 5448 202b 2022 2f6e 6f74 316d  G_PATH + "/not1m
+0000f520: 6d2e 6a73 6f6e 222c 2022 7274 222c 2065  m.json", "rt", e
+0000f530: 6e63 6f64 696e 673d 2275 7466 2d38 220a  ncoding="utf-8".
+0000f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f550: 2920 6173 2066 696c 655f 6465 7363 7269  ) as file_descri
+0000f560: 7074 6f72 3a0a 2020 2020 2020 2020 2020  ptor:.          
+0000f570: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000f580: 7265 6620 3d20 6c6f 6164 7328 6669 6c65  ref = loads(file
+0000f590: 5f64 6573 6372 6970 746f 722e 7265 6164  _descriptor.read
+0000f5a0: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+0000f5b0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+0000f5c0: 6e66 6f28 2225 7322 2c20 7365 6c66 2e70  nfo("%s", self.p
+0000f5d0: 7265 6629 0a20 2020 2020 2020 2020 2020  ref).           
+0000f5e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000f5f0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000f600: 666f 2822 4e6f 2070 7265 6665 7265 6e63  fo("No preferenc
+0000f610: 6520 6669 6c65 2e20 5772 6974 696e 6720  e file. Writing 
+0000f620: 7072 6566 6572 656e 6365 2e22 290a 2020  preference.").  
+0000f630: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+0000f640: 7468 206f 7065 6e28 0a20 2020 2020 2020  th open(.       
+0000f650: 2020 2020 2020 2020 2020 2020 2043 4f4e               CON
+0000f660: 4649 475f 5041 5448 202b 2022 2f6e 6f74  FIG_PATH + "/not
+0000f670: 316d 6d2e 6a73 6f6e 222c 2022 7774 222c  1mm.json", "wt",
+0000f680: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+0000f690: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000f6a0: 2020 2920 6173 2066 696c 655f 6465 7363    ) as file_desc
+0000f6b0: 7269 7074 6f72 3a0a 2020 2020 2020 2020  riptor:.        
+0000f6c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f6d0: 2e70 7265 6620 3d20 7365 6c66 2e70 7265  .pref = self.pre
+0000f6e0: 665f 7265 662e 636f 7079 2829 0a20 2020  f_ref.copy().   
+0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f700: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
+0000f710: 2e77 7269 7465 2864 756d 7073 2873 656c  .write(dumps(sel
+0000f720: 662e 7072 6566 2c20 696e 6465 6e74 3d34  f.pref, indent=4
+0000f730: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0000f740: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000f750: 666f 2822 2573 222c 2073 656c 662e 7072  fo("%s", self.pr
+0000f760: 6566 290a 2020 2020 2020 2020 6578 6365  ef).        exce
+0000f770: 7074 2049 4f45 7272 6f72 2061 7320 6578  pt IOError as ex
+0000f780: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
+0000f790: 2020 2020 206c 6f67 6765 722e 6372 6974       logger.crit
+0000f7a0: 6963 616c 2822 4572 726f 723a 2025 7322  ical("Error: %s"
+0000f7b0: 2c20 6578 6365 7074 696f 6e29 0a0a 2020  , exception)..  
+0000f7c0: 2020 2020 2020 7365 6c66 2e6c 6f6f 6b5f        self.look_
+0000f7d0: 7570 203d 204e 6f6e 650a 2020 2020 2020  up = None.      
+0000f7e0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+0000f7f0: 6574 2822 7573 6571 727a 2229 3a0a 2020  et("useqrz"):.  
+0000f800: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0000f810: 6f6f 6b5f 7570 203d 2051 525a 6c6f 6f6b  ook_up = QRZlook
+0000f820: 7570 280a 2020 2020 2020 2020 2020 2020  up(.            
+0000f830: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
+0000f840: 7428 226c 6f6f 6b75 7075 7365 726e 616d  t("lookupusernam
+0000f850: 6522 292c 0a20 2020 2020 2020 2020 2020  e"),.           
+0000f860: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
+0000f870: 6574 2822 6c6f 6f6b 7570 7061 7373 776f  et("lookuppasswo
+0000f880: 7264 2229 2c0a 2020 2020 2020 2020 2020  rd"),.          
+0000f890: 2020 290a 2020 2020 2020 2020 2320 6966    ).        # if
+0000f8a0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000f8b0: 7573 6568 616d 6462 2229 3a0a 2020 2020  usehamdb"):.    
+0000f8c0: 2020 2020 2320 2020 2020 7365 6c66 2e6c      #     self.l
+0000f8d0: 6f6f 6b5f 7570 203d 2048 616d 4442 6c6f  ook_up = HamDBlo
+0000f8e0: 6f6b 7570 2829 0a20 2020 2020 2020 2069  okup().        i
+0000f8f0: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+0000f900: 2275 7365 6861 6d71 7468 2229 3a0a 2020  "usehamqth"):.  
+0000f910: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0000f920: 6f6f 6b5f 7570 203d 2048 616d 5154 4828  ook_up = HamQTH(
+0000f930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f940: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000f950: 6c6f 6f6b 7570 7573 6572 6e61 6d65 2229  lookupusername")
+0000f960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f970: 2020 7365 6c66 2e70 7265 662e 6765 7428    self.pref.get(
+0000f980: 226c 6f6f 6b75 7070 6173 7377 6f72 6422  "lookuppassword"
+0000f990: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
+0000f9a0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000f9b0: 662e 7072 6566 2e67 6574 2822 7275 6e5f  f.pref.get("run_
+0000f9c0: 7374 6174 6522 293a 0a20 2020 2020 2020  state"):.       
+0000f9d0: 2020 2020 2073 656c 662e 7261 6469 6f42       self.radioB
+0000f9e0: 7574 746f 6e5f 7275 6e2e 7365 7443 6865  utton_run.setChe
+0000f9f0: 636b 6564 2854 7275 6529 0a20 2020 2020  cked(True).     
+0000fa00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000fa10: 2020 2020 2073 656c 662e 7261 6469 6f42       self.radioB
+0000fa20: 7574 746f 6e5f 7370 2e73 6574 4368 6563  utton_sp.setChec
+0000fa30: 6b65 6428 5472 7565 290a 0a20 2020 2020  ked(True)..     
+0000fa40: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
+0000fa50: 6765 7428 2263 6f6d 6d61 6e64 5f62 7574  get("command_but
+0000fa60: 746f 6e73 2229 3a0a 2020 2020 2020 2020  tons"):.        
+0000fa70: 2020 2020 7365 6c66 2e61 6374 696f 6e43      self.actionC
+0000fa80: 6f6d 6d61 6e64 5f42 7574 746f 6e73 2e73  ommand_Buttons.s
+0000fa90: 6574 4368 6563 6b65 6428 5472 7565 290a  etChecked(True).
+0000faa0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000fab0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000fac0: 6374 696f 6e43 6f6d 6d61 6e64 5f42 7574  ctionCommand_But
+0000fad0: 746f 6e73 2e73 6574 4368 6563 6b65 6428  tons.setChecked(
+0000fae0: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
+0000faf0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
+0000fb00: 2822 6377 5f6d 6163 726f 7322 293a 0a20  ("cw_macros"):. 
+0000fb10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fb20: 6163 7469 6f6e 4357 5f4d 6163 726f 732e  actionCW_Macros.
+0000fb30: 7365 7443 6865 636b 6564 2854 7275 6529  setChecked(True)
+0000fb40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000fb50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fb60: 6163 7469 6f6e 4357 5f4d 6163 726f 732e  actionCW_Macros.
+0000fb70: 7365 7443 6865 636b 6564 2846 616c 7365  setChecked(False
+0000fb80: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+0000fb90: 6c66 2e70 7265 662e 6765 7428 2262 616e  lf.pref.get("ban
+0000fba0: 6473 5f6d 6f64 6573 2229 3a0a 2020 2020  ds_modes"):.    
+0000fbb0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+0000fbc0: 696f 6e4d 6f64 655f 616e 645f 4261 6e64  ionMode_and_Band
+0000fbd0: 732e 7365 7443 6865 636b 6564 2854 7275  s.setChecked(Tru
+0000fbe0: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
+0000fbf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000fc00: 662e 6163 7469 6f6e 4d6f 6465 5f61 6e64  f.actionMode_and
+0000fc10: 5f42 616e 6473 2e73 6574 4368 6563 6b65  _Bands.setChecke
+0000fc20: 6428 4661 6c73 6529 0a0a 2020 2020 2020  d(False)..      
+0000fc30: 2020 6d75 6c74 6963 6173 745f 6772 6f75    multicast_grou
+0000fc40: 7020 3d20 7365 6c66 2e70 7265 662e 6765  p = self.pref.ge
+0000fc50: 7428 226d 756c 7469 6361 7374 5f67 726f  t("multicast_gro
+0000fc60: 7570 222c 2022 3233 392e 312e 312e 3122  up", "239.1.1.1"
+0000fc70: 290a 2020 2020 2020 2020 6d75 6c74 6963  ).        multic
+0000fc80: 6173 745f 706f 7274 203d 2073 656c 662e  ast_port = self.
+0000fc90: 7072 6566 2e67 6574 2822 6d75 6c74 6963  pref.get("multic
+0000fca0: 6173 745f 706f 7274 222c 2032 3233 3929  ast_port", 2239)
+0000fcb0: 0a20 2020 2020 2020 2069 6e74 6572 6661  .        interfa
+0000fcc0: 6365 5f69 7020 3d20 7365 6c66 2e70 7265  ce_ip = self.pre
+0000fcd0: 662e 6765 7428 2269 6e74 6572 6661 6365  f.get("interface
+0000fce0: 5f69 7022 2c20 2230 2e30 2e30 2e30 2229  _ip", "0.0.0.0")
+0000fcf0: 0a20 2020 2020 2020 2073 656c 662e 6d75  .        self.mu
+0000fd00: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
+0000fd10: 6520 3d20 4d75 6c74 6963 6173 7428 0a20  e = Multicast(. 
+0000fd20: 2020 2020 2020 2020 2020 206d 756c 7469             multi
+0000fd30: 6361 7374 5f67 726f 7570 2c20 6d75 6c74  cast_group, mult
+0000fd40: 6963 6173 745f 706f 7274 2c20 696e 7465  icast_port, inte
+0000fd50: 7266 6163 655f 6970 0a20 2020 2020 2020  rface_ip.       
+0000fd60: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+0000fd70: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+0000fd80: 6163 652e 7265 6164 795f 7265 6164 5f63  ace.ready_read_c
+0000fd90: 6f6e 6e65 6374 2873 656c 662e 7761 7463  onnect(self.watc
+0000fda0: 685f 7564 7029 0a0a 2020 2020 2020 2020  h_udp)..        
+0000fdb0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+0000fdc0: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+0000fdd0: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
+0000fde0: 7428 2275 7365 666c 7269 6722 2c20 4661  t("useflrig", Fa
+0000fdf0: 6c73 6529 3a0a 2020 2020 2020 2020 2020  lse):.          
+0000fe00: 2020 6c6f 6767 6572 2e64 6562 7567 280a    logger.debug(.
+0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe20: 2255 7369 6e67 2066 6c72 6967 3a20 2573  "Using flrig: %s
+0000fe30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000fe40: 2020 2066 227b 7365 6c66 2e70 7265 662e     f"{self.pref.
+0000fe50: 6765 7428 2743 4154 5f69 7027 297d 207b  get('CAT_ip')} {
+0000fe60: 7365 6c66 2e70 7265 662e 6765 7428 2743  self.pref.get('C
+0000fe70: 4154 5f70 6f72 7427 297d 222c 0a20 2020  AT_port')}",.   
+0000fe80: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000fe90: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+0000fea0: 636f 6e74 726f 6c20 3d20 4341 5428 0a20  control = CAT(. 
+0000feb0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000fec0: 666c 7269 6722 2c0a 2020 2020 2020 2020  flrig",.        
+0000fed0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+0000fee0: 662e 6765 7428 2243 4154 5f69 7022 2c20  f.get("CAT_ip", 
+0000fef0: 2231 3237 2e30 2e30 2e31 2229 2c0a 2020  "127.0.0.1"),.  
+0000ff00: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000ff10: 7428 7365 6c66 2e70 7265 662e 6765 7428  t(self.pref.get(
+0000ff20: 2243 4154 5f70 6f72 7422 2c20 3132 3334  "CAT_port", 1234
+0000ff30: 3529 292c 0a20 2020 2020 2020 2020 2020  5)),.           
+0000ff40: 2029 0a20 2020 2020 2020 2069 6620 7365   ).        if se
+0000ff50: 6c66 2e70 7265 662e 6765 7428 2275 7365  lf.pref.get("use
+0000ff60: 7269 6763 746c 6422 2c20 4661 6c73 6529  rigctld", False)
+0000ff70: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+0000ff80: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
+0000ff90: 2020 2020 2020 2020 2020 2020 2255 7369              "Usi
+0000ffa0: 6e67 2072 6967 6374 6c64 3a20 2573 222c  ng rigctld: %s",
+0000ffb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ffc0: 2066 227b 7365 6c66 2e70 7265 662e 6765   f"{self.pref.ge
+0000ffd0: 7428 2743 4154 5f69 7027 297d 207b 7365  t('CAT_ip')} {se
+0000ffe0: 6c66 2e70 7265 662e 6765 7428 2743 4154  lf.pref.get('CAT
+0000fff0: 5f70 6f72 7427 297d 222c 0a20 2020 2020  _port')}",.     
+00010000: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00010010: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
+00010020: 6e74 726f 6c20 3d20 4341 5428 0a20 2020  ntrol = CAT(.   
+00010030: 2020 2020 2020 2020 2020 2020 2022 7269               "ri
+00010040: 6763 746c 6422 2c0a 2020 2020 2020 2020  gctld",.        
+00010050: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+00010060: 662e 6765 7428 2243 4154 5f69 7022 2c20  f.get("CAT_ip", 
+00010070: 2231 3237 2e30 2e30 2e31 2229 2c0a 2020  "127.0.0.1"),.  
+00010080: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00010090: 7428 7365 6c66 2e70 7265 662e 6765 7428  t(self.pref.get(
+000100a0: 2243 4154 5f70 6f72 7422 2c20 3435 3332  "CAT_port", 4532
+000100b0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+000100c0: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+000100d0: 6c66 2e70 7265 662e 6765 7428 2263 7774  lf.pref.get("cwt
+000100e0: 7970 6522 2c20 3029 203d 3d20 303a 0a20  ype", 0) == 0:. 
+000100f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010100: 6377 203d 204e 6f6e 650a 2020 2020 2020  cw = None.      
+00010110: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00010120: 2020 2020 7365 6c66 2e63 7720 3d20 4357      self.cw = CW
+00010130: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010140: 2020 696e 7428 7365 6c66 2e70 7265 662e    int(self.pref.
+00010150: 6765 7428 2263 7774 7970 6522 2929 2c0a  get("cwtype")),.
+00010160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010170: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
+00010180: 7769 7022 292c 0a20 2020 2020 2020 2020  wip"),.         
+00010190: 2020 2020 2020 2069 6e74 2873 656c 662e         int(self.
+000101a0: 7072 6566 2e67 6574 2822 6377 706f 7274  pref.get("cwport
+000101b0: 222c 2036 3738 3929 292c 0a20 2020 2020  ", 6789)),.     
+000101c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000101d0: 2020 2020 2073 656c 662e 6377 2e73 7065       self.cw.spe
+000101e0: 6564 203d 2032 300a 2020 2020 2020 2020  ed = 20.        
+000101f0: 2020 2020 6966 2073 656c 662e 6377 2e73      if self.cw.s
+00010200: 6572 7665 7274 7970 6520 3d3d 2032 3a0a  ervertype == 2:.
+00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010220: 7365 6c66 2e63 772e 7365 745f 7769 6e6b  self.cw.set_wink
+00010230: 6579 6572 5f73 7065 6564 2832 3029 0a0a  eyer_speed(20)..
+00010240: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+00010250: 6d20 3d20 4e6f 6e65 0a20 2020 2020 2020  m = None.       
+00010260: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
+00010270: 7428 2273 656e 645f 6e31 6d6d 5f70 6163  t("send_n1mm_pac
+00010280: 6b65 7473 222c 2046 616c 7365 293a 0a20  kets", False):. 
+00010290: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102b0: 7365 6c66 2e6e 316d 6d20 3d20 4e31 4d4d  self.n1mm = N1MM
+000102c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000102d0: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
+000102e0: 6765 7428 226e 316d 6d5f 7261 6469 6f70  get("n1mm_radiop
+000102f0: 6f72 7422 2c20 2231 3237 2e30 2e30 2e31  ort", "127.0.0.1
+00010300: 3a31 3230 3630 2229 2c0a 2020 2020 2020  :12060"),.      
+00010310: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010320: 6c66 2e70 7265 662e 6765 7428 226e 316d  lf.pref.get("n1m
+00010330: 6d5f 636f 6e74 6163 7470 6f72 7422 2c20  m_contactport", 
+00010340: 2231 3237 2e30 2e30 2e31 3a31 3230 3631  "127.0.0.1:12061
+00010350: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00010360: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+00010370: 662e 6765 7428 226e 316d 6d5f 6c6f 6f6b  f.get("n1mm_look
+00010380: 7570 706f 7274 222c 2022 3132 372e 302e  upport", "127.0.
+00010390: 302e 313a 3132 3036 3022 292c 0a20 2020  0.1:12060"),.   
+000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103b0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+000103c0: 6e31 6d6d 5f73 636f 7265 706f 7274 222c  n1mm_scoreport",
+000103d0: 2022 3132 372e 302e 302e 313a 3132 3036   "127.0.0.1:1206
+000103e0: 3022 292c 0a20 2020 2020 2020 2020 2020  0"),.           
+000103f0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00010400: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
+00010410: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+00010420: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
+00010430: 6e69 6e67 2822 2573 222c 2066 227b 5661  ning("%s", f"{Va
+00010440: 6c75 6545 7272 6f72 7d22 290a 2020 2020  lueError}").    
+00010450: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+00010460: 6d2e 7365 6e64 5f72 6164 696f 5f70 6163  m.send_radio_pac
+00010470: 6b65 7473 203d 2073 656c 662e 7072 6566  kets = self.pref
+00010480: 2e67 6574 2822 7365 6e64 5f6e 316d 6d5f  .get("send_n1mm_
+00010490: 7261 6469 6f22 2c20 4661 6c73 6529 0a20  radio", False). 
+000104a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000104b0: 6e31 6d6d 2e73 656e 645f 636f 6e74 6163  n1mm.send_contac
+000104c0: 745f 7061 636b 6574 7320 3d20 7365 6c66  t_packets = self
+000104d0: 2e70 7265 662e 6765 7428 2273 656e 645f  .pref.get("send_
+000104e0: 6e31 6d6d 5f63 6f6e 7461 6374 222c 2046  n1mm_contact", F
+000104f0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00010500: 2020 7365 6c66 2e6e 316d 6d2e 7365 6e64    self.n1mm.send
+00010510: 5f6c 6f6f 6b75 705f 7061 636b 6574 7320  _lookup_packets 
+00010520: 3d20 7365 6c66 2e70 7265 662e 6765 7428  = self.pref.get(
+00010530: 2273 656e 645f 6e31 6d6d 5f6c 6f6f 6b75  "send_n1mm_looku
+00010540: 7022 2c20 4661 6c73 6529 0a20 2020 2020  p", False).     
+00010550: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+00010560: 2e73 656e 645f 7363 6f72 655f 7061 636b  .send_score_pack
+00010570: 6574 7320 3d20 7365 6c66 2e70 7265 662e  ets = self.pref.
+00010580: 6765 7428 2273 656e 645f 6e31 6d6d 5f73  get("send_n1mm_s
+00010590: 636f 7265 222c 2046 616c 7365 290a 2020  core", False).  
+000105a0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000105b0: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
+000105c0: 5374 6174 696f 6e4e 616d 6522 5d20 3d20  StationName"] = 
+000105d0: 7365 6c66 2e70 7265 662e 6765 7428 226e  self.pref.get("n
+000105e0: 316d 6d5f 7374 6174 696f 6e5f 6e61 6d65  1mm_station_name
+000105f0: 222c 2022 2229 0a0a 2020 2020 2020 2020  ", "")..        
+00010600: 7365 6c66 2e73 686f 775f 636f 6d6d 616e  self.show_comman
+00010610: 645f 6275 7474 6f6e 7328 290a 2020 2020  d_buttons().    
+00010620: 2020 2020 7365 6c66 2e73 686f 775f 4357      self.show_CW
+00010630: 5f6d 6163 726f 7328 290a 2020 2020 2020  _macros().      
+00010640: 2020 2320 7365 6c66 2e73 686f 775f 6261    # self.show_ba
+00010650: 6e64 5f6d 6f64 6528 290a 0a20 2020 2064  nd_mode()..    d
+00010660: 6566 2077 6174 6368 5f75 6470 2873 656c  ef watch_udp(sel
+00010670: 6629 3a0a 2020 2020 2020 2020 2222 2250  f):.        """P
+00010680: 726f 6365 7373 2055 4450 2064 6174 6167  rocess UDP datag
+00010690: 7261 6d73 2e22 2222 0a20 2020 2020 2020  rams.""".       
+000106a0: 2077 6869 6c65 2073 656c 662e 6d75 6c74   while self.mult
+000106b0: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+000106c0: 7365 7276 6572 5f75 6470 2e68 6173 5065  server_udp.hasPe
+000106d0: 6e64 696e 6744 6174 6167 7261 6d73 2829  ndingDatagrams()
+000106e0: 3a0a 2020 2020 2020 2020 2020 2020 6275  :.            bu
+000106f0: 6e64 6c65 203d 2073 656c 662e 6d75 6c74  ndle = self.mult
+00010700: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+00010710: 7365 7276 6572 5f75 6470 2e72 6561 6444  server_udp.readD
+00010720: 6174 6167 7261 6d28 0a20 2020 2020 2020  atagram(.       
+00010730: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
+00010740: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
+00010750: 652e 7365 7276 6572 5f75 6470 2e70 656e  e.server_udp.pen
+00010760: 6469 6e67 4461 7461 6772 616d 5369 7a65  dingDatagramSize
+00010770: 2829 0a20 2020 2020 2020 2020 2020 2029  ().            )
+00010780: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00010790: 6167 7261 6d2c 205f 2c20 5f20 3d20 6275  agram, _, _ = bu
+000107a0: 6e64 6c65 0a20 2020 2020 2020 2020 2020  ndle.           
+000107b0: 2023 206c 6f67 6765 722e 6465 6275 6728   # logger.debug(
+000107c0: 6461 7461 6772 616d 2e64 6563 6f64 6528  datagram.decode(
+000107d0: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
+000107e0: 6620 6461 7461 6772 616d 3a0a 2020 2020  f datagram:.    
+000107f0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00010800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010810: 2020 2020 2023 2064 6562 7567 5f69 6e66       # debug_inf
+00010820: 6f20 3d20 6622 7b64 6174 6167 7261 6d2e  o = f"{datagram.
+00010830: 6465 636f 6465 2829 7d22 0a20 2020 2020  decode()}".     
+00010840: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00010850: 206c 6f67 6765 722e 6465 6275 6728 6465   logger.debug(de
+00010860: 6275 675f 696e 666f 290a 2020 2020 2020  bug_info).      
+00010870: 2020 2020 2020 2020 2020 2020 2020 6a73                js
+00010880: 6f6e 5f64 6174 6120 3d20 6c6f 6164 7328  on_data = loads(
+00010890: 6461 7461 6772 616d 2e64 6563 6f64 6528  datagram.decode(
+000108a0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000108b0: 2020 2065 7863 6570 7420 556e 6963 6f64     except Unicod
+000108c0: 6544 6563 6f64 6545 7272 6f72 2061 7320  eDecodeError as 
+000108d0: 6572 723a 0a20 2020 2020 2020 2020 2020  err:.           
+000108e0: 2020 2020 2020 2020 2074 6865 5f65 7272           the_err
+000108f0: 6f72 203d 2066 224e 6f74 2055 6e69 636f  or = f"Not Unico
+00010900: 6465 3a20 7b65 7272 7d5c 6e7b 6461 7461  de: {err}\n{data
+00010910: 6772 616d 7d22 0a20 2020 2020 2020 2020  gram}".         
+00010920: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00010930: 722e 7761 726e 696e 6728 7468 655f 6572  r.warning(the_er
+00010940: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
+00010950: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00010960: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00010970: 2020 6578 6365 7074 204a 534f 4e44 6563    except JSONDec
+00010980: 6f64 6545 7272 6f72 2061 7320 6572 723a  odeError as err:
+00010990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000109a0: 2020 2020 2074 6865 5f65 7272 6f72 203d       the_error =
+000109b0: 2066 224e 6f74 204a 534f 4e3a 207b 6572   f"Not JSON: {er
+000109c0: 727d 5c6e 7b64 6174 6167 7261 6d7d 220a  r}\n{datagram}".
 000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109e0: 2020 2320 6c6f 6767 6572 2e64 6562 7567    # logger.debug
-000109f0: 2864 6562 7567 5f69 6e66 6f29 0a20 2020  (debug_info).   
+000109e0: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+000109f0: 6e67 2874 6865 5f65 7272 6f72 290a 2020  ng(the_error).  
 00010a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a10: 206a 736f 6e5f 6461 7461 203d 206c 6f61   json_data = loa
-00010a20: 6473 2864 6174 6167 7261 6d2e 6465 636f  ds(datagram.deco
-00010a30: 6465 2829 290a 2020 2020 2020 2020 2020  de()).          
-00010a40: 2020 2020 2020 6578 6365 7074 2055 6e69        except Uni
-00010a50: 636f 6465 4465 636f 6465 4572 726f 7220  codeDecodeError 
-00010a60: 6173 2065 7272 3a0a 2020 2020 2020 2020  as err:.        
-00010a70: 2020 2020 2020 2020 2020 2020 7468 655f              the_
-00010a80: 6572 726f 7220 3d20 6622 4e6f 7420 556e  error = f"Not Un
-00010a90: 6963 6f64 653a 207b 6572 727d 5c6e 7b64  icode: {err}\n{d
-00010aa0: 6174 6167 7261 6d7d 220a 2020 2020 2020  atagram}".      
-00010ab0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00010ac0: 6767 6572 2e77 6172 6e69 6e67 2874 6865  gger.warning(the
-00010ad0: 5f65 7272 6f72 290a 2020 2020 2020 2020  _error).        
-00010ae0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00010af0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
-00010b00: 2020 2020 2065 7863 6570 7420 4a53 4f4e       except JSON
-00010b10: 4465 636f 6465 4572 726f 7220 6173 2065  DecodeError as e
-00010b20: 7272 3a0a 2020 2020 2020 2020 2020 2020  rr:.            
-00010b30: 2020 2020 2020 2020 7468 655f 6572 726f          the_erro
-00010b40: 7220 3d20 6622 4e6f 7420 4a53 4f4e 3a20  r = f"Not JSON: 
-00010b50: 7b65 7272 7d5c 6e7b 6461 7461 6772 616d  {err}\n{datagram
-00010b60: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-00010b70: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
-00010b80: 726e 696e 6728 7468 655f 6572 726f 7229  rning(the_error)
-00010b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ba0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-00010bb0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010bc0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00010bd0: 2020 2020 2020 206a 736f 6e5f 6461 7461         json_data
-00010be0: 2e67 6574 2822 636d 6422 2c20 2222 2920  .get("cmd", "") 
-00010bf0: 3d3d 2022 4745 5443 4f4c 554d 4e53 220a  == "GETCOLUMNS".
-00010c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c10: 2020 2020 616e 6420 6a73 6f6e 5f64 6174      and json_dat
-00010c20: 612e 6765 7428 2273 7461 7469 6f6e 222c  a.get("station",
-00010c30: 2022 2229 203d 3d20 706c 6174 666f 726d   "") == platform
-00010c40: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-00010c50: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00010c60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00010c70: 6620 6861 7361 7474 7228 7365 6c66 2e63  f hasattr(self.c
-00010c80: 6f6e 7465 7374 2c20 2263 6f6c 756d 6e73  ontest, "columns
-00010c90: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00010ca0: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
-00010cb0: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
-00010cc0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-00010cd0: 5b22 636d 6422 5d20 3d20 2253 484f 5743  ["cmd"] = "SHOWC
-00010ce0: 4f4c 554d 4e53 220a 2020 2020 2020 2020  OLUMNS".        
-00010cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d00: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
-00010d10: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
-00010d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010d30: 2020 2020 2020 2020 2063 6d64 5b22 434f           cmd["CO
-00010d40: 4c55 4d4e 5322 5d20 3d20 7365 6c66 2e63  LUMNS"] = self.c
-00010d50: 6f6e 7465 7374 2e63 6f6c 756d 6e73 0a20  ontest.columns. 
+00010a10: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+00010a20: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
+00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a40: 2020 2020 6a73 6f6e 5f64 6174 612e 6765      json_data.ge
+00010a50: 7428 2263 6d64 222c 2022 2229 203d 3d20  t("cmd", "") == 
+00010a60: 2247 4554 434f 4c55 4d4e 5322 0a20 2020  "GETCOLUMNS".   
+00010a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a80: 2061 6e64 206a 736f 6e5f 6461 7461 2e67   and json_data.g
+00010a90: 6574 2822 7374 6174 696f 6e22 2c20 2222  et("station", ""
+00010aa0: 2920 3d3d 2070 6c61 7466 6f72 6d2e 6e6f  ) == platform.no
+00010ab0: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00010ac0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00010ad0: 2020 2020 2020 2020 2020 2020 6966 2068              if h
+00010ae0: 6173 6174 7472 2873 656c 662e 636f 6e74  asattr(self.cont
+00010af0: 6573 742c 2022 636f 6c75 6d6e 7322 293a  est, "columns"):
+00010b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b10: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+00010b20: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00010b30: 2020 2020 2020 2020 2020 636d 645b 2263            cmd["c
+00010b40: 6d64 225d 203d 2022 5348 4f57 434f 4c55  md"] = "SHOWCOLU
+00010b50: 4d4e 5322 0a20 2020 2020 2020 2020 2020  MNS".           
+00010b60: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+00010b70: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
+00010b80: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
+00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ba0: 2020 2020 2020 636d 645b 2243 4f4c 554d        cmd["COLUM
+00010bb0: 4e53 225d 203d 2073 656c 662e 636f 6e74  NS"] = self.cont
+00010bc0: 6573 742e 636f 6c75 6d6e 730a 2020 2020  est.columns.    
+00010bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010be0: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
+00010bf0: 7374 5f69 6e74 6572 6661 6365 2e73 656e  st_interface.sen
+00010c00: 645f 6173 5f6a 736f 6e28 636d 6429 0a20  d_as_json(cmd). 
+00010c10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010c20: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00010c30: 2020 2020 2020 2020 6a73 6f6e 5f64 6174          json_dat
+00010c40: 612e 6765 7428 2263 6d64 222c 2022 2229  a.get("cmd", "")
+00010c50: 203d 3d20 2254 554e 4522 0a20 2020 2020   == "TUNE".     
+00010c60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00010c70: 6e64 206a 736f 6e5f 6461 7461 2e67 6574  nd json_data.get
+00010c80: 2822 7374 6174 696f 6e22 2c20 2222 2920  ("station", "") 
+00010c90: 3d3d 2070 6c61 7466 6f72 6d2e 6e6f 6465  == platform.node
+00010ca0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00010cb0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00010cc0: 2020 2020 2020 2020 2020 2320 6227 7b22            # b'{"
+00010cd0: 636d 6422 3a20 2254 554e 4522 2c20 2266  cmd": "TUNE", "f
+00010ce0: 7265 7122 3a20 372e 3032 3335 2c20 2273  req": 7.0235, "s
+00010cf0: 706f 7422 3a20 224d 4d30 4447 4922 7d27  pot": "MM0DGI"}'
+00010d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d10: 2020 2020 2076 666f 203d 206a 736f 6e5f       vfo = json_
+00010d20: 6461 7461 2e67 6574 2822 6672 6571 2229  data.get("freq")
+00010d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d40: 2020 2020 2076 666f 203d 2066 6c6f 6174       vfo = float
+00010d50: 2876 666f 2920 2a20 3130 3030 3030 300a  (vfo) * 1000000.
 00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d70: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
-00010d80: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
-00010d90: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
-00010da0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010db0: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
-00010dc0: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
-00010dd0: 6461 7461 2e67 6574 2822 636d 6422 2c20  data.get("cmd", 
-00010de0: 2222 2920 3d3d 2022 5455 4e45 220a 2020  "") == "TUNE".  
-00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e00: 2020 616e 6420 6a73 6f6e 5f64 6174 612e    and json_data.
-00010e10: 6765 7428 2273 7461 7469 6f6e 222c 2022  get("station", "
-00010e20: 2229 203d 3d20 706c 6174 666f 726d 2e6e  ") == platform.n
-00010e30: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
-00010e40: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-00010e50: 2020 2020 2020 2020 2020 2020 2023 2062               # b
-00010e60: 277b 2263 6d64 223a 2022 5455 4e45 222c  '{"cmd": "TUNE",
-00010e70: 2022 6672 6571 223a 2037 2e30 3233 352c   "freq": 7.0235,
-00010e80: 2022 7370 6f74 223a 2022 4d4d 3044 4749   "spot": "MM0DGI
-00010e90: 227d 270a 2020 2020 2020 2020 2020 2020  "}'.            
-00010ea0: 2020 2020 2020 2020 7666 6f20 3d20 6a73          vfo = js
-00010eb0: 6f6e 5f64 6174 612e 6765 7428 2266 7265  on_data.get("fre
-00010ec0: 7122 290a 2020 2020 2020 2020 2020 2020  q").            
-00010ed0: 2020 2020 2020 2020 7666 6f20 3d20 666c          vfo = fl
-00010ee0: 6f61 7428 7666 6f29 202a 2031 3030 3030  oat(vfo) * 10000
-00010ef0: 3030 0a20 2020 2020 2020 2020 2020 2020  00.             
-00010f00: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-00010f10: 6f5f 7374 6174 655b 2276 666f 6122 5d20  o_state["vfoa"] 
-00010f20: 3d20 696e 7428 7666 6f29 0a20 2020 2020  = int(vfo).     
-00010f30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00010f40: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
-00010f50: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
-00010f60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010f70: 2e72 6967 5f63 6f6e 7472 6f6c 2e73 6574  .rig_control.set
-00010f80: 5f76 666f 2869 6e74 2876 666f 2929 0a20  _vfo(int(vfo)). 
-00010f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fa0: 2020 2073 706f 7420 3d20 6a73 6f6e 5f64     spot = json_d
-00010fb0: 6174 612e 6765 7428 2273 706f 7422 2c20  ata.get("spot", 
-00010fc0: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
-00010fd0: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
-00010fe0: 6c73 6967 6e2e 7365 7454 6578 7428 7370  lsign.setText(sp
-00010ff0: 6f74 290a 2020 2020 2020 2020 2020 2020  ot).            
-00011000: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
-00011010: 6c73 6967 6e5f 6368 616e 6765 6428 290a  lsign_changed().
-00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011030: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
-00011040: 6e2e 7365 7446 6f63 7573 2829 0a20 2020  n.setFocus().   
-00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011060: 2073 656c 662e 6361 6c6c 7369 676e 2e61   self.callsign.a
-00011070: 6374 6976 6174 6557 696e 646f 7728 290a  ctivateWindow().
-00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011090: 2020 2020 7769 6e64 6f77 2e72 6169 7365      window.raise
-000110a0: 5f28 290a 2020 2020 2020 2020 2020 2020  _().            
-000110b0: 2020 2020 2020 2020 2320 6667 203d 2077          # fg = w
-000110c0: 696e 646f 772e 6672 616d 6547 656f 6d65  indow.frameGeome
-000110d0: 7472 7928 292e 746f 704c 6566 740a 2020  try().topLeft.  
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 2320 2320 5f77 6964 7468 203d 2073    # # _width = s
-00011100: 656c 662e 7369 7a65 2829 2e77 6964 7468  elf.size().width
-00011110: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00011120: 2020 2020 2020 2023 2023 205f 6865 6967         # # _heig
-00011130: 6874 203d 2073 656c 662e 7369 7a65 2829  ht = self.size()
-00011140: 2e68 6569 6768 7428 290a 2020 2020 2020  .height().      
-00011150: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00011160: 2320 5f78 203d 2073 656c 662e 706f 7328  # _x = self.pos(
-00011170: 292e 7828 290a 2020 2020 2020 2020 2020  ).x().          
-00011180: 2020 2020 2020 2020 2020 2320 2320 5f79            # # _y
-00011190: 203d 2073 656c 662e 706f 7328 292e 7928   = self.pos().y(
-000111a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000111b0: 2020 2020 2020 2320 2320 7072 696e 7428        # # print(
-000111c0: 6622 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  f"**************
-000111d0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2078  ************** x
-000111e0: 207b 5f78 7d20 7920 7b5f 797d 2229 0a20   {_x} y {_y}"). 
-000111f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011200: 2020 2023 2023 2077 696e 646f 772e 6869     # # window.hi
-00011210: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
-00011220: 2020 2020 2020 2020 2023 2023 2077 696e           # # win
-00011230: 646f 772e 7368 6f77 2829 0a20 2020 2020  dow.show().     
-00011240: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00011250: 2023 2077 696e 646f 772e 7365 7447 656f   # window.setGeo
-00011260: 6d65 7472 7928 302c 2030 2c20 5f77 6964  metry(0, 0, _wid
-00011270: 7468 2c20 5f68 6569 6768 7429 0a20 2020  th, _height).   
-00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011290: 2023 2077 696e 646f 772e 7368 6f77 2829   # window.show()
-000112a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000112b0: 2020 2020 2023 2077 696e 646f 772e 6765       # window.ge
-000112c0: 6f6d 6574 7279 2829 2e73 6574 5828 3130  ometry().setX(10
-000112d0: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
-000112e0: 2020 2020 2020 2023 2077 696e 646f 772e         # window.
-000112f0: 6765 6f6d 6574 7279 2829 2e73 6574 5928  geometry().setY(
-00011300: 3130 3029 0a0a 2020 2020 6465 6620 6377  100)..    def cw
-00011310: 5f6d 6163 726f 735f 7374 6174 655f 6368  _macros_state_ch
-00011320: 616e 6765 6428 7365 6c66 293a 0a20 2020  anged(self):.   
-00011330: 2020 2020 2022 2222 4d65 6e75 2069 7465       """Menu ite
-00011340: 6d20 746f 2073 686f 772f 6869 6465 206d  m to show/hide m
-00011350: 6163 726f 2062 7574 746f 6e73 2222 220a  acro buttons""".
-00011360: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-00011370: 665b 2263 775f 6d61 6372 6f73 225d 203d  f["cw_macros"] =
-00011380: 2073 656c 662e 6163 7469 6f6e 4357 5f4d   self.actionCW_M
-00011390: 6163 726f 732e 6973 4368 6563 6b65 6428  acros.isChecked(
-000113a0: 290a 2020 2020 2020 2020 7365 6c66 2e77  ).        self.w
-000113b0: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
-000113c0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-000113d0: 686f 775f 4357 5f6d 6163 726f 7328 290a  how_CW_macros().
-000113e0: 0a20 2020 2064 6566 2073 686f 775f 4357  .    def show_CW
-000113f0: 5f6d 6163 726f 7328 7365 6c66 293a 0a20  _macros(self):. 
-00011400: 2020 2020 2020 2022 2222 6d61 6372 6f20         """macro 
-00011410: 6275 7474 6f6e 2073 7461 7465 2063 6861  button state cha
-00011420: 6e67 6522 2222 0a20 2020 2020 2020 2069  nge""".        i
-00011430: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
-00011440: 2263 775f 6d61 6372 6f73 2229 3a0a 2020  "cw_macros"):.  
-00011450: 2020 2020 2020 2020 2020 7365 6c66 2e42            self.B
-00011460: 7574 746f 6e5f 526f 7731 2e73 686f 7728  utton_Row1.show(
-00011470: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00011480: 6c66 2e42 7574 746f 6e5f 526f 7732 2e73  lf.Button_Row2.s
-00011490: 686f 7728 290a 2020 2020 2020 2020 656c  how().        el
-000114a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000114b0: 7365 6c66 2e42 7574 746f 6e5f 526f 7731  self.Button_Row1
-000114c0: 2e68 6964 6528 290a 2020 2020 2020 2020  .hide().        
-000114d0: 2020 2020 7365 6c66 2e42 7574 746f 6e5f      self.Button_
-000114e0: 526f 7732 2e68 6964 6528 290a 0a20 2020  Row2.hide()..   
-000114f0: 2064 6566 2063 6f6d 6d61 6e64 5f62 7574   def command_but
-00011500: 746f 6e73 5f73 7461 7465 5f63 6861 6e67  tons_state_chang
-00011510: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00011520: 2022 2222 4d65 6e75 2069 7465 6d20 746f   """Menu item to
-00011530: 2073 686f 772f 6869 6465 2063 6f6d 6d61   show/hide comma
-00011540: 6e64 2062 7574 746f 6e73 2222 220a 2020  nd buttons""".  
-00011550: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
-00011560: 2263 6f6d 6d61 6e64 5f62 7574 746f 6e73  "command_buttons
-00011570: 225d 203d 2073 656c 662e 6163 7469 6f6e  "] = self.action
-00011580: 436f 6d6d 616e 645f 4275 7474 6f6e 732e  Command_Buttons.
-00011590: 6973 4368 6563 6b65 6428 290a 2020 2020  isChecked().    
-000115a0: 2020 2020 7365 6c66 2e77 7269 7465 5f70      self.write_p
-000115b0: 7265 6665 7265 6e63 6528 290a 2020 2020  reference().    
-000115c0: 2020 2020 7365 6c66 2e73 686f 775f 636f      self.show_co
-000115d0: 6d6d 616e 645f 6275 7474 6f6e 7328 290a  mmand_buttons().
-000115e0: 0a20 2020 2064 6566 2073 686f 775f 636f  .    def show_co
-000115f0: 6d6d 616e 645f 6275 7474 6f6e 7328 7365  mmand_buttons(se
-00011600: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00011610: 636f 6d6d 616e 6420 6275 7474 6f6e 2073  command button s
-00011620: 7461 7465 2063 6861 6e67 6522 2222 0a20  tate change""". 
-00011630: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00011640: 7265 662e 6765 7428 2263 6f6d 6d61 6e64  ref.get("command
-00011650: 5f62 7574 746f 6e73 2229 3a0a 2020 2020  _buttons"):.    
-00011660: 2020 2020 2020 2020 7365 6c66 2e43 6f6d          self.Com
-00011670: 6d61 6e64 5f42 7574 746f 6e73 2e73 686f  mand_Buttons.sho
-00011680: 7728 290a 2020 2020 2020 2020 656c 7365  w().        else
-00011690: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000116a0: 6c66 2e43 6f6d 6d61 6e64 5f42 7574 746f  lf.Command_Butto
-000116b0: 6e73 2e68 6964 6528 290a 0a20 2020 2064  ns.hide()..    d
-000116c0: 6566 2069 735f 666c 6f61 7461 626c 6528  ef is_floatable(
-000116d0: 7365 6c66 2c20 6974 656d 3a20 7374 7229  self, item: str)
-000116e0: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-000116f0: 2020 2222 2263 6865 636b 2074 6f20 7365    """check to se
-00011700: 6520 6966 2073 7472 696e 6720 6361 6e20  e if string can 
-00011710: 6265 2061 2066 6c6f 6174 2222 220a 2020  be a float""".  
-00011720: 2020 2020 2020 6966 2069 7465 6d2e 6973        if item.is
-00011730: 6e75 6d65 7269 6328 293a 0a20 2020 2020  numeric():.     
-00011740: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00011750: 7565 0a20 2020 2020 2020 2074 7279 3a0a  ue.        try:.
-00011760: 2020 2020 2020 2020 2020 2020 5f74 6573              _tes
-00011770: 7420 3d20 666c 6f61 7428 6974 656d 290a  t = float(item).
-00011780: 2020 2020 2020 2020 6578 6365 7074 2056          except V
-00011790: 616c 7565 4572 726f 723a 0a20 2020 2020  alueError:.     
-000117a0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000117b0: 6c73 650a 2020 2020 2020 2020 7265 7475  lse.        retu
-000117c0: 726e 2054 7275 650a 0a20 2020 2064 6566  rn True..    def
-000117d0: 206f 7468 6572 5f32 5f63 6861 6e67 6564   other_2_changed
-000117e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000117f0: 2222 2243 616c 6c65 6420 7768 656e 2077  """Called when w
-00011800: 6520 6e65 6564 2074 6f20 7061 7273 6520  e need to parse 
-00011810: 5353 2065 7863 6861 6e67 652e 2222 220a  SS exchange.""".
-00011820: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00011830: 636f 6e74 6573 743a 0a20 2020 2020 2020  contest:.       
-00011840: 2020 2020 2069 6620 2241 5252 4c20 5377       if "ARRL Sw
-00011850: 6565 7073 7461 6b65 7322 2069 6e20 7365  eepstakes" in se
-00011860: 6c66 2e63 6f6e 7465 7374 2e6e 616d 653a  lf.contest.name:
-00011870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011880: 2073 656c 662e 636f 6e74 6573 742e 7061   self.contest.pa
-00011890: 7273 655f 6578 6368 616e 6765 2873 656c  rse_exchange(sel
-000118a0: 6629 0a0a 2020 2020 6465 6620 6361 6c6c  f)..    def call
-000118b0: 7369 676e 5f63 6861 6e67 6564 2873 656c  sign_changed(sel
-000118c0: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
-000118d0: 616c 6c65 6420 7768 656e 2074 6578 7420  alled when text 
-000118e0: 696e 2074 6865 2063 616c 6c73 6967 6e20  in the callsign 
-000118f0: 6669 656c 6420 6861 7320 6368 616e 6765  field has change
-00011900: 6422 2222 0a20 2020 2020 2020 2074 6578  d""".        tex
-00011910: 7420 3d20 7365 6c66 2e63 616c 6c73 6967  t = self.callsig
-00011920: 6e2e 7465 7874 2829 0a20 2020 2020 2020  n.text().       
-00011930: 2074 6578 7420 3d20 7465 7874 2e75 7070   text = text.upp
-00011940: 6572 2829 0a20 2020 2020 2020 2070 6f73  er().        pos
-00011950: 6974 696f 6e20 3d20 7365 6c66 2e63 616c  ition = self.cal
-00011960: 6c73 6967 6e2e 6375 7273 6f72 506f 7369  lsign.cursorPosi
-00011970: 7469 6f6e 2829 0a20 2020 2020 2020 2073  tion().        s
-00011980: 7472 6970 7065 645f 7465 7874 203d 2074  tripped_text = t
-00011990: 6578 742e 7374 7269 7028 292e 7265 706c  ext.strip().repl
-000119a0: 6163 6528 2220 222c 2022 2229 0a20 2020  ace(" ", "").   
-000119b0: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
-000119c0: 676e 2e73 6574 5465 7874 2873 7472 6970  gn.setText(strip
-000119d0: 7065 645f 7465 7874 290a 2020 2020 2020  ped_text).      
-000119e0: 2020 7365 6c66 2e63 616c 6c73 6967 6e2e    self.callsign.
-000119f0: 7365 7443 7572 736f 7250 6f73 6974 696f  setCursorPositio
-00011a00: 6e28 706f 7369 7469 6f6e 290a 0a20 2020  n(position)..   
-00011a10: 2020 2020 2069 6620 2220 2220 696e 2074       if " " in t
-00011a20: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
-00011a30: 2069 6620 7374 7269 7070 6564 5f74 6578   if stripped_tex
-00011a40: 7420 3d3d 2022 4357 223a 0a20 2020 2020  t == "CW":.     
-00011a50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011a60: 7365 746d 6f64 6528 2243 5722 290a 2020  setmode("CW").  
-00011a70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011a80: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
-00011a90: 6d6f 6465 225d 203d 2022 4357 220a 2020  mode"] = "CW".  
-00011aa0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011ab0: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
-00011ac0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
-00011ad0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-00011ae0: 6967 5f63 6f6e 7472 6f6c 2e6f 6e6c 696e  ig_control.onlin
-00011af0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00011b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011b10: 7269 675f 636f 6e74 726f 6c2e 7365 745f  rig_control.set_
-00011b20: 6d6f 6465 2822 4357 2229 0a20 2020 2020  mode("CW").     
-00011b30: 2020 2020 2020 2020 2020 2062 616e 6420             band 
-00011b40: 3d20 6765 7462 616e 6428 7374 7228 7365  = getband(str(se
-00011b50: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-00011b60: 6574 2822 7666 6f61 222c 2022 302e 3022  et("vfoa", "0.0"
-00011b70: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-00011b80: 2020 2020 7365 6c66 2e73 6574 5f62 616e      self.set_ban
-00011b90: 645f 696e 6469 6361 746f 7228 6261 6e64  d_indicator(band
-00011ba0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011bb0: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
-00011bc0: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
-00011bd0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00011be0: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
-00011bf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011c00: 662e 7265 6164 5f63 775f 6d61 6372 6f73  f.read_cw_macros
-00011c10: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00011c20: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00011c30: 2020 2020 2020 6966 2073 7472 6970 7065        if strippe
-00011c40: 645f 7465 7874 203d 3d20 2252 5454 5922  d_text == "RTTY"
-00011c50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011c60: 2020 7365 6c66 2e73 6574 6d6f 6465 2822    self.setmode("
-00011c70: 5254 5459 2229 0a20 2020 2020 2020 2020  RTTY").         
-00011c80: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-00011c90: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
-00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-00011cc0: 726f 6c2e 6f6e 6c69 6e65 3a0a 2020 2020  rol.online:.    
-00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ce0: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
-00011cf0: 7472 6f6c 2e73 6574 5f6d 6f64 6528 2252  trol.set_mode("R
-00011d00: 5454 5922 290a 2020 2020 2020 2020 2020  TTY").          
-00011d10: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d30: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-00011d40: 696f 5f73 7461 7465 5b22 6d6f 6465 225d  io_state["mode"]
-00011d50: 203d 2022 5254 5459 220a 2020 2020 2020   = "RTTY".      
-00011d60: 2020 2020 2020 2020 2020 6261 6e64 203d            band =
-00011d70: 2067 6574 6261 6e64 2873 7472 2873 656c   getband(str(sel
-00011d80: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-00011d90: 7428 2276 666f 6122 2c20 2230 2e30 2229  t("vfoa", "0.0")
-00011da0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00011db0: 2020 2073 656c 662e 7365 745f 6261 6e64     self.set_band
-00011dc0: 5f69 6e64 6963 6174 6f72 2862 616e 6429  _indicator(band)
-00011dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011de0: 2073 656c 662e 7365 745f 7769 6e64 6f77   self.set_window
-00011df0: 5f74 6974 6c65 2829 0a20 2020 2020 2020  _title().       
-00011e00: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-00011e10: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
-00011e20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00011e30: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
-00011e40: 6620 7374 7269 7070 6564 5f74 6578 7420  f stripped_text 
-00011e50: 3d3d 2022 5353 4222 3a0a 2020 2020 2020  == "SSB":.      
-00011e60: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00011e70: 6574 6d6f 6465 2822 5353 4222 290a 2020  etmode("SSB").  
-00011e80: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011e90: 2069 6e74 2873 656c 662e 7261 6469 6f5f   int(self.radio_
-00011ea0: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
-00011eb0: 2c20 3029 2920 3e20 3130 3030 3030 3030  , 0)) > 10000000
-00011ec0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011ed0: 2020 2020 2020 7365 6c66 2e72 6164 696f        self.radio
-00011ee0: 5f73 7461 7465 5b22 6d6f 6465 225d 203d  _state["mode"] =
-00011ef0: 2022 5553 4222 0a20 2020 2020 2020 2020   "USB".         
-00011f00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00011f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f20: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-00011f30: 655b 226d 6f64 6522 5d20 3d20 224c 5342  e["mode"] = "LSB
-00011f40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00011f50: 2020 6261 6e64 203d 2067 6574 6261 6e64    band = getband
-00011f60: 2873 7472 2873 656c 662e 7261 6469 6f5f  (str(self.radio_
-00011f70: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
-00011f80: 2c20 2230 2e30 2229 2929 0a20 2020 2020  , "0.0"))).     
-00011f90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011fa0: 7365 745f 6261 6e64 5f69 6e64 6963 6174  set_band_indicat
-00011fb0: 6f72 2862 616e 6429 0a20 2020 2020 2020  or(band).       
-00011fc0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00011fd0: 745f 7769 6e64 6f77 5f74 6974 6c65 2829  t_window_title()
-00011fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011ff0: 2069 6620 7365 6c66 2e72 6967 5f63 6f6e   if self.rig_con
-00012000: 7472 6f6c 3a0a 2020 2020 2020 2020 2020  trol:.          
-00012010: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00012020: 6967 5f63 6f6e 7472 6f6c 2e73 6574 5f6d  ig_control.set_m
-00012030: 6f64 6528 7365 6c66 2e72 6164 696f 5f73  ode(self.radio_s
-00012040: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-00012050: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012060: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
-00012070: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
-00012080: 2020 2020 2073 656c 662e 7265 6164 5f63       self.read_c
-00012090: 775f 6d61 6372 6f73 2829 0a20 2020 2020  w_macros().     
-000120a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000120b0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
-000120c0: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
-000120d0: 3d20 224f 504f 4e22 3a0a 2020 2020 2020  = "OPON":.      
-000120e0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-000120f0: 6574 5f6f 706f 6e28 290a 2020 2020 2020  et_opon().      
-00012100: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00012110: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
-00012120: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00012130: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-00012140: 6966 2073 7472 6970 7065 645f 7465 7874  if stripped_text
-00012150: 203d 3d20 2254 4553 5422 3a0a 2020 2020   == "TEST":.    
-00012160: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012170: 2e73 686f 775f 6d65 7373 6167 655f 626f  .show_message_bo
-00012180: 7828 2254 6869 7320 6973 2061 2074 6573  x("This is a tes
-00012190: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
-000121a0: 2020 2020 7365 6c66 2e63 6c65 6172 696e      self.clearin
-000121b0: 7075 7473 2829 0a20 2020 2020 2020 2020  puts().         
-000121c0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-000121d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000121e0: 662e 6973 5f66 6c6f 6174 6162 6c65 2873  f.is_floatable(s
-000121f0: 7472 6970 7065 645f 7465 7874 293a 0a20  tripped_text):. 
-00012200: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00012210: 666f 203d 2066 6c6f 6174 2873 7472 6970  fo = float(strip
-00012220: 7065 645f 7465 7874 290a 2020 2020 2020  ped_text).      
-00012230: 2020 2020 2020 2020 2020 7666 6f20 3d20            vfo = 
-00012240: 696e 7428 7666 6f20 2a20 3130 3030 290a  int(vfo * 1000).
-00012250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012260: 6261 6e64 203d 2067 6574 6261 6e64 2873  band = getband(s
-00012270: 7472 2876 666f 2929 0a20 2020 2020 2020  tr(vfo)).       
-00012280: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00012290: 745f 6261 6e64 5f69 6e64 6963 6174 6f72  t_band_indicator
-000122a0: 2862 616e 6429 0a20 2020 2020 2020 2020  (band).         
-000122b0: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-000122c0: 6e74 6163 745b 2242 616e 6422 5d20 3d20  ntact["Band"] = 
-000122d0: 6765 745f 6c6f 6767 6564 5f62 616e 6428  get_logged_band(
-000122e0: 7374 7228 7365 6c66 2e72 6164 696f 5f73  str(self.radio_s
-000122f0: 7461 7465 2e67 6574 2822 7666 6f61 222c  tate.get("vfoa",
-00012300: 2030 2e30 2929 290a 2020 2020 2020 2020   0.0))).        
-00012310: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-00012320: 696f 5f73 7461 7465 5b22 7666 6f61 225d  io_state["vfoa"]
-00012330: 203d 2076 666f 0a20 2020 2020 2020 2020   = vfo.         
-00012340: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
-00012350: 7769 6e64 6f77 5f74 6974 6c65 2829 0a20  window_title(). 
-00012360: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012370: 656c 662e 636c 6561 7269 6e70 7574 7328  elf.clearinputs(
-00012380: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012390: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
-000123a0: 6e74 726f 6c3a 0a20 2020 2020 2020 2020  ntrol:.         
-000123b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000123c0: 7269 675f 636f 6e74 726f 6c2e 7365 745f  rig_control.set_
-000123d0: 7666 6f28 7666 6f29 0a20 2020 2020 2020  vfo(vfo).       
-000123e0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000123f0: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-00012400: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
-00012410: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-00012420: 5b22 636d 6422 5d20 3d20 2252 4144 494f  ["cmd"] = "RADIO
-00012430: 5f53 5441 5445 220a 2020 2020 2020 2020  _STATE".        
-00012440: 2020 2020 2020 2020 636d 645b 2273 7461          cmd["sta
-00012450: 7469 6f6e 225d 203d 2070 6c61 7466 6f72  tion"] = platfor
-00012460: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
-00012470: 2020 2020 2020 2020 2063 6d64 5b22 6261           cmd["ba
-00012480: 6e64 225d 203d 2062 616e 640a 2020 2020  nd"] = band.    
-00012490: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-000124a0: 2276 666f 6122 5d20 3d20 7666 6f0a 2020  "vfoa"] = vfo.  
-000124b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000124c0: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-000124d0: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
-000124e0: 736f 6e28 636d 6429 0a20 2020 2020 2020  son(cmd).       
-000124f0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00012500: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012510: 662e 6368 6563 6b5f 6361 6c6c 7369 676e  f.check_callsign
-00012520: 2873 7472 6970 7065 645f 7465 7874 290a  (stripped_text).
-00012530: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00012540: 656c 662e 6368 6563 6b5f 6475 7065 2873  elf.check_dupe(s
-00012550: 7472 6970 7065 645f 7465 7874 293a 0a20  tripped_text):. 
-00012560: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012570: 656c 662e 6475 7065 5f69 6e64 6963 6174  elf.dupe_indicat
-00012580: 6f72 2e73 686f 7728 290a 2020 2020 2020  or.show().      
-00012590: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000125a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000125b0: 2e64 7570 655f 696e 6469 6361 746f 722e  .dupe_indicator.
-000125c0: 6869 6465 2829 0a20 2020 2020 2020 2020  hide().         
-000125d0: 2020 205f 7468 6574 6872 6561 6420 3d20     _thethread = 
-000125e0: 7468 7265 6164 696e 672e 5468 7265 6164  threading.Thread
-000125f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00012600: 2020 7461 7267 6574 3d73 656c 662e 6368    target=self.ch
-00012610: 6563 6b5f 6361 6c6c 7369 676e 322c 0a20  eck_callsign2,. 
-00012620: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00012630: 7267 733d 2874 6578 742c 292c 0a20 2020  rgs=(text,),.   
-00012640: 2020 2020 2020 2020 2020 2020 2064 6165               dae
-00012650: 6d6f 6e3d 5472 7565 2c0a 2020 2020 2020  mon=True,.      
-00012660: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00012670: 2020 2020 5f74 6865 7468 7265 6164 2e73      _thethread.s
-00012680: 7461 7274 2829 0a20 2020 2020 2020 2020  tart().         
-00012690: 2020 2073 656c 662e 6e65 7874 5f66 6965     self.next_fie
-000126a0: 6c64 2e73 6574 466f 6375 7328 290a 2020  ld.setFocus().  
-000126b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000126c0: 0a20 2020 2020 2020 2063 6d64 203d 207b  .        cmd = {
-000126d0: 7d0a 2020 2020 2020 2020 636d 645b 2263  }.        cmd["c
-000126e0: 6d64 225d 203d 2022 4341 4c4c 4348 414e  md"] = "CALLCHAN
-000126f0: 4745 4422 0a20 2020 2020 2020 2063 6d64  GED".        cmd
-00012700: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
-00012710: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
-00012720: 2020 2020 2020 636d 645b 2263 616c 6c22        cmd["call"
-00012730: 5d20 3d20 7374 7269 7070 6564 5f74 6578  ] = stripped_tex
-00012740: 740a 2020 2020 2020 2020 7365 6c66 2e6d  t.        self.m
-00012750: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
-00012760: 6365 2e73 656e 645f 6173 5f6a 736f 6e28  ce.send_as_json(
-00012770: 636d 6429 0a20 2020 2020 2020 2073 656c  cmd).        sel
-00012780: 662e 6368 6563 6b5f 6361 6c6c 7369 676e  f.check_callsign
-00012790: 2873 7472 6970 7065 645f 7465 7874 290a  (stripped_text).
-000127a0: 0a20 2020 2064 6566 2063 6865 636b 5f63  .    def check_c
-000127b0: 616c 6c73 6967 6e28 7365 6c66 2c20 6361  allsign(self, ca
-000127c0: 6c6c 7369 676e 293a 0a20 2020 2020 2020  llsign):.       
-000127d0: 2022 2222 4368 6563 6b20 6361 6c6c 2061   """Check call a
-000127e0: 7320 656e 7465 7265 6422 2222 0a20 2020  s entered""".   
-000127f0: 2020 2020 2072 6573 756c 7420 3d20 6374       result = ct
-00012800: 795f 6c6f 6f6b 7570 2863 616c 6c73 6967  y_lookup(callsig
-00012810: 6e29 0a20 2020 2020 2020 2064 6562 7567  n).        debug
-00012820: 5f72 6573 756c 7420 3d20 6622 7b72 6573  _result = f"{res
-00012830: 756c 747d 220a 2020 2020 2020 2020 6c6f  ult}".        lo
-00012840: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
-00012850: 2064 6562 7567 5f72 6573 756c 7429 0a20   debug_result). 
-00012860: 2020 2020 2020 2069 6620 7265 7375 6c74         if result
-00012870: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-00012880: 7220 6120 696e 2072 6573 756c 742e 6974  r a in result.it
-00012890: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-000128a0: 2020 2020 2020 2065 6e74 6974 7920 3d20         entity = 
-000128b0: 615b 315d 2e67 6574 2822 656e 7469 7479  a[1].get("entity
-000128c0: 222c 2022 2229 0a20 2020 2020 2020 2020  ", "").         
-000128d0: 2020 2020 2020 2063 7120 3d20 615b 315d         cq = a[1]
-000128e0: 2e67 6574 2822 6371 222c 2022 2229 0a20  .get("cq", ""). 
-000128f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012900: 7475 203d 2061 5b31 5d2e 6765 7428 2269  tu = a[1].get("i
-00012910: 7475 222c 2022 2229 0a20 2020 2020 2020  tu", "").       
-00012920: 2020 2020 2020 2020 2063 6f6e 7469 6e65           contine
-00012930: 6e74 203d 2061 5b31 5d2e 6765 7428 2263  nt = a[1].get("c
-00012940: 6f6e 7469 6e65 6e74 2229 0a20 2020 2020  ontinent").     
-00012950: 2020 2020 2020 2020 2020 206c 6174 203d             lat =
-00012960: 2066 6c6f 6174 2861 5b31 5d2e 6765 7428   float(a[1].get(
-00012970: 226c 6174 222c 2022 302e 3022 2929 0a20  "lat", "0.0")). 
-00012980: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00012990: 6f6e 203d 2066 6c6f 6174 2861 5b31 5d2e  on = float(a[1].
-000129a0: 6765 7428 226c 6f6e 6722 2c20 2230 2e30  get("long", "0.0
-000129b0: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
-000129c0: 2020 2020 6c6f 6e20 3d20 6c6f 6e20 2a20      lon = lon * 
-000129d0: 2d31 2020 2320 6374 792e 6461 7420 6669  -1  # cty.dat fi
-000129e0: 6c65 2069 6e76 6572 7473 206c 6f6e 6769  le inverts longi
-000129f0: 7475 6465 730a 2020 2020 2020 2020 2020  tudes.          
-00012a00: 2020 2020 2020 7072 696d 6172 795f 7066        primary_pf
-00012a10: 7820 3d20 615b 315d 2e67 6574 2822 7072  x = a[1].get("pr
-00012a20: 696d 6172 795f 7066 7822 2c20 2222 290a  imary_pfx", "").
-00012a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a40: 6865 6164 696e 6720 3d20 6265 6172 696e  heading = bearin
-00012a50: 675f 7769 7468 5f6c 6174 6c6f 6e28 7365  g_with_latlon(se
-00012a60: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-00012a70: 4772 6964 5371 7561 7265 2229 2c20 6c61  GridSquare"), la
-00012a80: 742c 206c 6f6e 290a 2020 2020 2020 2020  t, lon).        
-00012a90: 2020 2020 2020 2020 6b69 6c6f 6d65 7465          kilomete
-00012aa0: 7273 203d 2064 6973 7461 6e63 655f 7769  rs = distance_wi
-00012ab0: 7468 5f6c 6174 6c6f 6e28 0a20 2020 2020  th_latlon(.     
-00012ac0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012ad0: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-00012ae0: 2247 7269 6453 7175 6172 6522 292c 206c  "GridSquare"), l
-00012af0: 6174 2c20 6c6f 6e0a 2020 2020 2020 2020  at, lon.        
-00012b00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00012b10: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-00012b20: 6561 6469 6e67 5f64 6973 7461 6e63 652e  eading_distance.
-00012b30: 7365 7454 6578 7428 0a20 2020 2020 2020  setText(.       
-00012b40: 2020 2020 2020 2020 2020 2020 2066 2252               f"R
-00012b50: 6567 696f 6e61 6c20 4864 6720 7b68 6561  egional Hdg {hea
-00012b60: 6469 6e67 7dc2 b020 4c50 207b 7265 6369  ding}.. LP {reci
-00012b70: 7072 6f63 6f6c 2868 6561 6469 6e67 297d  procol(heading)}
-00012b80: c2b0 202f 2022 0a20 2020 2020 2020 2020  .. / ".         
-00012b90: 2020 2020 2020 2020 2020 2066 2264 6973             f"dis
-00012ba0: 7461 6e63 6520 7b69 6e74 286b 696c 6f6d  tance {int(kilom
-00012bb0: 6574 6572 732a 302e 3632 3133 3731 297d  eters*0.621371)}
-00012bc0: 6d69 207b 6b69 6c6f 6d65 7465 7273 7d6b  mi {kilometers}k
-00012bd0: 6d22 0a20 2020 2020 2020 2020 2020 2020  m".             
-00012be0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00012bf0: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-00012c00: 745b 2243 6f75 6e74 7279 5072 6566 6978  t["CountryPrefix
-00012c10: 225d 203d 2070 7269 6d61 7279 5f70 6678  "] = primary_pfx
-00012c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012c30: 2073 656c 662e 636f 6e74 6163 745b 225a   self.contact["Z
-00012c40: 4e22 5d20 3d20 696e 7428 6371 290a 2020  N"] = int(cq).  
-00012c50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012c60: 6c66 2e63 6f6e 7461 6374 5b22 436f 6e74  lf.contact["Cont
-00012c70: 696e 656e 7422 5d20 3d20 636f 6e74 696e  inent"] = contin
-00012c80: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
-00012c90: 2020 2020 7365 6c66 2e64 785f 656e 7469      self.dx_enti
-00012ca0: 7479 2e73 6574 5465 7874 280a 2020 2020  ty.setText(.    
-00012cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cc0: 6622 7b70 7269 6d61 7279 5f70 6678 7d3a  f"{primary_pfx}:
-00012cd0: 207b 636f 6e74 696e 656e 747d 2f7b 656e   {continent}/{en
-00012ce0: 7469 7479 7d20 6371 3a7b 6371 7d20 6974  tity} cq:{cq} it
-00012cf0: 753a 7b69 7475 7d22 0a20 2020 2020 2020  u:{itu}".       
-00012d00: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00012d10: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00012d20: 6e28 6361 6c6c 7369 676e 2920 3e20 323a  n(callsign) > 2:
-00012d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012d40: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-00012d50: 7465 7374 3a0a 2020 2020 2020 2020 2020  test:.          
-00012d60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012d70: 6c66 2e63 6f6e 7465 7374 2e70 7265 6669  lf.contest.prefi
-00012d80: 6c6c 2873 656c 6629 0a0a 2020 2020 6465  ll(self)..    de
-00012d90: 6620 6368 6563 6b5f 6361 6c6c 7369 676e  f check_callsign
-00012da0: 3228 7365 6c66 2c20 6361 6c6c 7369 676e  2(self, callsign
-00012db0: 293a 0a20 2020 2020 2020 2022 2222 4368  ):.        """Ch
-00012dc0: 6563 6b20 6361 6c6c 206f 6e63 6520 656e  eck call once en
-00012dd0: 7465 7265 6422 2222 0a20 2020 2020 2020  tered""".       
-00012de0: 2063 616c 6c73 6967 6e20 3d20 6361 6c6c   callsign = call
-00012df0: 7369 676e 2e73 7472 6970 2829 0a20 2020  sign.strip().   
-00012e00: 2020 2020 2064 6562 7567 5f6c 6f6f 6b75       debug_looku
-00012e10: 7020 3d20 6622 7b73 656c 662e 6c6f 6f6b  p = f"{self.look
-00012e20: 5f75 707d 220a 2020 2020 2020 2020 6c6f  _up}".        lo
-00012e30: 6767 6572 2e64 6562 7567 2822 2573 2c20  gger.debug("%s, 
-00012e40: 2573 222c 2063 616c 6c73 6967 6e2c 2064  %s", callsign, d
-00012e50: 6562 7567 5f6c 6f6f 6b75 7029 0a20 2020  ebug_lookup).   
-00012e60: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-00012e70: 7365 6c66 2e6c 6f6f 6b5f 7570 2c20 2273  self.look_up, "s
-00012e80: 6573 7369 6f6e 2229 3a0a 2020 2020 2020  ession"):.      
-00012e90: 2020 2020 2020 6966 2073 656c 662e 6c6f        if self.lo
-00012ea0: 6f6b 5f75 702e 7365 7373 696f 6e3a 0a20  ok_up.session:. 
-00012eb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00012ec0: 6573 706f 6e73 6520 3d20 7365 6c66 2e6c  esponse = self.l
-00012ed0: 6f6f 6b5f 7570 2e6c 6f6f 6b75 7028 6361  ook_up.lookup(ca
-00012ee0: 6c6c 7369 676e 290a 2020 2020 2020 2020  llsign).        
-00012ef0: 2020 2020 2020 2020 6465 6275 675f 7265          debug_re
-00012f00: 7370 6f6e 7365 203d 2066 227b 7265 7370  sponse = f"{resp
-00012f10: 6f6e 7365 7d22 0a20 2020 2020 2020 2020  onse}".         
-00012f20: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00012f30: 6275 6728 2254 6865 2052 6573 706f 6e73  bug("The Respons
-00012f40: 653a 2025 735c 6e22 2c20 6465 6275 675f  e: %s\n", debug_
-00012f50: 7265 7370 6f6e 7365 290a 2020 2020 2020  response).      
-00012f60: 2020 2020 2020 2020 2020 6966 2072 6573            if res
-00012f70: 706f 6e73 653a 0a20 2020 2020 2020 2020  ponse:.         
-00012f80: 2020 2020 2020 2020 2020 2074 6865 6972             their
-00012f90: 6772 6964 203d 2072 6573 706f 6e73 652e  grid = response.
-00012fa0: 6765 7428 2267 7269 6422 290a 2020 2020  get("grid").    
-00012fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fc0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4772  self.contact["Gr
-00012fd0: 6964 5371 7561 7265 225d 203d 2074 6865  idSquare"] = the
-00012fe0: 6972 6772 6964 0a20 2020 2020 2020 2020  irgrid.         
-00012ff0: 2020 2020 2020 2020 2020 205f 7468 6569             _thei
-00013000: 7263 6f75 6e74 7279 203d 2072 6573 706f  rcountry = respo
-00013010: 6e73 652e 6765 7428 2263 6f75 6e74 7279  nse.get("country
-00013020: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00013030: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00013040: 7461 7469 6f6e 2e67 6574 2822 4772 6964  tation.get("Grid
-00013050: 5371 7561 7265 222c 2022 2229 3a0a 2020  Square", ""):.  
-00013060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013070: 2020 2020 2020 6865 6164 696e 6720 3d20        heading = 
-00013080: 6265 6172 696e 6728 7365 6c66 2e73 7461  bearing(self.sta
-00013090: 7469 6f6e 2e67 6574 2822 4772 6964 5371  tion.get("GridSq
-000130a0: 7561 7265 222c 2022 2229 2c20 7468 6569  uare", ""), thei
-000130b0: 7267 7269 6429 0a20 2020 2020 2020 2020  rgrid).         
-000130c0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-000130d0: 696c 6f6d 6574 6572 7320 3d20 6469 7374  ilometers = dist
-000130e0: 616e 6365 2873 656c 662e 7374 6174 696f  ance(self.statio
-000130f0: 6e2e 6765 7428 2247 7269 6453 7175 6172  n.get("GridSquar
-00013100: 6522 292c 2074 6865 6972 6772 6964 290a  e"), theirgrid).
-00013110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013120: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-00013130: 6469 6e67 5f64 6973 7461 6e63 652e 7365  ding_distance.se
-00013140: 7454 6578 7428 0a20 2020 2020 2020 2020  tText(.         
-00013150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013160: 2020 2066 227b 7468 6569 7267 7269 647d     f"{theirgrid}
-00013170: 2048 6467 207b 6865 6164 696e 677d c2b0   Hdg {heading}..
-00013180: 204c 5020 7b72 6563 6970 726f 636f 6c28   LP {reciprocol(
-00013190: 6865 6164 696e 6729 7dc2 b020 2f20 220a  heading)}.. / ".
-000131a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131b0: 2020 2020 2020 2020 2020 2020 6622 6469              f"di
-000131c0: 7374 616e 6365 207b 696e 7428 6b69 6c6f  stance {int(kilo
-000131d0: 6d65 7465 7273 2a30 2e36 3231 3337 3129  meters*0.621371)
-000131e0: 7d6d 6920 7b6b 696c 6f6d 6574 6572 737d  }mi {kilometers}
-000131f0: 6b6d 220a 2020 2020 2020 2020 2020 2020  km".            
-00013200: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013220: 2020 2320 7365 6c66 2e64 785f 656e 7469    # self.dx_enti
-00013230: 7479 2e73 6574 5465 7874 2866 227b 7468  ty.setText(f"{th
-00013240: 6569 7263 6f75 6e74 7279 7d22 290a 2020  eircountry}").  
-00013250: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00013260: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00013270: 2020 2020 2020 2320 7365 6c66 2e68 6561        # self.hea
-00013280: 6469 6e67 5f64 6973 7461 6e63 652e 7365  ding_distance.se
-00013290: 7454 6578 7428 224c 6f6f 6b75 7020 6661  tText("Lookup fa
-000132a0: 696c 6564 2e22 290a 0a20 2020 2064 6566  iled.")..    def
-000132b0: 2063 6865 636b 5f64 7570 6528 7365 6c66   check_dupe(self
-000132c0: 2c20 6361 6c6c 3a20 7374 7229 202d 3e20  , call: str) -> 
-000132d0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-000132e0: 2243 6865 636b 7320 6966 2061 2063 616c  "Checks if a cal
-000132f0: 6c73 6967 6e20 6973 2061 2064 7570 6520  lsign is a dupe 
-00013300: 6f6e 2063 7572 7265 6e74 2062 616e 642f  on current band/
-00013310: 6d6f 6465 2e22 2222 0a20 2020 2020 2020  mode.""".       
-00013320: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
-00013330: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00013340: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
-00013350: 6d65 7373 6167 655f 626f 7828 2259 6f75  message_box("You
-00013360: 2068 6176 6520 6e6f 2063 6f6e 7465 7374   have no contest
-00013370: 206c 6f61 6465 642e 2229 0a20 2020 2020   loaded.").     
-00013380: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00013390: 6c73 650a 2020 2020 2020 2020 7365 6c66  lse.        self
-000133a0: 2e63 6f6e 7465 7374 2e70 7265 6475 7065  .contest.predupe
-000133b0: 2873 656c 6629 0a20 2020 2020 2020 2062  (self).        b
-000133c0: 616e 6420 3d20 666c 6f61 7428 6765 745f  and = float(get_
-000133d0: 6c6f 6767 6564 5f62 616e 6428 7374 7228  logged_band(str(
-000133e0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-000133f0: 2e67 6574 2822 7666 6f61 222c 2030 2e30  .get("vfoa", 0.0
-00013400: 2929 2929 0a20 2020 2020 2020 206d 6f64  )))).        mod
-00013410: 6520 3d20 7365 6c66 2e72 6164 696f 5f73  e = self.radio_s
-00013420: 7461 7465 2e67 6574 2822 6d6f 6465 222c  tate.get("mode",
-00013430: 2022 2229 0a20 2020 2020 2020 2064 6562   "").        deb
-00013440: 7567 6c69 6e65 203d 2028 0a20 2020 2020  ugline = (.     
-00013450: 2020 2020 2020 2066 2243 616c 6c3a 207b         f"Call: {
-00013460: 6361 6c6c 7d20 4261 6e64 3a20 7b62 616e  call} Band: {ban
-00013470: 647d 204d 6f64 653a 207b 6d6f 6465 7d20  d} Mode: {mode} 
-00013480: 4475 7065 7479 7065 3a20 7b73 656c 662e  Dupetype: {self.
-00013490: 636f 6e74 6573 742e 6475 7065 5f74 7970  contest.dupe_typ
-000134a0: 657d 220a 2020 2020 2020 2020 290a 2020  e}".        ).  
-000134b0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-000134c0: 7567 2822 2573 222c 2064 6562 7567 6c69  ug("%s", debugli
-000134d0: 6e65 290a 2020 2020 2020 2020 6966 2073  ne).        if s
-000134e0: 656c 662e 636f 6e74 6573 742e 6475 7065  elf.contest.dupe
-000134f0: 5f74 7970 6520 3d3d 2031 3a0a 2020 2020  _type == 1:.    
-00013500: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00013510: 2073 656c 662e 6461 7461 6261 7365 2e63   self.database.c
-00013520: 6865 636b 5f64 7570 6528 6361 6c6c 290a  heck_dupe(call).
-00013530: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00013540: 636f 6e74 6573 742e 6475 7065 5f74 7970  contest.dupe_typ
-00013550: 6520 3d3d 2032 3a0a 2020 2020 2020 2020  e == 2:.        
-00013560: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-00013570: 662e 6461 7461 6261 7365 2e63 6865 636b  f.database.check
-00013580: 5f64 7570 655f 6f6e 5f62 616e 6428 6361  _dupe_on_band(ca
-00013590: 6c6c 2c20 6261 6e64 290a 2020 2020 2020  ll, band).      
-000135a0: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
-000135b0: 742e 6475 7065 5f74 7970 6520 3d3d 2033  t.dupe_type == 3
-000135c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000135d0: 7375 6c74 203d 2073 656c 662e 6461 7461  sult = self.data
-000135e0: 6261 7365 2e63 6865 636b 5f64 7570 655f  base.check_dupe_
-000135f0: 6f6e 5f62 616e 645f 6d6f 6465 2863 616c  on_band_mode(cal
-00013600: 6c2c 2062 616e 642c 206d 6f64 6529 0a20  l, band, mode). 
-00013610: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00013620: 6f6e 7465 7374 2e64 7570 655f 7479 7065  ontest.dupe_type
-00013630: 203d 3d20 343a 0a20 2020 2020 2020 2020   == 4:.         
-00013640: 2020 2072 6573 756c 7420 3d20 7b22 6973     result = {"is
-00013650: 6475 7065 223a 2046 616c 7365 7d0a 2020  dupe": False}.  
-00013660: 2020 2020 2020 6465 6275 676c 696e 6520        debugline 
-00013670: 3d20 6622 7b72 6573 756c 747d 220a 2020  = f"{result}".  
-00013680: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00013690: 7567 2822 2573 222c 2064 6562 7567 6c69  ug("%s", debugli
-000136a0: 6e65 290a 2020 2020 2020 2020 7265 7475  ne).        retu
-000136b0: 726e 2072 6573 756c 742e 6765 7428 2269  rn result.get("i
-000136c0: 7364 7570 6522 2c20 4661 6c73 6529 0a0a  sdupe", False)..
-000136d0: 2020 2020 6465 6620 7365 746d 6f64 6528      def setmode(
-000136e0: 7365 6c66 2c20 6d6f 6465 3a20 7374 7229  self, mode: str)
-000136f0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00013700: 2020 2222 2273 7475 6220 666f 7220 7768    """stub for wh
-00013710: 656e 2074 6865 206d 6f64 6520 6368 616e  en the mode chan
-00013720: 6765 732e 2222 220a 2020 2020 2020 2020  ges.""".        
-00013730: 6966 206d 6f64 6520 3d3d 2022 4357 223a  if mode == "CW":
-00013740: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00013750: 662e 6375 7272 656e 745f 6d6f 6465 203d  f.current_mode =
-00013760: 2022 4357 220a 2020 2020 2020 2020 2020   "CW".          
-00013770: 2020 2320 7365 6c66 2e6d 6f64 652e 7365    # self.mode.se
-00013780: 7454 6578 7428 2243 5722 290a 2020 2020  tText("CW").    
-00013790: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-000137a0: 742e 7365 7454 6578 7428 2235 3939 2229  t.setText("599")
-000137b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000137c0: 662e 7265 6365 6976 652e 7365 7454 6578  f.receive.setTex
-000137d0: 7428 2235 3939 2229 0a20 2020 2020 2020  t("599").       
-000137e0: 2020 2020 2073 656c 662e 7265 6164 5f63       self.read_c
-000137f0: 775f 6d61 6372 6f73 2829 0a20 2020 2020  w_macros().     
-00013800: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00013810: 2020 2020 2020 6966 206d 6f64 6520 3d3d        if mode ==
-00013820: 2022 5353 4222 3a0a 2020 2020 2020 2020   "SSB":.        
-00013830: 2020 2020 7365 6c66 2e63 7572 7265 6e74      self.current
-00013840: 5f6d 6f64 6520 3d20 2253 5342 220a 2020  _mode = "SSB".  
-00013850: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-00013860: 2e6d 6f64 652e 7365 7454 6578 7428 2253  .mode.setText("S
-00013870: 5342 2229 0a20 2020 2020 2020 2020 2020  SB").           
-00013880: 2073 656c 662e 7365 6e74 2e73 6574 5465   self.sent.setTe
-00013890: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
-000138a0: 2020 2020 2073 656c 662e 7265 6365 6976       self.receiv
-000138b0: 652e 7365 7454 6578 7428 2235 3922 290a  e.setText("59").
-000138c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000138d0: 2e72 6561 645f 6377 5f6d 6163 726f 7328  .read_cw_macros(
-000138e0: 290a 2020 2020 2020 2020 6966 206d 6f64  ).        if mod
-000138f0: 6520 3d3d 2022 5254 5459 223a 0a20 2020  e == "RTTY":.   
-00013900: 2020 2020 2020 2020 2073 656c 662e 6375           self.cu
-00013910: 7272 656e 745f 6d6f 6465 203d 2022 5254  rrent_mode = "RT
-00013920: 5459 220a 2020 2020 2020 2020 2020 2020  TY".            
-00013930: 2320 7365 6c66 2e6d 6f64 652e 7365 7454  # self.mode.setT
-00013940: 6578 7428 2252 5454 5922 290a 2020 2020  ext("RTTY").    
-00013950: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00013960: 742e 7365 7454 6578 7428 2235 3922 290a  t.setText("59").
-00013970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013980: 2e72 6563 6569 7665 2e73 6574 5465 7874  .receive.setText
-00013990: 2822 3539 2229 0a0a 2020 2020 6465 6620  ("59")..    def 
-000139a0: 6765 745f 6f70 6f6e 2873 656c 6629 3a0a  get_opon(self):.
-000139b0: 2020 2020 2020 2020 2222 2243 7472 6c2b          """Ctrl+
-000139c0: 4f20 6f72 204f 504f 4e20 6469 616c 6f67  O or OPON dialog
-000139d0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-000139e0: 2e6f 706f 6e5f 6469 616c 6f67 203d 204f  .opon_dialog = O
-000139f0: 704f 6e28 574f 524b 494e 475f 5041 5448  pOn(WORKING_PATH
-00013a00: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
-00013a10: 706f 6e5f 6469 616c 6f67 2e61 6363 6570  pon_dialog.accep
-00013a20: 7465 642e 636f 6e6e 6563 7428 7365 6c66  ted.connect(self
-00013a30: 2e6e 6577 5f6f 7029 0a20 2020 2020 2020  .new_op).       
-00013a40: 2073 656c 662e 6f70 6f6e 5f64 6961 6c6f   self.opon_dialo
-00013a50: 672e 6f70 656e 2829 0a0a 2020 2020 6465  g.open()..    de
-00013a60: 6620 6e65 775f 6f70 2873 656c 6629 3a0a  f new_op(self):.
-00013a70: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
-00013a80: 6e65 7720 4f50 2222 220a 2020 2020 2020  new OP""".      
-00013a90: 2020 6966 2073 656c 662e 6f70 6f6e 5f64    if self.opon_d
-00013aa0: 6961 6c6f 672e 4e65 774f 7065 7261 746f  ialog.NewOperato
-00013ab0: 722e 7465 7874 2829 3a0a 2020 2020 2020  r.text():.      
-00013ac0: 2020 2020 2020 7365 6c66 2e63 7572 7265        self.curre
-00013ad0: 6e74 5f6f 7020 3d20 7365 6c66 2e6f 706f  nt_op = self.opo
-00013ae0: 6e5f 6469 616c 6f67 2e4e 6577 4f70 6572  n_dialog.NewOper
-00013af0: 6174 6f72 2e74 6578 7428 292e 7570 7065  ator.text().uppe
-00013b00: 7228 290a 2020 2020 2020 2020 7365 6c66  r().        self
-00013b10: 2e6f 706f 6e5f 6469 616c 6f67 2e63 6c6f  .opon_dialog.clo
-00013b20: 7365 2829 0a20 2020 2020 2020 206c 6f67  se().        log
-00013b30: 6765 722e 6465 6275 6728 224e 6577 204f  ger.debug("New O
-00013b40: 703a 2025 7322 2c20 7365 6c66 2e63 7572  p: %s", self.cur
-00013b50: 7265 6e74 5f6f 7029 0a20 2020 2020 2020  rent_op).       
-00013b60: 2073 656c 662e 6d61 6b65 5f6f 705f 6469   self.make_op_di
-00013b70: 7228 290a 0a20 2020 2064 6566 206d 616b  r()..    def mak
-00013b80: 655f 6f70 5f64 6972 2873 656c 6629 3a0a  e_op_dir(self):.
-00013b90: 2020 2020 2020 2020 2222 2243 7265 6174          """Creat
-00013ba0: 6520 4f50 2064 6972 6563 746f 7279 2069  e OP directory i
-00013bb0: 6620 6974 2064 6f65 7320 6e6f 7420 6578  f it does not ex
-00013bc0: 6973 742e 2222 220a 2020 2020 2020 2020  ist.""".        
-00013bd0: 6966 2073 656c 662e 6375 7272 656e 745f  if self.current_
-00013be0: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
-00013bf0: 6f70 5f70 6174 6820 3d20 5061 7468 2844  op_path = Path(D
-00013c00: 4154 415f 5041 5448 2920 2f20 7365 6c66  ATA_PATH) / self
-00013c10: 2e63 7572 7265 6e74 5f6f 700a 2020 2020  .current_op.    
-00013c20: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00013c30: 6562 7567 2822 6f70 5f70 6174 683a 2025  ebug("op_path: %
-00013c40: 7322 2c20 7374 7228 6f70 5f70 6174 6829  s", str(op_path)
-00013c50: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00013c60: 206f 705f 7061 7468 2e69 735f 6469 7228   op_path.is_dir(
-00013c70: 2920 6973 2046 616c 7365 3a0a 2020 2020  ) is False:.    
-00013c80: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00013c90: 6572 2e64 6562 7567 2822 4372 6561 7469  er.debug("Creati
-00013ca0: 6e67 204f 7020 4469 7265 6374 6f72 793a  ng Op Directory:
-00013cb0: 2025 7322 2c20 7374 7228 6f70 5f70 6174   %s", str(op_pat
-00013cc0: 6829 290a 2020 2020 2020 2020 2020 2020  h)).            
-00013cd0: 2020 2020 6f73 2e6d 6b64 6972 2873 7472      os.mkdir(str
-00013ce0: 286f 705f 7061 7468 2929 0a20 2020 2020  (op_path)).     
-00013cf0: 2020 2020 2020 2069 6620 6f70 5f70 6174         if op_pat
-00013d00: 682e 6973 5f64 6972 2829 3a0a 2020 2020  h.is_dir():.    
-00013d10: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-00013d20: 6365 5f70 6174 6820 3d20 5061 7468 2857  ce_path = Path(W
-00013d30: 4f52 4b49 4e47 5f50 4154 4829 202f 2022  ORKING_PATH) / "
-00013d40: 6461 7461 2220 2f20 2270 686f 6e65 7469  data" / "phoneti
-00013d50: 6373 220a 2020 2020 2020 2020 2020 2020  cs".            
-00013d60: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00013d70: 2822 736f 7572 6365 5f70 6174 683a 2025  ("source_path: %
-00013d80: 7322 2c20 7374 7228 736f 7572 6365 5f70  s", str(source_p
-00013d90: 6174 6829 290a 2020 2020 2020 2020 2020  ath)).          
-00013da0: 2020 2020 2020 666f 7220 6368 696c 6420        for child 
-00013db0: 696e 2073 6f75 7263 655f 7061 7468 2e69  in source_path.i
-00013dc0: 7465 7264 6972 2829 3a0a 2020 2020 2020  terdir():.      
-00013dd0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00013de0: 7374 696e 6174 696f 6e5f 6669 6c65 203d  stination_file =
-00013df0: 206f 705f 7061 7468 202f 2063 6869 6c64   op_path / child
-00013e00: 2e6e 616d 650a 2020 2020 2020 2020 2020  .name.          
-00013e10: 2020 2020 2020 2020 2020 6966 2064 6573            if des
-00013e20: 7469 6e61 7469 6f6e 5f66 696c 652e 6973  tination_file.is
-00013e30: 5f66 696c 6528 2920 6973 2046 616c 7365  _file() is False
-00013e40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013e50: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00013e60: 2e64 6562 7567 2822 4465 7374 696e 6174  .debug("Destinat
-00013e70: 696f 6e3a 2025 7322 2c20 7374 7228 6465  ion: %s", str(de
-00013e80: 7374 696e 6174 696f 6e5f 6669 6c65 2929  stination_file))
-00013e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ea0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-00013eb0: 7469 6f6e 5f66 696c 652e 7772 6974 655f  tion_file.write_
-00013ec0: 6279 7465 7328 6368 696c 642e 7265 6164  bytes(child.read
-00013ed0: 5f62 7974 6573 2829 290a 0a20 2020 2064  _bytes())..    d
-00013ee0: 6566 2070 6f6c 6c5f 7261 6469 6f28 7365  ef poll_radio(se
-00013ef0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00013f00: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
-00013f10: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-00013f20: 726f 6c3a 0a20 2020 2020 2020 2020 2020  rol:.           
-00013f30: 2069 6620 7365 6c66 2e72 6967 5f63 6f6e   if self.rig_con
-00013f40: 7472 6f6c 2e6f 6e6c 696e 6520 6973 2046  trol.online is F
-00013f50: 616c 7365 3a0a 2020 2020 2020 2020 2020  alse:.          
-00013f60: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
-00013f70: 6f6e 7472 6f6c 2e72 6569 6e69 7428 290a  ontrol.reinit().
-00013f80: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00013f90: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
-00013fa0: 6f6e 6c69 6e65 3a0a 2020 2020 2020 2020  online:.        
-00013fb0: 2020 2020 2020 2020 696e 666f 5f64 6972          info_dir
-00013fc0: 7479 203d 2046 616c 7365 0a20 2020 2020  ty = False.     
-00013fd0: 2020 2020 2020 2020 2020 2076 666f 203d             vfo =
-00013fe0: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
-00013ff0: 6c2e 6765 745f 7666 6f28 290a 2020 2020  l.get_vfo().    
-00014000: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00014010: 203d 2073 656c 662e 7269 675f 636f 6e74   = self.rig_cont
-00014020: 726f 6c2e 6765 745f 6d6f 6465 2829 0a20  rol.get_mode(). 
-00014030: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00014040: 7720 3d20 7365 6c66 2e72 6967 5f63 6f6e  w = self.rig_con
-00014050: 7472 6f6c 2e67 6574 5f62 7728 290a 2020  trol.get_bw().  
-00014060: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00014070: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00014080: 5b22 7074 7422 5d20 3d20 7365 6c66 2e72  ["ptt"] = self.r
-00014090: 6967 5f63 6f6e 7472 6f6c 2e67 6574 5f70  ig_control.get_p
-000140a0: 7474 2829 0a0a 2020 2020 2020 2020 2020  tt()..          
-000140b0: 2020 2020 2020 6966 206d 6f64 6520 3d3d        if mode ==
-000140c0: 2022 4357 223a 0a20 2020 2020 2020 2020   "CW":.         
-000140d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000140e0: 7365 746d 6f64 6528 6d6f 6465 290a 2020  setmode(mode).  
-000140f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014100: 206d 6f64 6520 3d3d 2022 4c53 4222 206f   mode == "LSB" o
-00014110: 7220 6d6f 6465 203d 3d20 2255 5342 223a  r mode == "USB":
-00014120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014130: 2020 2020 2073 656c 662e 7365 746d 6f64       self.setmod
-00014140: 6528 2253 5342 2229 0a20 2020 2020 2020  e("SSB").       
-00014150: 2020 2020 2020 2020 2069 6620 6d6f 6465           if mode
-00014160: 203d 3d20 2252 5454 5922 3a0a 2020 2020   == "RTTY":.    
-00014170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014180: 7365 6c66 2e73 6574 6d6f 6465 2822 5254  self.setmode("RT
-00014190: 5459 2229 0a0a 2020 2020 2020 2020 2020  TY")..          
-000141a0: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
-000141b0: 6469 6f5f 7374 6174 652e 6765 7428 2276  dio_state.get("v
-000141c0: 666f 6122 2920 213d 2076 666f 3a0a 2020  foa") != vfo:.  
-000141d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141e0: 2020 696e 666f 5f64 6972 7479 203d 2054    info_dirty = T
-000141f0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00014200: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-00014210: 696f 5f73 7461 7465 5b22 7666 6f61 225d  io_state["vfoa"]
-00014220: 203d 2076 666f 0a20 2020 2020 2020 2020   = vfo.         
-00014230: 2020 2020 2020 2062 616e 6420 3d20 6765         band = ge
-00014240: 7462 616e 6428 7374 7228 7666 6f29 290a  tband(str(vfo)).
+00010d70: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
+00010d80: 7461 7465 5b22 7666 6f61 225d 203d 2069  tate["vfoa"] = i
+00010d90: 6e74 2876 666f 290a 2020 2020 2020 2020  nt(vfo).        
+00010da0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00010db0: 656c 662e 7269 675f 636f 6e74 726f 6c3a  elf.rig_control:
+00010dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010dd0: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
+00010de0: 675f 636f 6e74 726f 6c2e 7365 745f 7666  g_control.set_vf
+00010df0: 6f28 696e 7428 7666 6f29 290a 2020 2020  o(int(vfo)).    
+00010e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e10: 7370 6f74 203d 206a 736f 6e5f 6461 7461  spot = json_data
+00010e20: 2e67 6574 2822 7370 6f74 222c 2022 2229  .get("spot", "")
+00010e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010e40: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+00010e50: 676e 2e73 6574 5465 7874 2873 706f 7429  gn.setText(spot)
+00010e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010e70: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+00010e80: 676e 5f63 6861 6e67 6564 2829 0a20 2020  gn_changed().   
+00010e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ea0: 2073 656c 662e 6361 6c6c 7369 676e 2e73   self.callsign.s
+00010eb0: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
+00010ec0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010ed0: 6c66 2e63 616c 6c73 6967 6e2e 6163 7469  lf.callsign.acti
+00010ee0: 7661 7465 5769 6e64 6f77 2829 0a20 2020  vateWindow().   
+00010ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f00: 2077 696e 646f 772e 7261 6973 655f 2829   window.raise_()
+00010f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f20: 2020 2020 2023 2066 6720 3d20 7769 6e64       # fg = wind
+00010f30: 6f77 2e66 7261 6d65 4765 6f6d 6574 7279  ow.frameGeometry
+00010f40: 2829 2e74 6f70 4c65 6674 0a20 2020 2020  ().topLeft.     
+00010f50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00010f60: 2023 205f 7769 6474 6820 3d20 7365 6c66   # _width = self
+00010f70: 2e73 697a 6528 292e 7769 6474 6828 290a  .size().width().
+00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f90: 2020 2020 2320 2320 5f68 6569 6768 7420      # # _height 
+00010fa0: 3d20 7365 6c66 2e73 697a 6528 292e 6865  = self.size().he
+00010fb0: 6967 6874 2829 0a20 2020 2020 2020 2020  ight().         
+00010fc0: 2020 2020 2020 2020 2020 2023 2023 205f             # # _
+00010fd0: 7820 3d20 7365 6c66 2e70 6f73 2829 2e78  x = self.pos().x
+00010fe0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00010ff0: 2020 2020 2020 2023 2023 205f 7920 3d20         # # _y = 
+00011000: 7365 6c66 2e70 6f73 2829 2e79 2829 0a20  self.pos().y(). 
+00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011020: 2020 2023 2023 2070 7269 6e74 2866 222a     # # print(f"*
+00011030: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00011040: 2a2a 2a2a 2a2a 2a2a 2a2a 2a20 7820 7b5f  *********** x {_
+00011050: 787d 2079 207b 5f79 7d22 290a 2020 2020  x} y {_y}").    
+00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011070: 2320 2320 7769 6e64 6f77 2e68 6964 6528  # # window.hide(
+00011080: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011090: 2020 2020 2020 2320 2320 7769 6e64 6f77        # # window
+000110a0: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
+000110b0: 2020 2020 2020 2020 2020 2020 2320 2320              # # 
+000110c0: 7769 6e64 6f77 2e73 6574 4765 6f6d 6574  window.setGeomet
+000110d0: 7279 2830 2c20 302c 205f 7769 6474 682c  ry(0, 0, _width,
+000110e0: 205f 6865 6967 6874 290a 2020 2020 2020   _height).      
+000110f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00011100: 7769 6e64 6f77 2e73 686f 7728 290a 2020  window.show().  
+00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011120: 2020 2320 7769 6e64 6f77 2e67 656f 6d65    # window.geome
+00011130: 7472 7928 292e 7365 7458 2831 3030 290a  try().setX(100).
+00011140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011150: 2020 2020 2320 7769 6e64 6f77 2e67 656f      # window.geo
+00011160: 6d65 7472 7928 292e 7365 7459 2831 3030  metry().setY(100
+00011170: 290a 0a20 2020 2064 6566 2063 775f 6d61  )..    def cw_ma
+00011180: 6372 6f73 5f73 7461 7465 5f63 6861 6e67  cros_state_chang
+00011190: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
+000111a0: 2020 2222 224d 656e 7520 6974 656d 2074    """Menu item t
+000111b0: 6f20 7368 6f77 2f68 6964 6520 6d61 6372  o show/hide macr
+000111c0: 6f20 6275 7474 6f6e 7322 2222 0a20 2020  o buttons""".   
+000111d0: 2020 2020 2073 656c 662e 7072 6566 5b22       self.pref["
+000111e0: 6377 5f6d 6163 726f 7322 5d20 3d20 7365  cw_macros"] = se
+000111f0: 6c66 2e61 6374 696f 6e43 575f 4d61 6372  lf.actionCW_Macr
+00011200: 6f73 2e69 7343 6865 636b 6564 2829 0a20  os.isChecked(). 
+00011210: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
+00011220: 655f 7072 6566 6572 656e 6365 2829 0a20  e_preference(). 
+00011230: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
+00011240: 5f43 575f 6d61 6372 6f73 2829 0a0a 2020  _CW_macros()..  
+00011250: 2020 6465 6620 7368 6f77 5f43 575f 6d61    def show_CW_ma
+00011260: 6372 6f73 2873 656c 6629 3a0a 2020 2020  cros(self):.    
+00011270: 2020 2020 2222 226d 6163 726f 2062 7574      """macro but
+00011280: 746f 6e20 7374 6174 6520 6368 616e 6765  ton state change
+00011290: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+000112a0: 656c 662e 7072 6566 2e67 6574 2822 6377  elf.pref.get("cw
+000112b0: 5f6d 6163 726f 7322 293a 0a20 2020 2020  _macros"):.     
+000112c0: 2020 2020 2020 2073 656c 662e 4275 7474         self.Butt
+000112d0: 6f6e 5f52 6f77 312e 7368 6f77 2829 0a20  on_Row1.show(). 
+000112e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000112f0: 4275 7474 6f6e 5f52 6f77 322e 7368 6f77  Button_Row2.show
+00011300: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
+00011310: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00011320: 662e 4275 7474 6f6e 5f52 6f77 312e 6869  f.Button_Row1.hi
+00011330: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00011340: 2073 656c 662e 4275 7474 6f6e 5f52 6f77   self.Button_Row
+00011350: 322e 6869 6465 2829 0a0a 2020 2020 6465  2.hide()..    de
+00011360: 6620 636f 6d6d 616e 645f 6275 7474 6f6e  f command_button
+00011370: 735f 7374 6174 655f 6368 616e 6765 2873  s_state_change(s
+00011380: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00011390: 224d 656e 7520 6974 656d 2074 6f20 7368  "Menu item to sh
+000113a0: 6f77 2f68 6964 6520 636f 6d6d 616e 6420  ow/hide command 
+000113b0: 6275 7474 6f6e 7322 2222 0a20 2020 2020  buttons""".     
+000113c0: 2020 2073 656c 662e 7072 6566 5b22 636f     self.pref["co
+000113d0: 6d6d 616e 645f 6275 7474 6f6e 7322 5d20  mmand_buttons"] 
+000113e0: 3d20 7365 6c66 2e61 6374 696f 6e43 6f6d  = self.actionCom
+000113f0: 6d61 6e64 5f42 7574 746f 6e73 2e69 7343  mand_Buttons.isC
+00011400: 6865 636b 6564 2829 0a20 2020 2020 2020  hecked().       
+00011410: 2073 656c 662e 7772 6974 655f 7072 6566   self.write_pref
+00011420: 6572 656e 6365 2829 0a20 2020 2020 2020  erence().       
+00011430: 2073 656c 662e 7368 6f77 5f63 6f6d 6d61   self.show_comma
+00011440: 6e64 5f62 7574 746f 6e73 2829 0a0a 2020  nd_buttons()..  
+00011450: 2020 6465 6620 7368 6f77 5f63 6f6d 6d61    def show_comma
+00011460: 6e64 5f62 7574 746f 6e73 2873 656c 6629  nd_buttons(self)
+00011470: 3a0a 2020 2020 2020 2020 2222 2263 6f6d  :.        """com
+00011480: 6d61 6e64 2062 7574 746f 6e20 7374 6174  mand button stat
+00011490: 6520 6368 616e 6765 2222 220a 2020 2020  e change""".    
+000114a0: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
+000114b0: 2e67 6574 2822 636f 6d6d 616e 645f 6275  .get("command_bu
+000114c0: 7474 6f6e 7322 293a 0a20 2020 2020 2020  ttons"):.       
+000114d0: 2020 2020 2073 656c 662e 436f 6d6d 616e       self.Comman
+000114e0: 645f 4275 7474 6f6e 732e 7368 6f77 2829  d_Buttons.show()
+000114f0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00011500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011510: 436f 6d6d 616e 645f 4275 7474 6f6e 732e  Command_Buttons.
+00011520: 6869 6465 2829 0a0a 2020 2020 6465 6620  hide()..    def 
+00011530: 6973 5f66 6c6f 6174 6162 6c65 2873 656c  is_floatable(sel
+00011540: 662c 2069 7465 6d3a 2073 7472 2920 2d3e  f, item: str) ->
+00011550: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00011560: 2222 6368 6563 6b20 746f 2073 6565 2069  ""check to see i
+00011570: 6620 7374 7269 6e67 2063 616e 2062 6520  f string can be 
+00011580: 6120 666c 6f61 7422 2222 0a20 2020 2020  a float""".     
+00011590: 2020 2069 6620 6974 656d 2e69 736e 756d     if item.isnum
+000115a0: 6572 6963 2829 3a0a 2020 2020 2020 2020  eric():.        
+000115b0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+000115c0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000115d0: 2020 2020 2020 2020 205f 7465 7374 203d           _test =
+000115e0: 2066 6c6f 6174 2869 7465 6d29 0a20 2020   float(item).   
+000115f0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
+00011600: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+00011610: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00011620: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011630: 5472 7565 0a0a 2020 2020 6465 6620 6f74  True..    def ot
+00011640: 6865 725f 325f 6368 616e 6765 6428 7365  her_2_changed(se
+00011650: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00011660: 4361 6c6c 6564 2077 6865 6e20 7765 206e  Called when we n
+00011670: 6565 6420 746f 2070 6172 7365 2053 5320  eed to parse SS 
+00011680: 6578 6368 616e 6765 2e22 2222 0a20 2020  exchange.""".   
+00011690: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+000116a0: 7465 7374 3a0a 2020 2020 2020 2020 2020  test:.          
+000116b0: 2020 6966 2022 4152 524c 2053 7765 6570    if "ARRL Sweep
+000116c0: 7374 616b 6573 2220 696e 2073 656c 662e  stakes" in self.
+000116d0: 636f 6e74 6573 742e 6e61 6d65 3a0a 2020  contest.name:.  
+000116e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000116f0: 6c66 2e63 6f6e 7465 7374 2e70 6172 7365  lf.contest.parse
+00011700: 5f65 7863 6861 6e67 6528 7365 6c66 290a  _exchange(self).
+00011710: 0a20 2020 2064 6566 2063 616c 6c73 6967  .    def callsig
+00011720: 6e5f 6368 616e 6765 6428 7365 6c66 293a  n_changed(self):
+00011730: 0a20 2020 2020 2020 2022 2222 4361 6c6c  .        """Call
+00011740: 6564 2077 6865 6e20 7465 7874 2069 6e20  ed when text in 
+00011750: 7468 6520 6361 6c6c 7369 676e 2066 6965  the callsign fie
+00011760: 6c64 2068 6173 2063 6861 6e67 6564 2222  ld has changed""
+00011770: 220a 2020 2020 2020 2020 7465 7874 203d  ".        text =
+00011780: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
+00011790: 6578 7428 290a 2020 2020 2020 2020 7465  ext().        te
+000117a0: 7874 203d 2074 6578 742e 7570 7065 7228  xt = text.upper(
+000117b0: 290a 2020 2020 2020 2020 706f 7369 7469  ).        positi
+000117c0: 6f6e 203d 2073 656c 662e 6361 6c6c 7369  on = self.callsi
+000117d0: 676e 2e63 7572 736f 7250 6f73 6974 696f  gn.cursorPositio
+000117e0: 6e28 290a 2020 2020 2020 2020 7374 7269  n().        stri
+000117f0: 7070 6564 5f74 6578 7420 3d20 7465 7874  pped_text = text
+00011800: 2e73 7472 6970 2829 2e72 6570 6c61 6365  .strip().replace
+00011810: 2822 2022 2c20 2222 290a 2020 2020 2020  (" ", "").      
+00011820: 2020 7365 6c66 2e63 616c 6c73 6967 6e2e    self.callsign.
+00011830: 7365 7454 6578 7428 7374 7269 7070 6564  setText(stripped
+00011840: 5f74 6578 7429 0a20 2020 2020 2020 2073  _text).        s
+00011850: 656c 662e 6361 6c6c 7369 676e 2e73 6574  elf.callsign.set
+00011860: 4375 7273 6f72 506f 7369 7469 6f6e 2870  CursorPosition(p
+00011870: 6f73 6974 696f 6e29 0a0a 2020 2020 2020  osition)..      
+00011880: 2020 6966 2022 2022 2069 6e20 7465 7874    if " " in text
+00011890: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000118a0: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
+000118b0: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+000118c0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+000118d0: 6d6f 6465 2822 4357 2229 0a20 2020 2020  mode("CW").     
+000118e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000118f0: 7261 6469 6f5f 7374 6174 655b 226d 6f64  radio_state["mod
+00011900: 6522 5d20 3d20 2243 5722 0a20 2020 2020  e"] = "CW".     
+00011910: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00011920: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 3a0a  lf.rig_control:.
+00011930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011940: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
+00011950: 636f 6e74 726f 6c2e 6f6e 6c69 6e65 3a0a  control.online:.
+00011960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011970: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
+00011980: 5f63 6f6e 7472 6f6c 2e73 6574 5f6d 6f64  _control.set_mod
+00011990: 6528 2243 5722 290a 2020 2020 2020 2020  e("CW").        
+000119a0: 2020 2020 2020 2020 6261 6e64 203d 2067          band = g
+000119b0: 6574 6261 6e64 2873 7472 2873 656c 662e  etband(str(self.
+000119c0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+000119d0: 2276 666f 6122 2c20 2230 2e30 2229 2929  "vfoa", "0.0")))
+000119e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000119f0: 2073 656c 662e 7365 745f 6261 6e64 5f69   self.set_band_i
+00011a00: 6e64 6963 6174 6f72 2862 616e 6429 0a20  ndicator(band). 
+00011a10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011a20: 656c 662e 7365 745f 7769 6e64 6f77 5f74  elf.set_window_t
+00011a30: 6974 6c65 2829 0a20 2020 2020 2020 2020  itle().         
+00011a40: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+00011a50: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
+00011a60: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00011a70: 6561 645f 6377 5f6d 6163 726f 7328 290a  ead_cw_macros().
+00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a90: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00011aa0: 2020 2069 6620 7374 7269 7070 6564 5f74     if stripped_t
+00011ab0: 6578 7420 3d3d 2022 5254 5459 223a 0a20  ext == "RTTY":. 
+00011ac0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011ad0: 656c 662e 7365 746d 6f64 6528 2252 5454  elf.setmode("RTT
+00011ae0: 5922 290a 2020 2020 2020 2020 2020 2020  Y").            
+00011af0: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
+00011b00: 636f 6e74 726f 6c3a 0a20 2020 2020 2020  control:.       
+00011b10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011b20: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+00011b30: 2e6f 6e6c 696e 653a 0a20 2020 2020 2020  .online:.       
+00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b50: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+00011b60: 6c2e 7365 745f 6d6f 6465 2822 5254 5459  l.set_mode("RTTY
+00011b70: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00011b80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ba0: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
+00011bb0: 7374 6174 655b 226d 6f64 6522 5d20 3d20  state["mode"] = 
+00011bc0: 2252 5454 5922 0a20 2020 2020 2020 2020  "RTTY".         
+00011bd0: 2020 2020 2020 2062 616e 6420 3d20 6765         band = ge
+00011be0: 7462 616e 6428 7374 7228 7365 6c66 2e72  tband(str(self.r
+00011bf0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+00011c00: 7666 6f61 222c 2022 302e 3022 2929 290a  vfoa", "0.0"))).
+00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c20: 7365 6c66 2e73 6574 5f62 616e 645f 696e  self.set_band_in
+00011c30: 6469 6361 746f 7228 6261 6e64 290a 2020  dicator(band).  
+00011c40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011c50: 6c66 2e73 6574 5f77 696e 646f 775f 7469  lf.set_window_ti
+00011c60: 746c 6528 290a 2020 2020 2020 2020 2020  tle().          
+00011c70: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
+00011c80: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
+00011c90: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00011ca0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00011cb0: 7472 6970 7065 645f 7465 7874 203d 3d20  tripped_text == 
+00011cc0: 2253 5342 223a 0a20 2020 2020 2020 2020  "SSB":.         
+00011cd0: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
+00011ce0: 6f64 6528 2253 5342 2229 0a20 2020 2020  ode("SSB").     
+00011cf0: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+00011d00: 7428 7365 6c66 2e72 6164 696f 5f73 7461  t(self.radio_sta
+00011d10: 7465 2e67 6574 2822 7666 6f61 222c 2030  te.get("vfoa", 0
+00011d20: 2929 203e 2031 3030 3030 3030 303a 0a20  )) > 10000000:. 
+00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d40: 2020 2073 656c 662e 7261 6469 6f5f 7374     self.radio_st
+00011d50: 6174 655b 226d 6f64 6522 5d20 3d20 2255  ate["mode"] = "U
+00011d60: 5342 220a 2020 2020 2020 2020 2020 2020  SB".            
+00011d70: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00011d80: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011d90: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
+00011da0: 6d6f 6465 225d 203d 2022 4c53 4222 0a20  mode"] = "LSB". 
+00011db0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00011dc0: 616e 6420 3d20 6765 7462 616e 6428 7374  and = getband(st
+00011dd0: 7228 7365 6c66 2e72 6164 696f 5f73 7461  r(self.radio_sta
+00011de0: 7465 2e67 6574 2822 7666 6f61 222c 2022  te.get("vfoa", "
+00011df0: 302e 3022 2929 290a 2020 2020 2020 2020  0.0"))).        
+00011e00: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00011e10: 5f62 616e 645f 696e 6469 6361 746f 7228  _band_indicator(
+00011e20: 6261 6e64 290a 2020 2020 2020 2020 2020  band).          
+00011e30: 2020 2020 2020 7365 6c66 2e73 6574 5f77        self.set_w
+00011e40: 696e 646f 775f 7469 746c 6528 290a 2020  indow_title().  
+00011e50: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011e60: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+00011e70: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+00011e80: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+00011e90: 636f 6e74 726f 6c2e 7365 745f 6d6f 6465  control.set_mode
+00011ea0: 2873 656c 662e 7261 6469 6f5f 7374 6174  (self.radio_stat
+00011eb0: 652e 6765 7428 226d 6f64 6522 2929 0a20  e.get("mode")). 
+00011ec0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011ed0: 656c 662e 636c 6561 7269 6e70 7574 7328  elf.clearinputs(
+00011ee0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011ef0: 2020 7365 6c66 2e72 6561 645f 6377 5f6d    self.read_cw_m
+00011f00: 6163 726f 7328 290a 2020 2020 2020 2020  acros().        
+00011f10: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00011f20: 2020 2020 2020 2020 2020 2069 6620 7374             if st
+00011f30: 7269 7070 6564 5f74 6578 7420 3d3d 2022  ripped_text == "
+00011f40: 4f50 4f4e 223a 0a20 2020 2020 2020 2020  OPON":.         
+00011f50: 2020 2020 2020 2073 656c 662e 6765 745f         self.get_
+00011f60: 6f70 6f6e 2829 0a20 2020 2020 2020 2020  opon().         
+00011f70: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+00011f80: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
+00011f90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011fa0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011fb0: 7374 7269 7070 6564 5f74 6578 7420 3d3d  stripped_text ==
+00011fc0: 2022 5445 5354 223a 0a20 2020 2020 2020   "TEST":.       
+00011fd0: 2020 2020 2020 2020 2073 656c 662e 7368           self.sh
+00011fe0: 6f77 5f6d 6573 7361 6765 5f62 6f78 2822  ow_message_box("
+00011ff0: 5468 6973 2069 7320 6120 7465 7374 2229  This is a test")
+00012000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012010: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
+00012020: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00012030: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00012040: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+00012050: 735f 666c 6f61 7461 626c 6528 7374 7269  s_floatable(stri
+00012060: 7070 6564 5f74 6578 7429 3a0a 2020 2020  pped_text):.    
+00012070: 2020 2020 2020 2020 2020 2020 7666 6f20              vfo 
+00012080: 3d20 666c 6f61 7428 7374 7269 7070 6564  = float(stripped
+00012090: 5f74 6578 7429 0a20 2020 2020 2020 2020  _text).         
+000120a0: 2020 2020 2020 2076 666f 203d 2069 6e74         vfo = int
+000120b0: 2876 666f 202a 2031 3030 3029 0a20 2020  (vfo * 1000).   
+000120c0: 2020 2020 2020 2020 2020 2020 2062 616e               ban
+000120d0: 6420 3d20 6765 7462 616e 6428 7374 7228  d = getband(str(
+000120e0: 7666 6f29 290a 2020 2020 2020 2020 2020  vfo)).          
+000120f0: 2020 2020 2020 7365 6c66 2e73 6574 5f62        self.set_b
+00012100: 616e 645f 696e 6469 6361 746f 7228 6261  and_indicator(ba
+00012110: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
+00012120: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+00012130: 6374 5b22 4261 6e64 225d 203d 2067 6574  ct["Band"] = get
+00012140: 5f6c 6f67 6765 645f 6261 6e64 2873 7472  _logged_band(str
+00012150: 2873 656c 662e 7261 6469 6f5f 7374 6174  (self.radio_stat
+00012160: 652e 6765 7428 2276 666f 6122 2c20 302e  e.get("vfoa", 0.
+00012170: 3029 2929 0a20 2020 2020 2020 2020 2020  0))).           
+00012180: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
+00012190: 7374 6174 655b 2276 666f 6122 5d20 3d20  state["vfoa"] = 
+000121a0: 7666 6f0a 2020 2020 2020 2020 2020 2020  vfo.            
+000121b0: 2020 2020 7365 6c66 2e73 6574 5f77 696e      self.set_win
+000121c0: 646f 775f 7469 746c 6528 290a 2020 2020  dow_title().    
+000121d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000121e0: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
+000121f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012200: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
+00012210: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
+00012220: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
+00012230: 5f63 6f6e 7472 6f6c 2e73 6574 5f76 666f  _control.set_vfo
+00012240: 2876 666f 290a 2020 2020 2020 2020 2020  (vfo).          
+00012250: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00012260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012270: 2063 6d64 203d 207b 7d0a 2020 2020 2020   cmd = {}.      
+00012280: 2020 2020 2020 2020 2020 636d 645b 2263            cmd["c
+00012290: 6d64 225d 203d 2022 5241 4449 4f5f 5354  md"] = "RADIO_ST
+000122a0: 4154 4522 0a20 2020 2020 2020 2020 2020  ATE".           
+000122b0: 2020 2020 2063 6d64 5b22 7374 6174 696f       cmd["statio
+000122c0: 6e22 5d20 3d20 706c 6174 666f 726d 2e6e  n"] = platform.n
+000122d0: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
+000122e0: 2020 2020 2020 636d 645b 2262 616e 6422        cmd["band"
+000122f0: 5d20 3d20 6261 6e64 0a20 2020 2020 2020  ] = band.       
+00012300: 2020 2020 2020 2020 2063 6d64 5b22 7666           cmd["vf
+00012310: 6f61 225d 203d 2076 666f 0a20 2020 2020  oa"] = vfo.     
+00012320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012330: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+00012340: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
+00012350: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
+00012360: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+00012370: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00012380: 6865 636b 5f63 616c 6c73 6967 6e28 7374  heck_callsign(st
+00012390: 7269 7070 6564 5f74 6578 7429 0a20 2020  ripped_text).   
+000123a0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000123b0: 2e63 6865 636b 5f64 7570 6528 7374 7269  .check_dupe(stri
+000123c0: 7070 6564 5f74 6578 7429 3a0a 2020 2020  pped_text):.    
+000123d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000123e0: 2e64 7570 655f 696e 6469 6361 746f 722e  .dupe_indicator.
+000123f0: 7368 6f77 2829 0a20 2020 2020 2020 2020  show().         
+00012400: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00012410: 2020 2020 2020 2020 2073 656c 662e 6475           self.du
+00012420: 7065 5f69 6e64 6963 6174 6f72 2e68 6964  pe_indicator.hid
+00012430: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00012440: 5f74 6865 7468 7265 6164 203d 2074 6872  _thethread = thr
+00012450: 6561 6469 6e67 2e54 6872 6561 6428 0a20  eading.Thread(. 
+00012460: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00012470: 6172 6765 743d 7365 6c66 2e63 6865 636b  arget=self.check
+00012480: 5f63 616c 6c73 6967 6e32 2c0a 2020 2020  _callsign2,.    
+00012490: 2020 2020 2020 2020 2020 2020 6172 6773              args
+000124a0: 3d28 7465 7874 2c29 2c0a 2020 2020 2020  =(text,),.      
+000124b0: 2020 2020 2020 2020 2020 6461 656d 6f6e            daemon
+000124c0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+000124d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000124e0: 205f 7468 6574 6872 6561 642e 7374 6172   _thethread.star
+000124f0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00012500: 7365 6c66 2e6e 6578 745f 6669 656c 642e  self.next_field.
+00012510: 7365 7446 6f63 7573 2829 0a20 2020 2020  setFocus().     
+00012520: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00012530: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
+00012540: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
+00012550: 5d20 3d20 2243 414c 4c43 4841 4e47 4544  ] = "CALLCHANGED
+00012560: 220a 2020 2020 2020 2020 636d 645b 2273  ".        cmd["s
+00012570: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+00012580: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+00012590: 2020 2063 6d64 5b22 6361 6c6c 225d 203d     cmd["call"] =
+000125a0: 2073 7472 6970 7065 645f 7465 7874 0a20   stripped_text. 
+000125b0: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
+000125c0: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+000125d0: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
+000125e0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+000125f0: 6865 636b 5f63 616c 6c73 6967 6e28 7374  heck_callsign(st
+00012600: 7269 7070 6564 5f74 6578 7429 0a0a 2020  ripped_text)..  
+00012610: 2020 6465 6620 6368 6563 6b5f 6361 6c6c    def check_call
+00012620: 7369 676e 2873 656c 662c 2063 616c 6c73  sign(self, calls
+00012630: 6967 6e29 3a0a 2020 2020 2020 2020 2222  ign):.        ""
+00012640: 2243 6865 636b 2063 616c 6c20 6173 2065  "Check call as e
+00012650: 6e74 6572 6564 2222 220a 2020 2020 2020  ntered""".      
+00012660: 2020 7265 7375 6c74 203d 2063 7479 5f6c    result = cty_l
+00012670: 6f6f 6b75 7028 6361 6c6c 7369 676e 290a  ookup(callsign).
+00012680: 2020 2020 2020 2020 6465 6275 675f 7265          debug_re
+00012690: 7375 6c74 203d 2066 227b 7265 7375 6c74  sult = f"{result
+000126a0: 7d22 0a20 2020 2020 2020 206c 6f67 6765  }".        logge
+000126b0: 722e 6465 6275 6728 2225 7322 2c20 6465  r.debug("%s", de
+000126c0: 6275 675f 7265 7375 6c74 290a 2020 2020  bug_result).    
+000126d0: 2020 2020 6966 2072 6573 756c 743a 0a20      if result:. 
+000126e0: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
+000126f0: 2069 6e20 7265 7375 6c74 2e69 7465 6d73   in result.items
+00012700: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00012710: 2020 2020 656e 7469 7479 203d 2061 5b31      entity = a[1
+00012720: 5d2e 6765 7428 2265 6e74 6974 7922 2c20  ].get("entity", 
+00012730: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
+00012740: 2020 2020 6371 203d 2061 5b31 5d2e 6765      cq = a[1].ge
+00012750: 7428 2263 7122 2c20 2222 290a 2020 2020  t("cq", "").    
+00012760: 2020 2020 2020 2020 2020 2020 6974 7520              itu 
+00012770: 3d20 615b 315d 2e67 6574 2822 6974 7522  = a[1].get("itu"
+00012780: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
+00012790: 2020 2020 2020 636f 6e74 696e 656e 7420        continent 
+000127a0: 3d20 615b 315d 2e67 6574 2822 636f 6e74  = a[1].get("cont
+000127b0: 696e 656e 7422 290a 2020 2020 2020 2020  inent").        
+000127c0: 2020 2020 2020 2020 6c61 7420 3d20 666c          lat = fl
+000127d0: 6f61 7428 615b 315d 2e67 6574 2822 6c61  oat(a[1].get("la
+000127e0: 7422 2c20 2230 2e30 2229 290a 2020 2020  t", "0.0")).    
+000127f0: 2020 2020 2020 2020 2020 2020 6c6f 6e20              lon 
+00012800: 3d20 666c 6f61 7428 615b 315d 2e67 6574  = float(a[1].get
+00012810: 2822 6c6f 6e67 222c 2022 302e 3022 2929  ("long", "0.0"))
+00012820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012830: 206c 6f6e 203d 206c 6f6e 202a 202d 3120   lon = lon * -1 
+00012840: 2023 2063 7479 2e64 6174 2066 696c 6520   # cty.dat file 
+00012850: 696e 7665 7274 7320 6c6f 6e67 6974 7564  inverts longitud
+00012860: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00012870: 2020 2070 7269 6d61 7279 5f70 6678 203d     primary_pfx =
+00012880: 2061 5b31 5d2e 6765 7428 2270 7269 6d61   a[1].get("prima
+00012890: 7279 5f70 6678 222c 2022 2229 0a20 2020  ry_pfx", "").   
+000128a0: 2020 2020 2020 2020 2020 2020 2068 6561               hea
+000128b0: 6469 6e67 203d 2062 6561 7269 6e67 5f77  ding = bearing_w
+000128c0: 6974 685f 6c61 746c 6f6e 2873 656c 662e  ith_latlon(self.
+000128d0: 7374 6174 696f 6e2e 6765 7428 2247 7269  station.get("Gri
+000128e0: 6453 7175 6172 6522 292c 206c 6174 2c20  dSquare"), lat, 
+000128f0: 6c6f 6e29 0a20 2020 2020 2020 2020 2020  lon).           
+00012900: 2020 2020 206b 696c 6f6d 6574 6572 7320       kilometers 
+00012910: 3d20 6469 7374 616e 6365 5f77 6974 685f  = distance_with_
+00012920: 6c61 746c 6f6e 280a 2020 2020 2020 2020  latlon(.        
+00012930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012940: 2e73 7461 7469 6f6e 2e67 6574 2822 4772  .station.get("Gr
+00012950: 6964 5371 7561 7265 2229 2c20 6c61 742c  idSquare"), lat,
+00012960: 206c 6f6e 0a20 2020 2020 2020 2020 2020   lon.           
+00012970: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00012980: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+00012990: 696e 675f 6469 7374 616e 6365 2e73 6574  ing_distance.set
+000129a0: 5465 7874 280a 2020 2020 2020 2020 2020  Text(.          
+000129b0: 2020 2020 2020 2020 2020 6622 5265 6769            f"Regi
+000129c0: 6f6e 616c 2048 6467 207b 6865 6164 696e  onal Hdg {headin
+000129d0: 677d c2b0 204c 5020 7b72 6563 6970 726f  g}.. LP {recipro
+000129e0: 636f 6c28 6865 6164 696e 6729 7dc2 b020  col(heading)}.. 
+000129f0: 2f20 220a 2020 2020 2020 2020 2020 2020  / ".            
+00012a00: 2020 2020 2020 2020 6622 6469 7374 616e          f"distan
+00012a10: 6365 207b 696e 7428 6b69 6c6f 6d65 7465  ce {int(kilomete
+00012a20: 7273 2a30 2e36 3231 3337 3129 7d6d 6920  rs*0.621371)}mi 
+00012a30: 7b6b 696c 6f6d 6574 6572 737d 6b6d 220a  {kilometers}km".
+00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012a60: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+00012a70: 436f 756e 7472 7950 7265 6669 7822 5d20  CountryPrefix"] 
+00012a80: 3d20 7072 696d 6172 795f 7066 780a 2020  = primary_pfx.  
+00012a90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012aa0: 6c66 2e63 6f6e 7461 6374 5b22 5a4e 225d  lf.contact["ZN"]
+00012ab0: 203d 2069 6e74 2863 7129 0a20 2020 2020   = int(cq).     
+00012ac0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012ad0: 636f 6e74 6163 745b 2243 6f6e 7469 6e65  contact["Contine
+00012ae0: 6e74 225d 203d 2063 6f6e 7469 6e65 6e74  nt"] = continent
+00012af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b00: 2073 656c 662e 6478 5f65 6e74 6974 792e   self.dx_entity.
+00012b10: 7365 7454 6578 7428 0a20 2020 2020 2020  setText(.       
+00012b20: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
+00012b30: 7072 696d 6172 795f 7066 787d 3a20 7b63  primary_pfx}: {c
+00012b40: 6f6e 7469 6e65 6e74 7d2f 7b65 6e74 6974  ontinent}/{entit
+00012b50: 797d 2063 713a 7b63 717d 2069 7475 3a7b  y} cq:{cq} itu:{
+00012b60: 6974 757d 220a 2020 2020 2020 2020 2020  itu}".          
+00012b70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00012b80: 2020 2020 2020 2020 6966 206c 656e 2863          if len(c
+00012b90: 616c 6c73 6967 6e29 203e 2032 3a0a 2020  allsign) > 2:.  
+00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bb0: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
+00012bc0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00012bd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012be0: 636f 6e74 6573 742e 7072 6566 696c 6c28  contest.prefill(
+00012bf0: 7365 6c66 290a 0a20 2020 2064 6566 2063  self)..    def c
+00012c00: 6865 636b 5f63 616c 6c73 6967 6e32 2873  heck_callsign2(s
+00012c10: 656c 662c 2063 616c 6c73 6967 6e29 3a0a  elf, callsign):.
+00012c20: 2020 2020 2020 2020 2222 2243 6865 636b          """Check
+00012c30: 2063 616c 6c20 6f6e 6365 2065 6e74 6572   call once enter
+00012c40: 6564 2222 220a 2020 2020 2020 2020 6361  ed""".        ca
+00012c50: 6c6c 7369 676e 203d 2063 616c 6c73 6967  llsign = callsig
+00012c60: 6e2e 7374 7269 7028 290a 2020 2020 2020  n.strip().      
+00012c70: 2020 6465 6275 675f 6c6f 6f6b 7570 203d    debug_lookup =
+00012c80: 2066 227b 7365 6c66 2e6c 6f6f 6b5f 7570   f"{self.look_up
+00012c90: 7d22 0a20 2020 2020 2020 206c 6f67 6765  }".        logge
+00012ca0: 722e 6465 6275 6728 2225 732c 2025 7322  r.debug("%s, %s"
+00012cb0: 2c20 6361 6c6c 7369 676e 2c20 6465 6275  , callsign, debu
+00012cc0: 675f 6c6f 6f6b 7570 290a 2020 2020 2020  g_lookup).      
+00012cd0: 2020 6966 2068 6173 6174 7472 2873 656c    if hasattr(sel
+00012ce0: 662e 6c6f 6f6b 5f75 702c 2022 7365 7373  f.look_up, "sess
+00012cf0: 696f 6e22 293a 0a20 2020 2020 2020 2020  ion"):.         
+00012d00: 2020 2069 6620 7365 6c66 2e6c 6f6f 6b5f     if self.look_
+00012d10: 7570 2e73 6573 7369 6f6e 3a0a 2020 2020  up.session:.    
+00012d20: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+00012d30: 6f6e 7365 203d 2073 656c 662e 6c6f 6f6b  onse = self.look
+00012d40: 5f75 702e 6c6f 6f6b 7570 2863 616c 6c73  _up.lookup(calls
+00012d50: 6967 6e29 0a20 2020 2020 2020 2020 2020  ign).           
+00012d60: 2020 2020 2064 6562 7567 5f72 6573 706f       debug_respo
+00012d70: 6e73 6520 3d20 6622 7b72 6573 706f 6e73  nse = f"{respons
+00012d80: 657d 220a 2020 2020 2020 2020 2020 2020  e}".            
+00012d90: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00012da0: 2822 5468 6520 5265 7370 6f6e 7365 3a20  ("The Response: 
+00012db0: 2573 5c6e 222c 2064 6562 7567 5f72 6573  %s\n", debug_res
+00012dc0: 706f 6e73 6529 0a20 2020 2020 2020 2020  ponse).         
+00012dd0: 2020 2020 2020 2069 6620 7265 7370 6f6e         if respon
+00012de0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012df0: 2020 2020 2020 2020 7468 6569 7267 7269          theirgri
+00012e00: 6420 3d20 7265 7370 6f6e 7365 2e67 6574  d = response.get
+00012e10: 2822 6772 6964 2229 0a20 2020 2020 2020  ("grid").       
+00012e20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012e30: 662e 636f 6e74 6163 745b 2247 7269 6453  f.contact["GridS
+00012e40: 7175 6172 6522 5d20 3d20 7468 6569 7267  quare"] = theirg
+00012e50: 7269 640a 2020 2020 2020 2020 2020 2020  rid.            
+00012e60: 2020 2020 2020 2020 5f74 6865 6972 636f          _theirco
+00012e70: 756e 7472 7920 3d20 7265 7370 6f6e 7365  untry = response
+00012e80: 2e67 6574 2822 636f 756e 7472 7922 290a  .get("country").
+00012e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ea0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00012eb0: 696f 6e2e 6765 7428 2247 7269 6453 7175  ion.get("GridSqu
+00012ec0: 6172 6522 2c20 2222 293a 0a20 2020 2020  are", ""):.     
+00012ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ee0: 2020 2068 6561 6469 6e67 203d 2062 6561     heading = bea
+00012ef0: 7269 6e67 2873 656c 662e 7374 6174 696f  ring(self.statio
+00012f00: 6e2e 6765 7428 2247 7269 6453 7175 6172  n.get("GridSquar
+00012f10: 6522 2c20 2222 292c 2074 6865 6972 6772  e", ""), theirgr
+00012f20: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
+00012f30: 2020 2020 2020 2020 2020 2020 6b69 6c6f              kilo
+00012f40: 6d65 7465 7273 203d 2064 6973 7461 6e63  meters = distanc
+00012f50: 6528 7365 6c66 2e73 7461 7469 6f6e 2e67  e(self.station.g
+00012f60: 6574 2822 4772 6964 5371 7561 7265 2229  et("GridSquare")
+00012f70: 2c20 7468 6569 7267 7269 6429 0a20 2020  , theirgrid).   
+00012f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f90: 2020 2020 2073 656c 662e 6865 6164 696e       self.headin
+00012fa0: 675f 6469 7374 616e 6365 2e73 6574 5465  g_distance.setTe
+00012fb0: 7874 280a 2020 2020 2020 2020 2020 2020  xt(.            
+00012fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fd0: 6622 7b74 6865 6972 6772 6964 7d20 4864  f"{theirgrid} Hd
+00012fe0: 6720 7b68 6561 6469 6e67 7dc2 b020 4c50  g {heading}.. LP
+00012ff0: 207b 7265 6369 7072 6f63 6f6c 2868 6561   {reciprocol(hea
+00013000: 6469 6e67 297d c2b0 202f 2022 0a20 2020  ding)}.. / ".   
+00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013020: 2020 2020 2020 2020 2066 2264 6973 7461           f"dista
+00013030: 6e63 6520 7b69 6e74 286b 696c 6f6d 6574  nce {int(kilomet
+00013040: 6572 732a 302e 3632 3133 3731 297d 6d69  ers*0.621371)}mi
+00013050: 207b 6b69 6c6f 6d65 7465 7273 7d6b 6d22   {kilometers}km"
+00013060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013070: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00013080: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00013090: 2073 656c 662e 6478 5f65 6e74 6974 792e   self.dx_entity.
+000130a0: 7365 7454 6578 7428 6622 7b74 6865 6972  setText(f"{their
+000130b0: 636f 756e 7472 797d 2229 0a20 2020 2020  country}").     
+000130c0: 2020 2020 2020 2020 2020 2023 2065 6c73             # els
+000130d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000130e0: 2020 2023 2073 656c 662e 6865 6164 696e     # self.headin
+000130f0: 675f 6469 7374 616e 6365 2e73 6574 5465  g_distance.setTe
+00013100: 7874 2822 4c6f 6f6b 7570 2066 6169 6c65  xt("Lookup faile
+00013110: 642e 2229 0a0a 2020 2020 6465 6620 6368  d.")..    def ch
+00013120: 6563 6b5f 6475 7065 2873 656c 662c 2063  eck_dupe(self, c
+00013130: 616c 6c3a 2073 7472 2920 2d3e 2062 6f6f  all: str) -> boo
+00013140: 6c3a 0a20 2020 2020 2020 2022 2222 4368  l:.        """Ch
+00013150: 6563 6b73 2069 6620 6120 6361 6c6c 7369  ecks if a callsi
+00013160: 676e 2069 7320 6120 6475 7065 206f 6e20  gn is a dupe on 
+00013170: 6375 7272 656e 7420 6261 6e64 2f6d 6f64  current band/mod
+00013180: 652e 2222 220a 2020 2020 2020 2020 7365  e.""".        se
+00013190: 6c66 2e63 6f6e 7465 7374 2e70 7265 6475  lf.contest.predu
+000131a0: 7065 2873 656c 6629 0a20 2020 2020 2020  pe(self).       
+000131b0: 2062 616e 6420 3d20 666c 6f61 7428 6765   band = float(ge
+000131c0: 745f 6c6f 6767 6564 5f62 616e 6428 7374  t_logged_band(st
+000131d0: 7228 7365 6c66 2e72 6164 696f 5f73 7461  r(self.radio_sta
+000131e0: 7465 2e67 6574 2822 7666 6f61 222c 2030  te.get("vfoa", 0
+000131f0: 2e30 2929 2929 0a20 2020 2020 2020 206d  .0)))).        m
+00013200: 6f64 6520 3d20 7365 6c66 2e72 6164 696f  ode = self.radio
+00013210: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+00013220: 222c 2022 2229 0a20 2020 2020 2020 2064  ", "").        d
+00013230: 6562 7567 6c69 6e65 203d 2028 0a20 2020  ebugline = (.   
+00013240: 2020 2020 2020 2020 2066 2243 616c 6c3a           f"Call:
+00013250: 207b 6361 6c6c 7d20 4261 6e64 3a20 7b62   {call} Band: {b
+00013260: 616e 647d 204d 6f64 653a 207b 6d6f 6465  and} Mode: {mode
+00013270: 7d20 4475 7065 7479 7065 3a20 7b73 656c  } Dupetype: {sel
+00013280: 662e 636f 6e74 6573 742e 6475 7065 5f74  f.contest.dupe_t
+00013290: 7970 657d 220a 2020 2020 2020 2020 290a  ype}".        ).
+000132a0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+000132b0: 6562 7567 2822 2573 222c 2064 6562 7567  ebug("%s", debug
+000132c0: 6c69 6e65 290a 2020 2020 2020 2020 6966  line).        if
+000132d0: 2073 656c 662e 636f 6e74 6573 742e 6475   self.contest.du
+000132e0: 7065 5f74 7970 6520 3d3d 2031 3a0a 2020  pe_type == 1:.  
+000132f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00013300: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
+00013310: 2e63 6865 636b 5f64 7570 6528 6361 6c6c  .check_dupe(call
+00013320: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00013330: 662e 636f 6e74 6573 742e 6475 7065 5f74  f.contest.dupe_t
+00013340: 7970 6520 3d3d 2032 3a0a 2020 2020 2020  ype == 2:.      
+00013350: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00013360: 656c 662e 6461 7461 6261 7365 2e63 6865  elf.database.che
+00013370: 636b 5f64 7570 655f 6f6e 5f62 616e 6428  ck_dupe_on_band(
+00013380: 6361 6c6c 2c20 6261 6e64 290a 2020 2020  call, band).    
+00013390: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
+000133a0: 6573 742e 6475 7065 5f74 7970 6520 3d3d  est.dupe_type ==
+000133b0: 2033 3a0a 2020 2020 2020 2020 2020 2020   3:.            
+000133c0: 7265 7375 6c74 203d 2073 656c 662e 6461  result = self.da
+000133d0: 7461 6261 7365 2e63 6865 636b 5f64 7570  tabase.check_dup
+000133e0: 655f 6f6e 5f62 616e 645f 6d6f 6465 2863  e_on_band_mode(c
+000133f0: 616c 6c2c 2062 616e 642c 206d 6f64 6529  all, band, mode)
+00013400: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00013410: 2e63 6f6e 7465 7374 2e64 7570 655f 7479  .contest.dupe_ty
+00013420: 7065 203d 3d20 343a 0a20 2020 2020 2020  pe == 4:.       
+00013430: 2020 2020 2072 6573 756c 7420 3d20 7b22       result = {"
+00013440: 6973 6475 7065 223a 2046 616c 7365 7d0a  isdupe": False}.
+00013450: 2020 2020 2020 2020 6465 6275 676c 696e          debuglin
+00013460: 6520 3d20 6622 7b72 6573 756c 747d 220a  e = f"{result}".
+00013470: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00013480: 6562 7567 2822 2573 222c 2064 6562 7567  ebug("%s", debug
+00013490: 6c69 6e65 290a 2020 2020 2020 2020 7265  line).        re
+000134a0: 7475 726e 2072 6573 756c 742e 6765 7428  turn result.get(
+000134b0: 2269 7364 7570 6522 2c20 4661 6c73 6529  "isdupe", False)
+000134c0: 0a0a 2020 2020 6465 6620 7365 746d 6f64  ..    def setmod
+000134d0: 6528 7365 6c66 2c20 6d6f 6465 3a20 7374  e(self, mode: st
+000134e0: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
+000134f0: 2020 2020 2222 2273 7475 6220 666f 7220      """stub for 
+00013500: 7768 656e 2074 6865 206d 6f64 6520 6368  when the mode ch
+00013510: 616e 6765 732e 2222 220a 2020 2020 2020  anges.""".      
+00013520: 2020 6966 206d 6f64 6520 3d3d 2022 4357    if mode == "CW
+00013530: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
+00013540: 656c 662e 6375 7272 656e 745f 6d6f 6465  elf.current_mode
+00013550: 203d 2022 4357 220a 2020 2020 2020 2020   = "CW".        
+00013560: 2020 2020 2320 7365 6c66 2e6d 6f64 652e      # self.mode.
+00013570: 7365 7454 6578 7428 2243 5722 290a 2020  setText("CW").  
+00013580: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00013590: 656e 742e 7365 7454 6578 7428 2235 3939  ent.setText("599
+000135a0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+000135b0: 656c 662e 7265 6365 6976 652e 7365 7454  elf.receive.setT
+000135c0: 6578 7428 2235 3939 2229 0a20 2020 2020  ext("599").     
+000135d0: 2020 2020 2020 2073 656c 662e 7265 6164         self.read
+000135e0: 5f63 775f 6d61 6372 6f73 2829 0a20 2020  _cw_macros().   
+000135f0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00013600: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
+00013610: 3d3d 2022 5353 4222 3a0a 2020 2020 2020  == "SSB":.      
+00013620: 2020 2020 2020 7365 6c66 2e63 7572 7265        self.curre
+00013630: 6e74 5f6d 6f64 6520 3d20 2253 5342 220a  nt_mode = "SSB".
+00013640: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+00013650: 6c66 2e6d 6f64 652e 7365 7454 6578 7428  lf.mode.setText(
+00013660: 2253 5342 2229 0a20 2020 2020 2020 2020  "SSB").         
+00013670: 2020 2073 656c 662e 7365 6e74 2e73 6574     self.sent.set
+00013680: 5465 7874 2822 3539 2229 0a20 2020 2020  Text("59").     
+00013690: 2020 2020 2020 2073 656c 662e 7265 6365         self.rece
+000136a0: 6976 652e 7365 7454 6578 7428 2235 3922  ive.setText("59"
+000136b0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000136c0: 6c66 2e72 6561 645f 6377 5f6d 6163 726f  lf.read_cw_macro
+000136d0: 7328 290a 2020 2020 2020 2020 6966 206d  s().        if m
+000136e0: 6f64 6520 3d3d 2022 5254 5459 223a 0a20  ode == "RTTY":. 
+000136f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013700: 6375 7272 656e 745f 6d6f 6465 203d 2022  current_mode = "
+00013710: 5254 5459 220a 2020 2020 2020 2020 2020  RTTY".          
+00013720: 2020 2320 7365 6c66 2e6d 6f64 652e 7365    # self.mode.se
+00013730: 7454 6578 7428 2252 5454 5922 290a 2020  tText("RTTY").  
+00013740: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00013750: 656e 742e 7365 7454 6578 7428 2235 3922  ent.setText("59"
+00013760: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00013770: 6c66 2e72 6563 6569 7665 2e73 6574 5465  lf.receive.setTe
+00013780: 7874 2822 3539 2229 0a0a 2020 2020 6465  xt("59")..    de
+00013790: 6620 6765 745f 6f70 6f6e 2873 656c 6629  f get_opon(self)
+000137a0: 3a0a 2020 2020 2020 2020 2222 2243 7472  :.        """Ctr
+000137b0: 6c2b 4f20 6f72 204f 504f 4e20 6469 616c  l+O or OPON dial
+000137c0: 6f67 2222 220a 2020 2020 2020 2020 7365  og""".        se
+000137d0: 6c66 2e6f 706f 6e5f 6469 616c 6f67 203d  lf.opon_dialog =
+000137e0: 204f 704f 6e28 574f 524b 494e 475f 5041   OpOn(WORKING_PA
+000137f0: 5448 290a 2020 2020 2020 2020 7365 6c66  TH).        self
+00013800: 2e6f 706f 6e5f 6469 616c 6f67 2e61 6363  .opon_dialog.acc
+00013810: 6570 7465 642e 636f 6e6e 6563 7428 7365  epted.connect(se
+00013820: 6c66 2e6e 6577 5f6f 7029 0a20 2020 2020  lf.new_op).     
+00013830: 2020 2073 656c 662e 6f70 6f6e 5f64 6961     self.opon_dia
+00013840: 6c6f 672e 6f70 656e 2829 0a0a 2020 2020  log.open()..    
+00013850: 6465 6620 6e65 775f 6f70 2873 656c 6629  def new_op(self)
+00013860: 3a0a 2020 2020 2020 2020 2222 2253 6176  :.        """Sav
+00013870: 6520 6e65 7720 4f50 2222 220a 2020 2020  e new OP""".    
+00013880: 2020 2020 6966 2073 656c 662e 6f70 6f6e      if self.opon
+00013890: 5f64 6961 6c6f 672e 4e65 774f 7065 7261  _dialog.NewOpera
+000138a0: 746f 722e 7465 7874 2829 3a0a 2020 2020  tor.text():.    
+000138b0: 2020 2020 2020 2020 7365 6c66 2e63 7572          self.cur
+000138c0: 7265 6e74 5f6f 7020 3d20 7365 6c66 2e6f  rent_op = self.o
+000138d0: 706f 6e5f 6469 616c 6f67 2e4e 6577 4f70  pon_dialog.NewOp
+000138e0: 6572 6174 6f72 2e74 6578 7428 292e 7570  erator.text().up
+000138f0: 7065 7228 290a 2020 2020 2020 2020 7365  per().        se
+00013900: 6c66 2e6f 706f 6e5f 6469 616c 6f67 2e63  lf.opon_dialog.c
+00013910: 6c6f 7365 2829 0a20 2020 2020 2020 206c  lose().        l
+00013920: 6f67 6765 722e 6465 6275 6728 224e 6577  ogger.debug("New
+00013930: 204f 703a 2025 7322 2c20 7365 6c66 2e63   Op: %s", self.c
+00013940: 7572 7265 6e74 5f6f 7029 0a20 2020 2020  urrent_op).     
+00013950: 2020 2073 656c 662e 6d61 6b65 5f6f 705f     self.make_op_
+00013960: 6469 7228 290a 0a20 2020 2064 6566 206d  dir()..    def m
+00013970: 616b 655f 6f70 5f64 6972 2873 656c 6629  ake_op_dir(self)
+00013980: 3a0a 2020 2020 2020 2020 2222 2243 7265  :.        """Cre
+00013990: 6174 6520 4f50 2064 6972 6563 746f 7279  ate OP directory
+000139a0: 2069 6620 6974 2064 6f65 7320 6e6f 7420   if it does not 
+000139b0: 6578 6973 742e 2222 220a 2020 2020 2020  exist.""".      
+000139c0: 2020 6966 2073 656c 662e 6375 7272 656e    if self.curren
+000139d0: 745f 6f70 3a0a 2020 2020 2020 2020 2020  t_op:.          
+000139e0: 2020 6f70 5f70 6174 6820 3d20 5061 7468    op_path = Path
+000139f0: 2844 4154 415f 5041 5448 2920 2f20 7365  (DATA_PATH) / se
+00013a00: 6c66 2e63 7572 7265 6e74 5f6f 700a 2020  lf.current_op.  
+00013a10: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00013a20: 2e64 6562 7567 2822 6f70 5f70 6174 683a  .debug("op_path:
+00013a30: 2025 7322 2c20 7374 7228 6f70 5f70 6174   %s", str(op_pat
+00013a40: 6829 290a 2020 2020 2020 2020 2020 2020  h)).            
+00013a50: 6966 206f 705f 7061 7468 2e69 735f 6469  if op_path.is_di
+00013a60: 7228 2920 6973 2046 616c 7365 3a0a 2020  r() is False:.  
+00013a70: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00013a80: 6767 6572 2e64 6562 7567 2822 4372 6561  gger.debug("Crea
+00013a90: 7469 6e67 204f 7020 4469 7265 6374 6f72  ting Op Director
+00013aa0: 793a 2025 7322 2c20 7374 7228 6f70 5f70  y: %s", str(op_p
+00013ab0: 6174 6829 290a 2020 2020 2020 2020 2020  ath)).          
+00013ac0: 2020 2020 2020 6f73 2e6d 6b64 6972 2873        os.mkdir(s
+00013ad0: 7472 286f 705f 7061 7468 2929 0a20 2020  tr(op_path)).   
+00013ae0: 2020 2020 2020 2020 2069 6620 6f70 5f70           if op_p
+00013af0: 6174 682e 6973 5f64 6972 2829 3a0a 2020  ath.is_dir():.  
+00013b00: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00013b10: 7572 6365 5f70 6174 6820 3d20 5061 7468  urce_path = Path
+00013b20: 2857 4f52 4b49 4e47 5f50 4154 4829 202f  (WORKING_PATH) /
+00013b30: 2022 6461 7461 2220 2f20 2270 686f 6e65   "data" / "phone
+00013b40: 7469 6373 220a 2020 2020 2020 2020 2020  tics".          
+00013b50: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00013b60: 7567 2822 736f 7572 6365 5f70 6174 683a  ug("source_path:
+00013b70: 2025 7322 2c20 7374 7228 736f 7572 6365   %s", str(source
+00013b80: 5f70 6174 6829 290a 2020 2020 2020 2020  _path)).        
+00013b90: 2020 2020 2020 2020 666f 7220 6368 696c          for chil
+00013ba0: 6420 696e 2073 6f75 7263 655f 7061 7468  d in source_path
+00013bb0: 2e69 7465 7264 6972 2829 3a0a 2020 2020  .iterdir():.    
+00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bd0: 6465 7374 696e 6174 696f 6e5f 6669 6c65  destination_file
+00013be0: 203d 206f 705f 7061 7468 202f 2063 6869   = op_path / chi
+00013bf0: 6c64 2e6e 616d 650a 2020 2020 2020 2020  ld.name.        
+00013c00: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+00013c10: 6573 7469 6e61 7469 6f6e 5f66 696c 652e  estination_file.
+00013c20: 6973 5f66 696c 6528 2920 6973 2046 616c  is_file() is Fal
+00013c30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00013c40: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00013c50: 6572 2e64 6562 7567 2822 4465 7374 696e  er.debug("Destin
+00013c60: 6174 696f 6e3a 2025 7322 2c20 7374 7228  ation: %s", str(
+00013c70: 6465 7374 696e 6174 696f 6e5f 6669 6c65  destination_file
+00013c80: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00013c90: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+00013ca0: 6e61 7469 6f6e 5f66 696c 652e 7772 6974  nation_file.writ
+00013cb0: 655f 6279 7465 7328 6368 696c 642e 7265  e_bytes(child.re
+00013cc0: 6164 5f62 7974 6573 2829 290a 0a20 2020  ad_bytes())..   
+00013cd0: 2064 6566 2070 6f6c 6c5f 7261 6469 6f28   def poll_radio(
+00013ce0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00013cf0: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+00013d00: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
+00013d10: 6e74 726f 6c3a 0a20 2020 2020 2020 2020  ntrol:.         
+00013d20: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
+00013d30: 6f6e 7472 6f6c 2e6f 6e6c 696e 6520 6973  ontrol.online is
+00013d40: 2046 616c 7365 3a0a 2020 2020 2020 2020   False:.        
+00013d50: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
+00013d60: 5f63 6f6e 7472 6f6c 2e72 6569 6e69 7428  _control.reinit(
+00013d70: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00013d80: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+00013d90: 6c2e 6f6e 6c69 6e65 3a0a 2020 2020 2020  l.online:.      
+00013da0: 2020 2020 2020 2020 2020 696e 666f 5f64            info_d
+00013db0: 6972 7479 203d 2046 616c 7365 0a20 2020  irty = False.   
+00013dc0: 2020 2020 2020 2020 2020 2020 2076 666f               vfo
+00013dd0: 203d 2073 656c 662e 7269 675f 636f 6e74   = self.rig_cont
+00013de0: 726f 6c2e 6765 745f 7666 6f28 290a 2020  rol.get_vfo().  
+00013df0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00013e00: 6465 203d 2073 656c 662e 7269 675f 636f  de = self.rig_co
+00013e10: 6e74 726f 6c2e 6765 745f 6d6f 6465 2829  ntrol.get_mode()
+00013e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013e30: 2062 7720 3d20 7365 6c66 2e72 6967 5f63   bw = self.rig_c
+00013e40: 6f6e 7472 6f6c 2e67 6574 5f62 7728 290a  ontrol.get_bw().
+00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e60: 2320 7365 6c66 2e72 6164 696f 5f73 7461  # self.radio_sta
+00013e70: 7465 5b22 7074 7422 5d20 3d20 7365 6c66  te["ptt"] = self
+00013e80: 2e72 6967 5f63 6f6e 7472 6f6c 2e67 6574  .rig_control.get
+00013e90: 5f70 7474 2829 0a0a 2020 2020 2020 2020  _ptt()..        
+00013ea0: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
+00013eb0: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
+00013ec0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013ed0: 662e 7365 746d 6f64 6528 6d6f 6465 290a  f.setmode(mode).
+00013ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ef0: 6966 206d 6f64 6520 3d3d 2022 4c53 4222  if mode == "LSB"
+00013f00: 206f 7220 6d6f 6465 203d 3d20 2255 5342   or mode == "USB
+00013f10: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00013f20: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
+00013f30: 6f64 6528 2253 5342 2229 0a20 2020 2020  ode("SSB").     
+00013f40: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+00013f50: 6465 203d 3d20 2252 5454 5922 3a0a 2020  de == "RTTY":.  
+00013f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f70: 2020 7365 6c66 2e73 6574 6d6f 6465 2822    self.setmode("
+00013f80: 5254 5459 2229 0a0a 2020 2020 2020 2020  RTTY")..        
+00013f90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00013fa0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+00013fb0: 2276 666f 6122 2920 213d 2076 666f 3a0a  "vfoa") != vfo:.
+00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fd0: 2020 2020 696e 666f 5f64 6972 7479 203d      info_dirty =
+00013fe0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+00013ff0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00014000: 6164 696f 5f73 7461 7465 5b22 7666 6f61  adio_state["vfoa
+00014010: 225d 203d 2076 666f 0a20 2020 2020 2020  "] = vfo.       
+00014020: 2020 2020 2020 2020 2062 616e 6420 3d20           band = 
+00014030: 6765 7462 616e 6428 7374 7228 7666 6f29  getband(str(vfo)
+00014040: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014050: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
+00014060: 7465 5b22 6261 6e64 225d 203d 2062 616e  te["band"] = ban
+00014070: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00014080: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+00014090: 4261 6e64 225d 203d 2067 6574 5f6c 6f67  Band"] = get_log
+000140a0: 6765 645f 6261 6e64 2873 7472 2876 666f  ged_band(str(vfo
+000140b0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000140c0: 2020 2073 656c 662e 7365 745f 6261 6e64     self.set_band
+000140d0: 5f69 6e64 6963 6174 6f72 2862 616e 6429  _indicator(band)
+000140e0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000140f0: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
+00014100: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
+00014110: 2920 213d 206d 6f64 653a 0a20 2020 2020  ) != mode:.     
+00014120: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014130: 6e66 6f5f 6469 7274 7920 3d20 5472 7565  nfo_dirty = True
+00014140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014150: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
+00014160: 7374 6174 655b 226d 6f64 6522 5d20 3d20  state["mode"] = 
+00014170: 6d6f 6465 0a0a 2020 2020 2020 2020 2020  mode..          
+00014180: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
+00014190: 6469 6f5f 7374 6174 652e 6765 7428 2262  dio_state.get("b
+000141a0: 7722 2920 213d 2062 773a 0a20 2020 2020  w") != bw:.     
+000141b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000141c0: 6e66 6f5f 6469 7274 7920 3d20 5472 7565  nfo_dirty = True
+000141d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000141e0: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
+000141f0: 7374 6174 655b 2262 7722 5d20 3d20 6277  state["bw"] = bw
+00014200: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014210: 2020 6966 2064 6174 6574 696d 652e 6e6f    if datetime.no
+00014220: 7728 2920 3e20 676c 6f62 616c 7328 295b  w() > globals()[
+00014230: 2270 6f6c 6c5f 7469 6d65 225d 206f 7220  "poll_time"] or 
+00014240: 696e 666f 5f64 6972 7479 3a0a 2020 2020  info_dirty:.    
 00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014260: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00014270: 5b22 6261 6e64 225d 203d 2062 616e 640a  ["band"] = band.
-00014280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014290: 7365 6c66 2e63 6f6e 7461 6374 5b22 4261  self.contact["Ba
-000142a0: 6e64 225d 203d 2067 6574 5f6c 6f67 6765  nd"] = get_logge
-000142b0: 645f 6261 6e64 2873 7472 2876 666f 2929  d_band(str(vfo))
-000142c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000142d0: 2073 656c 662e 7365 745f 6261 6e64 5f69   self.set_band_i
-000142e0: 6e64 6963 6174 6f72 2862 616e 6429 0a0a  ndicator(band)..
-000142f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014300: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
-00014310: 6174 652e 6765 7428 226d 6f64 6522 2920  ate.get("mode") 
-00014320: 213d 206d 6f64 653a 0a20 2020 2020 2020  != mode:.       
-00014330: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
-00014340: 6f5f 6469 7274 7920 3d20 5472 7565 0a20  o_dirty = True. 
-00014350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014360: 2020 2073 656c 662e 7261 6469 6f5f 7374     self.radio_st
-00014370: 6174 655b 226d 6f64 6522 5d20 3d20 6d6f  ate["mode"] = mo
-00014380: 6465 0a0a 2020 2020 2020 2020 2020 2020  de..            
-00014390: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
-000143a0: 6f5f 7374 6174 652e 6765 7428 2262 7722  o_state.get("bw"
-000143b0: 2920 213d 2062 773a 0a20 2020 2020 2020  ) != bw:.       
-000143c0: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
-000143d0: 6f5f 6469 7274 7920 3d20 5472 7565 0a20  o_dirty = True. 
+00014260: 6c6f 6767 6572 2e64 6562 7567 2822 5646  logger.debug("VF
+00014270: 4f3a 2025 7320 204d 4f44 453a 2025 7320  O: %s  MODE: %s 
+00014280: 4257 3a20 2573 222c 2076 666f 2c20 6d6f  BW: %s", vfo, mo
+00014290: 6465 2c20 6277 290a 2020 2020 2020 2020  de, bw).        
+000142a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000142b0: 2e73 6574 5f77 696e 646f 775f 7469 746c  .set_window_titl
+000142c0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+000142d0: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
+000142e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000142f0: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
+00014300: 3d20 2252 4144 494f 5f53 5441 5445 220a  = "RADIO_STATE".
+00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014320: 2020 2020 636d 645b 2273 7461 7469 6f6e      cmd["station
+00014330: 225d 203d 2070 6c61 7466 6f72 6d2e 6e6f  "] = platform.no
+00014340: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00014350: 2020 2020 2020 2020 2063 6d64 5b22 6261           cmd["ba
+00014360: 6e64 225d 203d 2062 616e 640a 2020 2020  nd"] = band.    
+00014370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014380: 636d 645b 2276 666f 6122 5d20 3d20 7666  cmd["vfoa"] = vf
+00014390: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
+000143a0: 2020 2020 2020 636d 645b 226d 6f64 6522        cmd["mode"
+000143b0: 5d20 3d20 6d6f 6465 0a20 2020 2020 2020  ] = mode.       
+000143c0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+000143d0: 5b22 6277 225d 203d 2062 770a 2020 2020  ["bw"] = bw.    
 000143e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143f0: 2020 2073 656c 662e 7261 6469 6f5f 7374     self.radio_st
-00014400: 6174 655b 2262 7722 5d20 3d20 6277 0a0a  ate["bw"] = bw..
-00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014420: 6966 2064 6174 6574 696d 652e 6e6f 7728  if datetime.now(
-00014430: 2920 3e20 676c 6f62 616c 7328 295b 2270  ) > globals()["p
-00014440: 6f6c 6c5f 7469 6d65 225d 206f 7220 696e  oll_time"] or in
-00014450: 666f 5f64 6972 7479 3a0a 2020 2020 2020  fo_dirty:.      
-00014460: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00014470: 6767 6572 2e64 6562 7567 2822 5646 4f3a  gger.debug("VFO:
-00014480: 2025 7320 204d 4f44 453a 2025 7320 4257   %s  MODE: %s BW
-00014490: 3a20 2573 222c 2076 666f 2c20 6d6f 6465  : %s", vfo, mode
-000144a0: 2c20 6277 290a 2020 2020 2020 2020 2020  , bw).          
-000144b0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000144c0: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
-000144d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000144e0: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
-000144f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014500: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
-00014510: 2252 4144 494f 5f53 5441 5445 220a 2020  "RADIO_STATE".  
-00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014530: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
-00014540: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
-00014550: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00014560: 2020 2020 2020 2063 6d64 5b22 6261 6e64         cmd["band
-00014570: 225d 203d 2062 616e 640a 2020 2020 2020  "] = band.      
-00014580: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-00014590: 645b 2276 666f 6122 5d20 3d20 7666 6f0a  d["vfoa"] = vfo.
-000145a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145b0: 2020 2020 636d 645b 226d 6f64 6522 5d20      cmd["mode"] 
-000145c0: 3d20 6d6f 6465 0a20 2020 2020 2020 2020  = mode.         
-000145d0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-000145e0: 6277 225d 203d 2062 770a 2020 2020 2020  bw"] = bw.      
-000145f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00014600: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-00014610: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
-00014620: 736f 6e28 636d 6429 0a20 2020 2020 2020  son(cmd).       
-00014630: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00014640: 7365 6c66 2e6e 316d 6d3a 0a20 2020 2020  self.n1mm:.     
-00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014660: 2020 2069 6620 7365 6c66 2e6e 316d 6d2e     if self.n1mm.
-00014670: 7365 6e64 5f72 6164 696f 5f70 6163 6b65  send_radio_packe
-00014680: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-00014690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146a0: 7365 6c66 2e6e 316d 6d2e 7261 6469 6f5f  self.n1mm.radio_
-000146b0: 696e 666f 5b22 4672 6571 225d 203d 2076  info["Freq"] = v
-000146c0: 666f 5b3a 2d31 5d0a 2020 2020 2020 2020  fo[:-1].        
-000146d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146e0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
-000146f0: 6469 6f5f 696e 666f 5b22 5458 4672 6571  dio_info["TXFreq
-00014700: 225d 203d 2076 666f 5b3a 2d31 5d0a 2020  "] = vfo[:-1].  
-00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014720: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00014730: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
-00014740: 4d6f 6465 225d 203d 206d 6f64 650a 2020  Mode"] = mode.  
-00014750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014760: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00014770: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
-00014780: 4f70 4361 6c6c 225d 203d 2073 656c 662e  OpCall"] = self.
-00014790: 6375 7272 656e 745f 6f70 0a20 2020 2020  current_op.     
-000147a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147b0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-000147c0: 2e72 6164 696f 5f69 6e66 6f5b 2249 7352  .radio_info["IsR
-000147d0: 756e 6e69 6e67 225d 203d 2073 7472 280a  unning"] = str(.
-000147e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014800: 7365 6c66 2e70 7265 662e 6765 7428 2272  self.pref.get("r
-00014810: 756e 5f73 7461 7465 222c 2046 616c 7365  un_state", False
-00014820: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014830: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00014840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014860: 2e6e 316d 6d2e 7365 6e64 5f72 6164 696f  .n1mm.send_radio
-00014870: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00014880: 2020 2020 2020 2067 6c6f 6261 6c73 2829         globals()
-00014890: 5b22 706f 6c6c 5f74 696d 6522 5d20 3d20  ["poll_time"] = 
-000148a0: 6461 7465 7469 6d65 2e6e 6f77 2829 202b  datetime.now() +
-000148b0: 2064 742e 7469 6d65 6465 6c74 6128 7365   dt.timedelta(se
-000148c0: 636f 6e64 733d 3130 290a 0a20 2020 2064  conds=10)..    d
-000148d0: 6566 2065 6469 745f 6377 5f6d 6163 726f  ef edit_cw_macro
-000148e0: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
-000148f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014900: 2020 2020 2043 616c 6c73 2074 6865 2064       Calls the d
-00014910: 6566 6175 6c74 2074 6578 7420 6564 6974  efault text edit
-00014920: 6f72 2074 6f20 6564 6974 2074 6865 2043  or to edit the C
-00014930: 5720 6d61 6372 6f20 6669 6c65 2e0a 2020  W macro file..  
-00014940: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00014950: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
-00014960: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
-00014970: 2920 3d3d 2022 4357 223a 0a20 2020 2020  ) == "CW":.     
-00014980: 2020 2020 2020 206d 6163 726f 5f66 696c         macro_fil
-00014990: 6520 3d20 222f 6377 6d61 6372 6f73 2e74  e = "/cwmacros.t
-000149a0: 7874 220a 2020 2020 2020 2020 656c 7365  xt".        else
-000149b0: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-000149c0: 6372 6f5f 6669 6c65 203d 2022 2f73 7362  cro_file = "/ssb
-000149d0: 6d61 6372 6f73 2e74 7874 220a 2020 2020  macros.txt".    
-000149e0: 2020 2020 6966 206e 6f74 2050 6174 6828      if not Path(
-000149f0: 4441 5441 5f50 4154 4820 2b20 6d61 6372  DATA_PATH + macr
-00014a00: 6f5f 6669 6c65 292e 6578 6973 7473 2829  o_file).exists()
-00014a10: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-00014a20: 6767 6572 2e64 6562 7567 2822 7265 6164  gger.debug("read
-00014a30: 5f63 775f 6d61 6372 6f73 3a20 636f 7079  _cw_macros: copy
-00014a40: 696e 6720 6465 6661 756c 7420 6d61 6372  ing default macr
-00014a50: 6f20 6669 6c65 2e22 290a 2020 2020 2020  o file.").      
-00014a60: 2020 2020 2020 636f 7079 6669 6c65 2857        copyfile(W
-00014a70: 4f52 4b49 4e47 5f50 4154 4820 2b20 222f  ORKING_PATH + "/
-00014a80: 6461 7461 2220 2b20 6d61 6372 6f5f 6669  data" + macro_fi
-00014a90: 6c65 2c20 4441 5441 5f50 4154 4820 2b20  le, DATA_PATH + 
-00014aa0: 6d61 6372 6f5f 6669 6c65 290a 2020 2020  macro_file).    
-00014ab0: 2020 2020 6f73 2e73 7973 7465 6d28 6622      os.system(f"
-00014ac0: 7864 672d 6f70 656e 207b 4441 5441 5f50  xdg-open {DATA_P
-00014ad0: 4154 487d 7b6d 6163 726f 5f66 696c 657d  ATH}{macro_file}
-00014ae0: 2229 0a0a 2020 2020 6465 6620 7265 6164  ")..    def read
-00014af0: 5f63 775f 6d61 6372 6f73 2873 656c 6629  _cw_macros(self)
-00014b00: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00014b10: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-00014b20: 6164 7320 696e 2074 6865 2043 5720 6d61  ads in the CW ma
-00014b30: 6372 6f73 2c20 6669 7273 7473 2069 7420  cros, firsts it 
-00014b40: 6368 6563 6b73 2074 6f20 7365 6520 6966  checks to see if
-00014b50: 2074 6865 2066 696c 6520 6578 6973 7473   the file exists
-00014b60: 2e20 4966 2069 7420 646f 6573 206e 6f74  . If it does not
-00014b70: 2c0a 2020 2020 2020 2020 616e 6420 7468  ,.        and th
-00014b80: 6973 2068 6173 2062 6565 6e20 7061 636b  is has been pack
-00014b90: 6167 6564 2077 6974 6820 7079 696e 7374  aged with pyinst
-00014ba0: 616c 6c65 7220 6974 2077 696c 6c20 636f  aller it will co
-00014bb0: 7079 2074 6865 2064 6566 6175 6c74 2066  py the default f
-00014bc0: 696c 6520 6672 6f6d 2074 6865 0a20 2020  ile from the.   
-00014bd0: 2020 2020 2074 656d 7020 6469 7265 6374       temp direct
-00014be0: 6f72 7920 7468 6973 2069 7320 7275 6e6e  ory this is runn
-00014bf0: 696e 6720 6672 6f6d 2e2e 2e20 496e 2074  ing from... In t
-00014c00: 6865 6f72 792e 0a20 2020 2020 2020 2022  heory..        "
-00014c10: 2222 0a0a 2020 2020 2020 2020 6966 2073  ""..        if s
-00014c20: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-00014c30: 6765 7428 226d 6f64 6522 2920 3d3d 2022  get("mode") == "
-00014c40: 4357 223a 0a20 2020 2020 2020 2020 2020  CW":.           
-00014c50: 206d 6163 726f 5f66 696c 6520 3d20 222f   macro_file = "/
-00014c60: 6377 6d61 6372 6f73 2e74 7874 220a 2020  cwmacros.txt".  
-00014c70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00014c80: 2020 2020 2020 2020 6d61 6372 6f5f 6669          macro_fi
-00014c90: 6c65 203d 2022 2f73 7362 6d61 6372 6f73  le = "/ssbmacros
-00014ca0: 2e74 7874 220a 0a20 2020 2020 2020 2069  .txt"..        i
-00014cb0: 6620 6e6f 7420 5061 7468 2844 4154 415f  f not Path(DATA_
-00014cc0: 5041 5448 202b 206d 6163 726f 5f66 696c  PATH + macro_fil
-00014cd0: 6529 2e65 7869 7374 7328 293a 0a20 2020  e).exists():.   
-00014ce0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00014cf0: 6465 6275 6728 2272 6561 645f 6377 5f6d  debug("read_cw_m
-00014d00: 6163 726f 733a 2063 6f70 7969 6e67 2064  acros: copying d
-00014d10: 6566 6175 6c74 206d 6163 726f 2066 696c  efault macro fil
-00014d20: 652e 2229 0a20 2020 2020 2020 2020 2020  e.").           
-00014d30: 2063 6f70 7966 696c 6528 574f 524b 494e   copyfile(WORKIN
-00014d40: 475f 5041 5448 202b 2022 2f64 6174 6122  G_PATH + "/data"
-00014d50: 202b 206d 6163 726f 5f66 696c 652c 2044   + macro_file, D
-00014d60: 4154 415f 5041 5448 202b 206d 6163 726f  ATA_PATH + macro
-00014d70: 5f66 696c 6529 0a20 2020 2020 2020 2077  _file).        w
-00014d80: 6974 6820 6f70 656e 2844 4154 415f 5041  ith open(DATA_PA
-00014d90: 5448 202b 206d 6163 726f 5f66 696c 652c  TH + macro_file,
-00014da0: 2022 7222 2c20 656e 636f 6469 6e67 3d22   "r", encoding="
-00014db0: 7574 662d 3822 2920 6173 2066 696c 655f  utf-8") as file_
-00014dc0: 6465 7363 7269 7074 6f72 3a0a 2020 2020  descriptor:.    
-00014dd0: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
-00014de0: 2069 6e20 6669 6c65 5f64 6573 6372 6970   in file_descrip
-00014df0: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
-00014e00: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00014e10: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-00014e20: 6465 2c20 666b 6579 2c20 6275 7474 6f6e  de, fkey, button
-00014e30: 6e61 6d65 2c20 6377 7465 7874 203d 206c  name, cwtext = l
-00014e40: 696e 652e 7370 6c69 7428 227c 2229 0a20  ine.split("|"). 
-00014e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e60: 2020 2069 6620 6d6f 6465 2e73 7472 6970     if mode.strip
-00014e70: 2829 2e75 7070 6572 2829 203d 3d20 2252  ().upper() == "R
-00014e80: 2220 616e 6420 7365 6c66 2e70 7265 662e  " and self.pref.
-00014e90: 6765 7428 2272 756e 5f73 7461 7465 2229  get("run_state")
-00014ea0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014eb0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-00014ec0: 6b65 7973 5b66 6b65 792e 7374 7269 7028  keys[fkey.strip(
-00014ed0: 295d 203d 2028 6275 7474 6f6e 6e61 6d65  )] = (buttonname
-00014ee0: 2e73 7472 6970 2829 2c20 6377 7465 7874  .strip(), cwtext
-00014ef0: 2e73 7472 6970 2829 290a 2020 2020 2020  .strip()).      
-00014f00: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014f10: 206d 6f64 652e 7374 7269 7028 292e 7570   mode.strip().up
-00014f20: 7065 7228 2920 213d 2022 5222 2061 6e64  per() != "R" and
-00014f30: 206e 6f74 2073 656c 662e 7072 6566 2e67   not self.pref.g
-00014f40: 6574 2822 7275 6e5f 7374 6174 6522 293a  et("run_state"):
-00014f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014f60: 2020 2020 2020 2020 2073 656c 662e 666b           self.fk
-00014f70: 6579 735b 666b 6579 2e73 7472 6970 2829  eys[fkey.strip()
-00014f80: 5d20 3d20 2862 7574 746f 6e6e 616d 652e  ] = (buttonname.
-00014f90: 7374 7269 7028 292c 2063 7774 6578 742e  strip(), cwtext.
-00014fa0: 7374 7269 7028 2929 0a20 2020 2020 2020  strip()).       
-00014fb0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00014fc0: 5661 6c75 6545 7272 6f72 2061 7320 6572  ValueError as er
-00014fd0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00014fe0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00014ff0: 666f 2822 7265 6164 5f63 775f 6d61 6372  fo("read_cw_macr
-00015000: 6f73 3a20 2573 222c 2065 7272 290a 2020  os: %s", err).  
-00015010: 2020 2020 2020 6b65 7973 203d 2073 656c        keys = sel
-00015020: 662e 666b 6579 732e 6b65 7973 2829 0a20  f.fkeys.keys(). 
-00015030: 2020 2020 2020 2069 6620 2246 3122 2069         if "F1" i
-00015040: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
-00015050: 2020 2020 7365 6c66 2e46 312e 7365 7454      self.F1.setT
-00015060: 6578 7428 6622 4631 3a20 7b73 656c 662e  ext(f"F1: {self.
-00015070: 666b 6579 735b 2746 3127 5d5b 305d 7d22  fkeys['F1'][0]}"
-00015080: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00015090: 6c66 2e46 312e 7365 7454 6f6f 6c54 6970  lf.F1.setToolTip
-000150a0: 2873 656c 662e 666b 6579 735b 2246 3122  (self.fkeys["F1"
-000150b0: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
-000150c0: 2022 4632 2220 696e 206b 6579 733a 0a20   "F2" in keys:. 
-000150d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000150e0: 4632 2e73 6574 5465 7874 2866 2246 323a  F2.setText(f"F2:
-000150f0: 207b 7365 6c66 2e66 6b65 7973 5b27 4632   {self.fkeys['F2
-00015100: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
-00015110: 2020 2020 2073 656c 662e 4632 2e73 6574       self.F2.set
-00015120: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
-00015130: 7973 5b22 4632 225d 5b31 5d29 0a20 2020  ys["F2"][1]).   
-00015140: 2020 2020 2069 6620 2246 3322 2069 6e20       if "F3" in 
-00015150: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-00015160: 2020 7365 6c66 2e46 332e 7365 7454 6578    self.F3.setTex
-00015170: 7428 6622 4633 3a20 7b73 656c 662e 666b  t(f"F3: {self.fk
-00015180: 6579 735b 2746 3327 5d5b 305d 7d22 290a  eys['F3'][0]}").
-00015190: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000151a0: 2e46 332e 7365 7454 6f6f 6c54 6970 2873  .F3.setToolTip(s
-000151b0: 656c 662e 666b 6579 735b 2246 3322 5d5b  elf.fkeys["F3"][
-000151c0: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
-000151d0: 4634 2220 696e 206b 6579 733a 0a20 2020  F4" in keys:.   
-000151e0: 2020 2020 2020 2020 2073 656c 662e 4634           self.F4
-000151f0: 2e73 6574 5465 7874 2866 2246 343a 207b  .setText(f"F4: {
-00015200: 7365 6c66 2e66 6b65 7973 5b27 4634 275d  self.fkeys['F4']
-00015210: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
-00015220: 2020 2073 656c 662e 4634 2e73 6574 546f     self.F4.setTo
-00015230: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
-00015240: 5b22 4634 225d 5b31 5d29 0a20 2020 2020  ["F4"][1]).     
-00015250: 2020 2069 6620 2246 3522 2069 6e20 6b65     if "F5" in ke
-00015260: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-00015270: 7365 6c66 2e46 352e 7365 7454 6578 7428  self.F5.setText(
-00015280: 6622 4635 3a20 7b73 656c 662e 666b 6579  f"F5: {self.fkey
-00015290: 735b 2746 3527 5d5b 305d 7d22 290a 2020  s['F5'][0]}").  
-000152a0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-000152b0: 352e 7365 7454 6f6f 6c54 6970 2873 656c  5.setToolTip(sel
-000152c0: 662e 666b 6579 735b 2246 3522 5d5b 315d  f.fkeys["F5"][1]
-000152d0: 290a 2020 2020 2020 2020 6966 2022 4636  ).        if "F6
-000152e0: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
-000152f0: 2020 2020 2020 2073 656c 662e 4636 2e73         self.F6.s
-00015300: 6574 5465 7874 2866 2246 363a 207b 7365  etText(f"F6: {se
-00015310: 6c66 2e66 6b65 7973 5b27 4636 275d 5b30  lf.fkeys['F6'][0
-00015320: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
-00015330: 2073 656c 662e 4636 2e73 6574 546f 6f6c   self.F6.setTool
-00015340: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
-00015350: 4636 225d 5b31 5d29 0a20 2020 2020 2020  F6"][1]).       
-00015360: 2069 6620 2246 3722 2069 6e20 6b65 7973   if "F7" in keys
-00015370: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00015380: 6c66 2e46 372e 7365 7454 6578 7428 6622  lf.F7.setText(f"
-00015390: 4637 3a20 7b73 656c 662e 666b 6579 735b  F7: {self.fkeys[
-000153a0: 2746 3727 5d5b 305d 7d22 290a 2020 2020  'F7'][0]}").    
-000153b0: 2020 2020 2020 2020 7365 6c66 2e46 372e          self.F7.
-000153c0: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
-000153d0: 666b 6579 735b 2246 3722 5d5b 315d 290a  fkeys["F7"][1]).
-000153e0: 2020 2020 2020 2020 6966 2022 4638 2220          if "F8" 
-000153f0: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
-00015400: 2020 2020 2073 656c 662e 4638 2e73 6574       self.F8.set
-00015410: 5465 7874 2866 2246 383a 207b 7365 6c66  Text(f"F8: {self
-00015420: 2e66 6b65 7973 5b27 4638 275d 5b30 5d7d  .fkeys['F8'][0]}
-00015430: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-00015440: 656c 662e 4638 2e73 6574 546f 6f6c 5469  elf.F8.setToolTi
-00015450: 7028 7365 6c66 2e66 6b65 7973 5b22 4638  p(self.fkeys["F8
-00015460: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
-00015470: 6620 2246 3922 2069 6e20 6b65 7973 3a0a  f "F9" in keys:.
-00015480: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015490: 2e46 392e 7365 7454 6578 7428 6622 4639  .F9.setText(f"F9
-000154a0: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
-000154b0: 3927 5d5b 305d 7d22 290a 2020 2020 2020  9'][0]}").      
-000154c0: 2020 2020 2020 7365 6c66 2e46 392e 7365        self.F9.se
-000154d0: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
-000154e0: 6579 735b 2246 3922 5d5b 315d 290a 2020  eys["F9"][1]).  
-000154f0: 2020 2020 2020 6966 2022 4631 3022 2069        if "F10" i
-00015500: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
-00015510: 2020 2020 7365 6c66 2e46 3130 2e73 6574      self.F10.set
-00015520: 5465 7874 2866 2246 3130 3a20 7b73 656c  Text(f"F10: {sel
-00015530: 662e 666b 6579 735b 2746 3130 275d 5b30  f.fkeys['F10'][0
-00015540: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
-00015550: 2073 656c 662e 4631 302e 7365 7454 6f6f   self.F10.setToo
-00015560: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
-00015570: 2246 3130 225d 5b31 5d29 0a20 2020 2020  "F10"][1]).     
-00015580: 2020 2069 6620 2246 3131 2220 696e 206b     if "F11" in k
-00015590: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
-000155a0: 2073 656c 662e 4631 312e 7365 7454 6578   self.F11.setTex
-000155b0: 7428 6622 4631 313a 207b 7365 6c66 2e66  t(f"F11: {self.f
-000155c0: 6b65 7973 5b27 4631 3127 5d5b 305d 7d22  keys['F11'][0]}"
-000155d0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000155e0: 6c66 2e46 3131 2e73 6574 546f 6f6c 5469  lf.F11.setToolTi
-000155f0: 7028 7365 6c66 2e66 6b65 7973 5b22 4631  p(self.fkeys["F1
-00015600: 3122 5d5b 315d 290a 2020 2020 2020 2020  1"][1]).        
-00015610: 6966 2022 4631 3222 2069 6e20 6b65 7973  if "F12" in keys
-00015620: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00015630: 6c66 2e46 3132 2e73 6574 5465 7874 2866  lf.F12.setText(f
-00015640: 2246 3132 3a20 7b73 656c 662e 666b 6579  "F12: {self.fkey
-00015650: 735b 2746 3132 275d 5b30 5d7d 2229 0a20  s['F12'][0]}"). 
-00015660: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015670: 4631 322e 7365 7454 6f6f 6c54 6970 2873  F12.setToolTip(s
-00015680: 656c 662e 666b 6579 735b 2246 3132 225d  elf.fkeys["F12"]
-00015690: 5b31 5d29 0a0a 2020 2020 6465 6620 6765  [1])..    def ge
-000156a0: 6e65 7261 7465 5f61 6469 6628 7365 6c66  nerate_adif(self
-000156b0: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-000156c0: 6e65 7261 7465 2041 4449 4622 2222 0a20  nerate ADIF""". 
-000156d0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-000156e0: 6275 6728 222a 2a2a 2a2a 2a41 4449 462a  bug("******ADIF*
-000156f0: 2a2a 2a2a 2229 0a20 2020 2020 2020 2073  ****").        s
-00015700: 656c 662e 636f 6e74 6573 742e 6164 6966  elf.contest.adif
-00015710: 2873 656c 6629 0a0a 2020 2020 6465 6620  (self)..    def 
-00015720: 6765 6e65 7261 7465 5f63 6162 7269 6c6c  generate_cabrill
-00015730: 6f28 7365 6c66 293a 0a20 2020 2020 2020  o(self):.       
-00015740: 2022 2222 4765 6e65 7261 7465 7320 4361   """Generates Ca
-00015750: 6272 696c 6c6f 2066 696c 652e 204d 6179  brillo file. May
-00015760: 6265 2e22 2222 0a20 2020 2020 2020 2023  be.""".        #
-00015770: 2068 7474 7073 3a2f 2f77 7777 2e63 7177   https://www.cqw
-00015780: 7078 2e63 6f6d 2f63 6162 7269 6c6c 6f2e  px.com/cabrillo.
-00015790: 6874 6d0a 2020 2020 2020 2020 6c6f 6767  htm.        logg
-000157a0: 6572 2e64 6562 7567 2822 2a2a 2a2a 2a2a  er.debug("******
-000157b0: 4361 6272 696c 6c6f 2a2a 2a2a 2a22 290a  Cabrillo*****").
-000157c0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000157d0: 7465 7374 2e63 6162 7269 6c6c 6f28 7365  test.cabrillo(se
-000157e0: 6c66 290a 0a0a 6465 6620 6c6f 6164 5f66  lf)...def load_f
-000157f0: 6f6e 7473 5f66 726f 6d5f 6469 7228 6469  onts_from_dir(di
-00015800: 7265 6374 6f72 793a 2073 7472 2920 2d3e  rectory: str) ->
-00015810: 2073 6574 3a0a 2020 2020 2222 220a 2020   set:.    """.  
-00015820: 2020 5765 6c6c 2069 7420 6c6f 6164 7320    Well it loads 
-00015830: 666f 6e74 7320 6672 6f6d 2061 2064 6972  fonts from a dir
-00015840: 6563 746f 7279 2e2e 2e0a 2020 2020 2222  ectory....    ""
-00015850: 220a 2020 2020 666f 6e74 5f66 616d 696c  ".    font_famil
-00015860: 6965 7320 3d20 7365 7428 290a 2020 2020  ies = set().    
-00015870: 666f 7220 5f66 6920 696e 2051 4469 7228  for _fi in QDir(
-00015880: 6469 7265 6374 6f72 7929 2e65 6e74 7279  directory).entry
-00015890: 496e 666f 4c69 7374 285b 222a 2e74 7466  InfoList(["*.ttf
-000158a0: 222c 2022 2a2e 776f 6666 222c 2022 2a2e  ", "*.woff", "*.
-000158b0: 776f 6666 3222 5d29 3a0a 2020 2020 2020  woff2"]):.      
-000158c0: 2020 5f69 6420 3d20 5146 6f6e 7444 6174    _id = QFontDat
-000158d0: 6162 6173 652e 6164 6441 7070 6c69 6361  abase.addApplica
-000158e0: 7469 6f6e 466f 6e74 285f 6669 2e61 6273  tionFont(_fi.abs
-000158f0: 6f6c 7574 6546 696c 6550 6174 6828 2929  oluteFilePath())
-00015900: 0a20 2020 2020 2020 2066 6f6e 745f 6661  .        font_fa
-00015910: 6d69 6c69 6573 207c 3d20 7365 7428 5146  milies |= set(QF
-00015920: 6f6e 7444 6174 6162 6173 652e 6170 706c  ontDatabase.appl
-00015930: 6963 6174 696f 6e46 6f6e 7446 616d 696c  icationFontFamil
-00015940: 6965 7328 5f69 6429 290a 2020 2020 7265  ies(_id)).    re
-00015950: 7475 726e 2066 6f6e 745f 6661 6d69 6c69  turn font_famili
-00015960: 6573 0a0a 0a64 6566 2069 6e73 7461 6c6c  es...def install
-00015970: 5f69 636f 6e73 2829 3a0a 2020 2020 2222  _icons():.    ""
-00015980: 2249 6e73 7461 6c6c 2069 636f 6e73 2222  "Install icons""
-00015990: 220a 2020 2020 6f73 2e73 7973 7465 6d28  ".    os.system(
-000159a0: 0a20 2020 2020 2020 2022 7864 672d 6963  .        "xdg-ic
-000159b0: 6f6e 2d72 6573 6f75 7263 6520 696e 7374  on-resource inst
-000159c0: 616c 6c20 2d2d 7369 7a65 2033 3220 2d2d  all --size 32 --
-000159d0: 636f 6e74 6578 7420 6170 7073 202d 2d6d  context apps --m
-000159e0: 6f64 6520 7573 6572 2022 0a20 2020 2020  ode user ".     
-000159f0: 2020 2066 227b 574f 524b 494e 475f 5041     f"{WORKING_PA
-00015a00: 5448 7d2f 6461 7461 2f6b 3667 7465 2e6e  TH}/data/k6gte.n
-00015a10: 6f74 316d 6d2d 3332 2e70 6e67 206b 3667  ot1mm-32.png k6g
-00015a20: 7465 2d6e 6f74 316d 6d22 0a20 2020 2029  te-not1mm".    )
-00015a30: 0a20 2020 206f 732e 7379 7374 656d 280a  .    os.system(.
-00015a40: 2020 2020 2020 2020 2278 6467 2d69 636f          "xdg-ico
-00015a50: 6e2d 7265 736f 7572 6365 2069 6e73 7461  n-resource insta
-00015a60: 6c6c 202d 2d73 697a 6520 3634 202d 2d63  ll --size 64 --c
-00015a70: 6f6e 7465 7874 2061 7070 7320 2d2d 6d6f  ontext apps --mo
-00015a80: 6465 2075 7365 7220 220a 2020 2020 2020  de user ".      
-00015a90: 2020 6622 7b57 4f52 4b49 4e47 5f50 4154    f"{WORKING_PAT
-00015aa0: 487d 2f64 6174 612f 6b36 6774 652e 6e6f  H}/data/k6gte.no
-00015ab0: 7431 6d6d 2d36 342e 706e 6720 6b36 6774  t1mm-64.png k6gt
-00015ac0: 652d 6e6f 7431 6d6d 220a 2020 2020 290a  e-not1mm".    ).
-00015ad0: 2020 2020 6f73 2e73 7973 7465 6d28 0a20      os.system(. 
-00015ae0: 2020 2020 2020 2022 7864 672d 6963 6f6e         "xdg-icon
-00015af0: 2d72 6573 6f75 7263 6520 696e 7374 616c  -resource instal
-00015b00: 6c20 2d2d 7369 7a65 2031 3238 202d 2d63  l --size 128 --c
-00015b10: 6f6e 7465 7874 2061 7070 7320 2d2d 6d6f  ontext apps --mo
-00015b20: 6465 2075 7365 7220 220a 2020 2020 2020  de user ".      
-00015b30: 2020 6622 7b57 4f52 4b49 4e47 5f50 4154    f"{WORKING_PAT
-00015b40: 487d 2f64 6174 612f 6b36 6774 652e 6e6f  H}/data/k6gte.no
-00015b50: 7431 6d6d 2d31 3238 2e70 6e67 206b 3667  t1mm-128.png k6g
-00015b60: 7465 2d6e 6f74 316d 6d22 0a20 2020 2029  te-not1mm".    )
-00015b70: 0a20 2020 206f 732e 7379 7374 656d 2866  .    os.system(f
-00015b80: 2278 6467 2d64 6573 6b74 6f70 2d6d 656e  "xdg-desktop-men
-00015b90: 7520 696e 7374 616c 6c20 7b57 4f52 4b49  u install {WORKI
-00015ba0: 4e47 5f50 4154 487d 2f64 6174 612f 6b36  NG_PATH}/data/k6
-00015bb0: 6774 652d 6e6f 7431 6d6d 2e64 6573 6b74  gte-not1mm.deskt
-00015bc0: 6f70 2229 0a0a 0a64 6566 2064 6f69 6d70  op")...def doimp
-00015bd0: 286d 6f64 6e61 6d65 293a 0a20 2020 2022  (modname):.    "
-00015be0: 2222 7265 7475 726e 206d 6f64 756c 6520  ""return module 
-00015bf0: 7061 7468 2222 220a 2020 2020 7265 7475  path""".    retu
-00015c00: 726e 2069 6d70 6f72 746c 6962 2e69 6d70  rn importlib.imp
-00015c10: 6f72 745f 6d6f 6475 6c65 2866 226e 6f74  ort_module(f"not
-00015c20: 316d 6d2e 706c 7567 696e 732e 7b6d 6f64  1mm.plugins.{mod
-00015c30: 6e61 6d65 7d22 290a 0a0a 6465 6620 7275  name}")...def ru
-00015c40: 6e28 293a 0a20 2020 2022 2222 0a20 2020  n():.    """.   
-00015c50: 204d 6169 6e20 456e 7472 790a 2020 2020   Main Entry.    
-00015c60: 2222 220a 2020 2020 696e 7374 616c 6c5f  """.    install_
-00015c70: 6963 6f6e 7328 290a 2020 2020 7469 6d65  icons().    time
-00015c80: 722e 7374 6172 7428 3235 3029 0a20 2020  r.start(250).   
-00015c90: 2073 7973 2e65 7869 7428 6170 702e 6578   sys.exit(app.ex
-00015ca0: 6563 2829 290a 0a0a 6c6f 6767 6572 203d  ec())...logger =
-00015cb0: 206c 6f67 6769 6e67 2e67 6574 4c6f 6767   logging.getLogg
-00015cc0: 6572 2822 5f5f 6d61 696e 5f5f 2229 0a68  er("__main__").h
-00015cd0: 616e 646c 6572 203d 206c 6f67 6769 6e67  andler = logging
-00015ce0: 2e53 7472 6561 6d48 616e 646c 6572 2829  .StreamHandler()
-00015cf0: 0a66 6f72 6d61 7474 6572 203d 206c 6f67  .formatter = log
-00015d00: 6769 6e67 2e46 6f72 6d61 7474 6572 280a  ging.Formatter(.
-00015d10: 2020 2020 6461 7465 666d 743d 2225 483a      datefmt="%H:
-00015d20: 254d 3a25 5322 2c0a 2020 2020 666d 743d  %M:%S",.    fmt=
-00015d30: 225b 2528 6173 6374 696d 6529 735d 2025  "[%(asctime)s] %
-00015d40: 286c 6576 656c 6e61 6d65 2973 2025 286d  (levelname)s %(m
-00015d50: 6f64 756c 6529 7320 2d20 2528 6675 6e63  odule)s - %(func
-00015d60: 4e61 6d65 2973 204c 696e 6520 2528 6c69  Name)s Line %(li
-00015d70: 6e65 6e6f 2964 3a20 2528 6d65 7373 6167  neno)d: %(messag
-00015d80: 6529 7322 2c0a 290a 6861 6e64 6c65 722e  e)s",.).handler.
-00015d90: 7365 7446 6f72 6d61 7474 6572 2866 6f72  setFormatter(for
-00015da0: 6d61 7474 6572 290a 6c6f 6767 6572 2e61  matter).logger.a
-00015db0: 6464 4861 6e64 6c65 7228 6861 6e64 6c65  ddHandler(handle
-00015dc0: 7229 0a0a 4245 5441 5f54 4553 5420 3d20  r)..BETA_TEST = 
-00015dd0: 4661 6c73 650a 6966 2050 6174 6828 222e  False.if Path(".
-00015de0: 2f62 6574 6174 6573 7422 292e 6578 6973  /betatest").exis
-00015df0: 7473 2829 3a0a 2020 2020 4245 5441 5f54  ts():.    BETA_T
-00015e00: 4553 5420 3d20 5472 7565 0a0a 6966 2050  EST = True..if P
-00015e10: 6174 6828 222e 2f64 6562 7567 2229 2e65  ath("./debug").e
-00015e20: 7869 7374 7328 293a 0a20 2020 206c 6f67  xists():.    log
-00015e30: 6765 722e 7365 744c 6576 656c 286c 6f67  ger.setLevel(log
-00015e40: 6769 6e67 2e44 4542 5547 290a 2020 2020  ging.DEBUG).    
-00015e50: 6c6f 6767 6572 2e64 6562 7567 2822 6465  logger.debug("de
-00015e60: 6275 6767 696e 6720 6f6e 2229 0a65 6c73  bugging on").els
-00015e70: 653a 0a20 2020 206c 6f67 6765 722e 7365  e:.    logger.se
-00015e80: 744c 6576 656c 286c 6f67 6769 6e67 2e57  tLevel(logging.W
-00015e90: 4152 4e49 4e47 290a 2020 2020 6c6f 6767  ARNING).    logg
-00015ea0: 6572 2e77 6172 6e69 6e67 2822 6465 6275  er.warning("debu
-00015eb0: 6767 696e 6720 6f66 6622 290a 0a61 7070  gging off")..app
-00015ec0: 203d 2051 7457 6964 6765 7473 2e51 4170   = QtWidgets.QAp
-00015ed0: 706c 6963 6174 696f 6e28 7379 732e 6172  plication(sys.ar
-00015ee0: 6776 290a 6170 702e 7365 7453 7479 6c65  gv).app.setStyle
-00015ef0: 2822 4164 7761 6974 612d 4461 726b 2229  ("Adwaita-Dark")
-00015f00: 0a66 6f6e 745f 7061 7468 203d 2057 4f52  .font_path = WOR
-00015f10: 4b49 4e47 5f50 4154 4820 2b20 222f 6461  KING_PATH + "/da
-00015f20: 7461 220a 6661 6d69 6c69 6573 203d 206c  ta".families = l
-00015f30: 6f61 645f 666f 6e74 735f 6672 6f6d 5f64  oad_fonts_from_d
-00015f40: 6972 286f 732e 6673 7061 7468 2866 6f6e  ir(os.fspath(fon
-00015f50: 745f 7061 7468 2929 0a6c 6f67 6765 722e  t_path)).logger.
-00015f60: 696e 666f 2866 616d 696c 6965 7329 0a77  info(families).w
-00015f70: 696e 646f 7720 3d20 4d61 696e 5769 6e64  indow = MainWind
-00015f80: 6f77 2829 0a68 6569 6768 7420 3d20 7769  ow().height = wi
-00015f90: 6e64 6f77 2e70 7265 662e 6765 7428 2277  ndow.pref.get("w
-00015fa0: 696e 646f 775f 6865 6967 6874 222c 2033  indow_height", 3
-00015fb0: 3030 290a 7769 6474 6820 3d20 7769 6e64  00).width = wind
-00015fc0: 6f77 2e70 7265 662e 6765 7428 2277 696e  ow.pref.get("win
-00015fd0: 646f 775f 7769 6474 6822 2c20 3730 3029  dow_width", 700)
-00015fe0: 0a78 203d 2077 696e 646f 772e 7072 6566  .x = window.pref
-00015ff0: 2e67 6574 2822 7769 6e64 6f77 5f78 222c  .get("window_x",
-00016000: 202d 3129 0a79 203d 2077 696e 646f 772e   -1).y = window.
-00016010: 7072 6566 2e67 6574 2822 7769 6e64 6f77  pref.get("window
-00016020: 5f79 222c 202d 3129 0a77 696e 646f 772e  _y", -1).window.
-00016030: 7365 7447 656f 6d65 7472 7928 782c 2079  setGeometry(x, y
-00016040: 2c20 7769 6474 682c 2068 6569 6768 7429  , width, height)
-00016050: 0a77 696e 646f 772e 6361 6c6c 7369 676e  .window.callsign
-00016060: 2e73 6574 466f 6375 7328 290a 7769 6e64  .setFocus().wind
-00016070: 6f77 2e73 686f 7728 290a 7469 6d65 7220  ow.show().timer 
-00016080: 3d20 5174 436f 7265 2e51 5469 6d65 7228  = QtCore.QTimer(
-00016090: 290a 7469 6d65 722e 7469 6d65 6f75 742e  ).timer.timeout.
-000160a0: 636f 6e6e 6563 7428 7769 6e64 6f77 2e70  connect(window.p
-000160b0: 6f6c 6c5f 7261 6469 6f29 0a0a 6966 205f  oll_radio)..if _
-000160c0: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
-000160d0: 696e 5f5f 223a 0a20 2020 2072 756e 2829  in__":.    run()
-000160e0: 0a                                       .
+000143f0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+00014400: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+00014410: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+00014420: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014430: 6620 7365 6c66 2e6e 316d 6d3a 0a20 2020  f self.n1mm:.   
+00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014450: 2020 2020 2069 6620 7365 6c66 2e6e 316d       if self.n1m
+00014460: 6d2e 7365 6e64 5f72 6164 696f 5f70 6163  m.send_radio_pac
+00014470: 6b65 7473 3a0a 2020 2020 2020 2020 2020  kets:.          
+00014480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014490: 2020 7365 6c66 2e6e 316d 6d2e 7261 6469    self.n1mm.radi
+000144a0: 6f5f 696e 666f 5b22 4672 6571 225d 203d  o_info["Freq"] =
+000144b0: 2076 666f 5b3a 2d31 5d0a 2020 2020 2020   vfo[:-1].      
+000144c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144d0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+000144e0: 7261 6469 6f5f 696e 666f 5b22 5458 4672  radio_info["TXFr
+000144f0: 6571 225d 203d 2076 666f 5b3a 2d31 5d0a  eq"] = vfo[:-1].
+00014500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014510: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014520: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
+00014530: 5b22 4d6f 6465 225d 203d 206d 6f64 650a  ["Mode"] = mode.
+00014540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014560: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
+00014570: 5b22 4f70 4361 6c6c 225d 203d 2073 656c  ["OpCall"] = sel
+00014580: 662e 6375 7272 656e 745f 6f70 0a20 2020  f.current_op.   
+00014590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145a0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+000145b0: 6d6d 2e72 6164 696f 5f69 6e66 6f5b 2249  mm.radio_info["I
+000145c0: 7352 756e 6e69 6e67 225d 203d 2073 7472  sRunning"] = str
+000145d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000145e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145f0: 2020 7365 6c66 2e70 7265 662e 6765 7428    self.pref.get(
+00014600: 2272 756e 5f73 7461 7465 222c 2046 616c  "run_state", Fal
+00014610: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014630: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014640: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014650: 6c66 2e6e 316d 6d2e 7365 6e64 5f72 6164  lf.n1mm.send_rad
+00014660: 696f 2829 0a20 2020 2020 2020 2020 2020  io().           
+00014670: 2020 2020 2020 2020 2067 6c6f 6261 6c73           globals
+00014680: 2829 5b22 706f 6c6c 5f74 696d 6522 5d20  ()["poll_time"] 
+00014690: 3d20 6461 7465 7469 6d65 2e6e 6f77 2829  = datetime.now()
+000146a0: 202b 2064 742e 7469 6d65 6465 6c74 6128   + dt.timedelta(
+000146b0: 7365 636f 6e64 733d 3130 290a 0a20 2020  seconds=10)..   
+000146c0: 2064 6566 2065 6469 745f 6377 5f6d 6163   def edit_cw_mac
+000146d0: 726f 7328 7365 6c66 2920 2d3e 204e 6f6e  ros(self) -> Non
+000146e0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+000146f0: 2020 2020 2020 2043 616c 6c73 2074 6865         Calls the
+00014700: 2064 6566 6175 6c74 2074 6578 7420 6564   default text ed
+00014710: 6974 6f72 2074 6f20 6564 6974 2074 6865  itor to edit the
+00014720: 2043 5720 6d61 6372 6f20 6669 6c65 2e0a   CW macro file..
+00014730: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014740: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
+00014750: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
+00014760: 6522 2920 3d3d 2022 4357 223a 0a20 2020  e") == "CW":.   
+00014770: 2020 2020 2020 2020 206d 6163 726f 5f66           macro_f
+00014780: 696c 6520 3d20 222f 6377 6d61 6372 6f73  ile = "/cwmacros
+00014790: 2e74 7874 220a 2020 2020 2020 2020 656c  .txt".        el
+000147a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000147b0: 6d61 6372 6f5f 6669 6c65 203d 2022 2f73  macro_file = "/s
+000147c0: 7362 6d61 6372 6f73 2e74 7874 220a 2020  sbmacros.txt".  
+000147d0: 2020 2020 2020 6966 206e 6f74 2050 6174        if not Pat
+000147e0: 6828 4441 5441 5f50 4154 4820 2b20 6d61  h(DATA_PATH + ma
+000147f0: 6372 6f5f 6669 6c65 292e 6578 6973 7473  cro_file).exists
+00014800: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00014810: 6c6f 6767 6572 2e64 6562 7567 2822 7265  logger.debug("re
+00014820: 6164 5f63 775f 6d61 6372 6f73 3a20 636f  ad_cw_macros: co
+00014830: 7079 696e 6720 6465 6661 756c 7420 6d61  pying default ma
+00014840: 6372 6f20 6669 6c65 2e22 290a 2020 2020  cro file.").    
+00014850: 2020 2020 2020 2020 636f 7079 6669 6c65          copyfile
+00014860: 2857 4f52 4b49 4e47 5f50 4154 4820 2b20  (WORKING_PATH + 
+00014870: 222f 6461 7461 2220 2b20 6d61 6372 6f5f  "/data" + macro_
+00014880: 6669 6c65 2c20 4441 5441 5f50 4154 4820  file, DATA_PATH 
+00014890: 2b20 6d61 6372 6f5f 6669 6c65 290a 2020  + macro_file).  
+000148a0: 2020 2020 2020 6f73 2e73 7973 7465 6d28        os.system(
+000148b0: 6622 7864 672d 6f70 656e 207b 4441 5441  f"xdg-open {DATA
+000148c0: 5f50 4154 487d 7b6d 6163 726f 5f66 696c  _PATH}{macro_fil
+000148d0: 657d 2229 0a0a 2020 2020 6465 6620 7265  e}")..    def re
+000148e0: 6164 5f63 775f 6d61 6372 6f73 2873 656c  ad_cw_macros(sel
+000148f0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00014900: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014910: 5265 6164 7320 696e 2074 6865 2043 5720  Reads in the CW 
+00014920: 6d61 6372 6f73 2c20 6669 7273 7473 2069  macros, firsts i
+00014930: 7420 6368 6563 6b73 2074 6f20 7365 6520  t checks to see 
+00014940: 6966 2074 6865 2066 696c 6520 6578 6973  if the file exis
+00014950: 7473 2e20 4966 2069 7420 646f 6573 206e  ts. If it does n
+00014960: 6f74 2c0a 2020 2020 2020 2020 616e 6420  ot,.        and 
+00014970: 7468 6973 2068 6173 2062 6565 6e20 7061  this has been pa
+00014980: 636b 6167 6564 2077 6974 6820 7079 696e  ckaged with pyin
+00014990: 7374 616c 6c65 7220 6974 2077 696c 6c20  staller it will 
+000149a0: 636f 7079 2074 6865 2064 6566 6175 6c74  copy the default
+000149b0: 2066 696c 6520 6672 6f6d 2074 6865 0a20   file from the. 
+000149c0: 2020 2020 2020 2074 656d 7020 6469 7265         temp dire
+000149d0: 6374 6f72 7920 7468 6973 2069 7320 7275  ctory this is ru
+000149e0: 6e6e 696e 6720 6672 6f6d 2e2e 2e20 496e  nning from... In
+000149f0: 2074 6865 6f72 792e 0a20 2020 2020 2020   theory..       
+00014a00: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
+00014a10: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+00014a20: 652e 6765 7428 226d 6f64 6522 2920 3d3d  e.get("mode") ==
+00014a30: 2022 4357 223a 0a20 2020 2020 2020 2020   "CW":.         
+00014a40: 2020 206d 6163 726f 5f66 696c 6520 3d20     macro_file = 
+00014a50: 222f 6377 6d61 6372 6f73 2e74 7874 220a  "/cwmacros.txt".
+00014a60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00014a70: 2020 2020 2020 2020 2020 6d61 6372 6f5f            macro_
+00014a80: 6669 6c65 203d 2022 2f73 7362 6d61 6372  file = "/ssbmacr
+00014a90: 6f73 2e74 7874 220a 0a20 2020 2020 2020  os.txt"..       
+00014aa0: 2069 6620 6e6f 7420 5061 7468 2844 4154   if not Path(DAT
+00014ab0: 415f 5041 5448 202b 206d 6163 726f 5f66  A_PATH + macro_f
+00014ac0: 696c 6529 2e65 7869 7374 7328 293a 0a20  ile).exists():. 
+00014ad0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00014ae0: 722e 6465 6275 6728 2272 6561 645f 6377  r.debug("read_cw
+00014af0: 5f6d 6163 726f 733a 2063 6f70 7969 6e67  _macros: copying
+00014b00: 2064 6566 6175 6c74 206d 6163 726f 2066   default macro f
+00014b10: 696c 652e 2229 0a20 2020 2020 2020 2020  ile.").         
+00014b20: 2020 2063 6f70 7966 696c 6528 574f 524b     copyfile(WORK
+00014b30: 494e 475f 5041 5448 202b 2022 2f64 6174  ING_PATH + "/dat
+00014b40: 6122 202b 206d 6163 726f 5f66 696c 652c  a" + macro_file,
+00014b50: 2044 4154 415f 5041 5448 202b 206d 6163   DATA_PATH + mac
+00014b60: 726f 5f66 696c 6529 0a20 2020 2020 2020  ro_file).       
+00014b70: 2077 6974 6820 6f70 656e 2844 4154 415f   with open(DATA_
+00014b80: 5041 5448 202b 206d 6163 726f 5f66 696c  PATH + macro_fil
+00014b90: 652c 2022 7222 2c20 656e 636f 6469 6e67  e, "r", encoding
+00014ba0: 3d22 7574 662d 3822 2920 6173 2066 696c  ="utf-8") as fil
+00014bb0: 655f 6465 7363 7269 7074 6f72 3a0a 2020  e_descriptor:.  
+00014bc0: 2020 2020 2020 2020 2020 666f 7220 6c69            for li
+00014bd0: 6e65 2069 6e20 6669 6c65 5f64 6573 6372  ne in file_descr
+00014be0: 6970 746f 723a 0a20 2020 2020 2020 2020  iptor:.         
+00014bf0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00014c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c10: 6d6f 6465 2c20 666b 6579 2c20 6275 7474  mode, fkey, butt
+00014c20: 6f6e 6e61 6d65 2c20 6377 7465 7874 203d  onname, cwtext =
+00014c30: 206c 696e 652e 7370 6c69 7428 227c 2229   line.split("|")
+00014c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014c50: 2020 2020 2069 6620 6d6f 6465 2e73 7472       if mode.str
+00014c60: 6970 2829 2e75 7070 6572 2829 203d 3d20  ip().upper() == 
+00014c70: 2252 2220 616e 6420 7365 6c66 2e70 7265  "R" and self.pre
+00014c80: 662e 6765 7428 2272 756e 5f73 7461 7465  f.get("run_state
+00014c90: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00014ca0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014cb0: 2e66 6b65 7973 5b66 6b65 792e 7374 7269  .fkeys[fkey.stri
+00014cc0: 7028 295d 203d 2028 6275 7474 6f6e 6e61  p()] = (buttonna
+00014cd0: 6d65 2e73 7472 6970 2829 2c20 6377 7465  me.strip(), cwte
+00014ce0: 7874 2e73 7472 6970 2829 290a 2020 2020  xt.strip()).    
+00014cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d00: 6966 206d 6f64 652e 7374 7269 7028 292e  if mode.strip().
+00014d10: 7570 7065 7228 2920 213d 2022 5222 2061  upper() != "R" a
+00014d20: 6e64 206e 6f74 2073 656c 662e 7072 6566  nd not self.pref
+00014d30: 2e67 6574 2822 7275 6e5f 7374 6174 6522  .get("run_state"
+00014d40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00014d50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014d60: 666b 6579 735b 666b 6579 2e73 7472 6970  fkeys[fkey.strip
+00014d70: 2829 5d20 3d20 2862 7574 746f 6e6e 616d  ()] = (buttonnam
+00014d80: 652e 7374 7269 7028 292c 2063 7774 6578  e.strip(), cwtex
+00014d90: 742e 7374 7269 7028 2929 0a20 2020 2020  t.strip()).     
+00014da0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00014db0: 7420 5661 6c75 6545 7272 6f72 2061 7320  t ValueError as 
+00014dc0: 6572 723a 0a20 2020 2020 2020 2020 2020  err:.           
+00014dd0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00014de0: 696e 666f 2822 7265 6164 5f63 775f 6d61  info("read_cw_ma
+00014df0: 6372 6f73 3a20 2573 222c 2065 7272 290a  cros: %s", err).
+00014e00: 2020 2020 2020 2020 6b65 7973 203d 2073          keys = s
+00014e10: 656c 662e 666b 6579 732e 6b65 7973 2829  elf.fkeys.keys()
+00014e20: 0a20 2020 2020 2020 2069 6620 2246 3122  .        if "F1"
+00014e30: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
+00014e40: 2020 2020 2020 7365 6c66 2e46 312e 7365        self.F1.se
+00014e50: 7454 6578 7428 6622 4631 3a20 7b73 656c  tText(f"F1: {sel
+00014e60: 662e 666b 6579 735b 2746 3127 5d5b 305d  f.fkeys['F1'][0]
+00014e70: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+00014e80: 7365 6c66 2e46 312e 7365 7454 6f6f 6c54  self.F1.setToolT
+00014e90: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
+00014ea0: 3122 5d5b 315d 290a 2020 2020 2020 2020  1"][1]).        
+00014eb0: 6966 2022 4632 2220 696e 206b 6579 733a  if "F2" in keys:
+00014ec0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00014ed0: 662e 4632 2e73 6574 5465 7874 2866 2246  f.F2.setText(f"F
+00014ee0: 323a 207b 7365 6c66 2e66 6b65 7973 5b27  2: {self.fkeys['
+00014ef0: 4632 275d 5b30 5d7d 2229 0a20 2020 2020  F2'][0]}").     
+00014f00: 2020 2020 2020 2073 656c 662e 4632 2e73         self.F2.s
+00014f10: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
+00014f20: 6b65 7973 5b22 4632 225d 5b31 5d29 0a20  keys["F2"][1]). 
+00014f30: 2020 2020 2020 2069 6620 2246 3322 2069         if "F3" i
+00014f40: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
+00014f50: 2020 2020 7365 6c66 2e46 332e 7365 7454      self.F3.setT
+00014f60: 6578 7428 6622 4633 3a20 7b73 656c 662e  ext(f"F3: {self.
+00014f70: 666b 6579 735b 2746 3327 5d5b 305d 7d22  fkeys['F3'][0]}"
+00014f80: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00014f90: 6c66 2e46 332e 7365 7454 6f6f 6c54 6970  lf.F3.setToolTip
+00014fa0: 2873 656c 662e 666b 6579 735b 2246 3322  (self.fkeys["F3"
+00014fb0: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
+00014fc0: 2022 4634 2220 696e 206b 6579 733a 0a20   "F4" in keys:. 
+00014fd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014fe0: 4634 2e73 6574 5465 7874 2866 2246 343a  F4.setText(f"F4:
+00014ff0: 207b 7365 6c66 2e66 6b65 7973 5b27 4634   {self.fkeys['F4
+00015000: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
+00015010: 2020 2020 2073 656c 662e 4634 2e73 6574       self.F4.set
+00015020: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
+00015030: 7973 5b22 4634 225d 5b31 5d29 0a20 2020  ys["F4"][1]).   
+00015040: 2020 2020 2069 6620 2246 3522 2069 6e20       if "F5" in 
+00015050: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+00015060: 2020 7365 6c66 2e46 352e 7365 7454 6578    self.F5.setTex
+00015070: 7428 6622 4635 3a20 7b73 656c 662e 666b  t(f"F5: {self.fk
+00015080: 6579 735b 2746 3527 5d5b 305d 7d22 290a  eys['F5'][0]}").
+00015090: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000150a0: 2e46 352e 7365 7454 6f6f 6c54 6970 2873  .F5.setToolTip(s
+000150b0: 656c 662e 666b 6579 735b 2246 3522 5d5b  elf.fkeys["F5"][
+000150c0: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
+000150d0: 4636 2220 696e 206b 6579 733a 0a20 2020  F6" in keys:.   
+000150e0: 2020 2020 2020 2020 2073 656c 662e 4636           self.F6
+000150f0: 2e73 6574 5465 7874 2866 2246 363a 207b  .setText(f"F6: {
+00015100: 7365 6c66 2e66 6b65 7973 5b27 4636 275d  self.fkeys['F6']
+00015110: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
+00015120: 2020 2073 656c 662e 4636 2e73 6574 546f     self.F6.setTo
+00015130: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
+00015140: 5b22 4636 225d 5b31 5d29 0a20 2020 2020  ["F6"][1]).     
+00015150: 2020 2069 6620 2246 3722 2069 6e20 6b65     if "F7" in ke
+00015160: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
+00015170: 7365 6c66 2e46 372e 7365 7454 6578 7428  self.F7.setText(
+00015180: 6622 4637 3a20 7b73 656c 662e 666b 6579  f"F7: {self.fkey
+00015190: 735b 2746 3727 5d5b 305d 7d22 290a 2020  s['F7'][0]}").  
+000151a0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
+000151b0: 372e 7365 7454 6f6f 6c54 6970 2873 656c  7.setToolTip(sel
+000151c0: 662e 666b 6579 735b 2246 3722 5d5b 315d  f.fkeys["F7"][1]
+000151d0: 290a 2020 2020 2020 2020 6966 2022 4638  ).        if "F8
+000151e0: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
+000151f0: 2020 2020 2020 2073 656c 662e 4638 2e73         self.F8.s
+00015200: 6574 5465 7874 2866 2246 383a 207b 7365  etText(f"F8: {se
+00015210: 6c66 2e66 6b65 7973 5b27 4638 275d 5b30  lf.fkeys['F8'][0
+00015220: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
+00015230: 2073 656c 662e 4638 2e73 6574 546f 6f6c   self.F8.setTool
+00015240: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
+00015250: 4638 225d 5b31 5d29 0a20 2020 2020 2020  F8"][1]).       
+00015260: 2069 6620 2246 3922 2069 6e20 6b65 7973   if "F9" in keys
+00015270: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00015280: 6c66 2e46 392e 7365 7454 6578 7428 6622  lf.F9.setText(f"
+00015290: 4639 3a20 7b73 656c 662e 666b 6579 735b  F9: {self.fkeys[
+000152a0: 2746 3927 5d5b 305d 7d22 290a 2020 2020  'F9'][0]}").    
+000152b0: 2020 2020 2020 2020 7365 6c66 2e46 392e          self.F9.
+000152c0: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
+000152d0: 666b 6579 735b 2246 3922 5d5b 315d 290a  fkeys["F9"][1]).
+000152e0: 2020 2020 2020 2020 6966 2022 4631 3022          if "F10"
+000152f0: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
+00015300: 2020 2020 2020 7365 6c66 2e46 3130 2e73        self.F10.s
+00015310: 6574 5465 7874 2866 2246 3130 3a20 7b73  etText(f"F10: {s
+00015320: 656c 662e 666b 6579 735b 2746 3130 275d  elf.fkeys['F10']
+00015330: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
+00015340: 2020 2073 656c 662e 4631 302e 7365 7454     self.F10.setT
+00015350: 6f6f 6c54 6970 2873 656c 662e 666b 6579  oolTip(self.fkey
+00015360: 735b 2246 3130 225d 5b31 5d29 0a20 2020  s["F10"][1]).   
+00015370: 2020 2020 2069 6620 2246 3131 2220 696e       if "F11" in
+00015380: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
+00015390: 2020 2073 656c 662e 4631 312e 7365 7454     self.F11.setT
+000153a0: 6578 7428 6622 4631 313a 207b 7365 6c66  ext(f"F11: {self
+000153b0: 2e66 6b65 7973 5b27 4631 3127 5d5b 305d  .fkeys['F11'][0]
+000153c0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+000153d0: 7365 6c66 2e46 3131 2e73 6574 546f 6f6c  self.F11.setTool
+000153e0: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
+000153f0: 4631 3122 5d5b 315d 290a 2020 2020 2020  F11"][1]).      
+00015400: 2020 6966 2022 4631 3222 2069 6e20 6b65    if "F12" in ke
+00015410: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
+00015420: 7365 6c66 2e46 3132 2e73 6574 5465 7874  self.F12.setText
+00015430: 2866 2246 3132 3a20 7b73 656c 662e 666b  (f"F12: {self.fk
+00015440: 6579 735b 2746 3132 275d 5b30 5d7d 2229  eys['F12'][0]}")
+00015450: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00015460: 662e 4631 322e 7365 7454 6f6f 6c54 6970  f.F12.setToolTip
+00015470: 2873 656c 662e 666b 6579 735b 2246 3132  (self.fkeys["F12
+00015480: 225d 5b31 5d29 0a0a 2020 2020 6465 6620  "][1])..    def 
+00015490: 6765 6e65 7261 7465 5f61 6469 6628 7365  generate_adif(se
+000154a0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000154b0: 4765 6e65 7261 7465 2041 4449 4622 2222  Generate ADIF"""
+000154c0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+000154d0: 6465 6275 6728 222a 2a2a 2a2a 2a41 4449  debug("******ADI
+000154e0: 462a 2a2a 2a2a 2229 0a20 2020 2020 2020  F*****").       
+000154f0: 2073 656c 662e 636f 6e74 6573 742e 6164   self.contest.ad
+00015500: 6966 2873 656c 6629 0a0a 2020 2020 6465  if(self)..    de
+00015510: 6620 6765 6e65 7261 7465 5f63 6162 7269  f generate_cabri
+00015520: 6c6c 6f28 7365 6c66 293a 0a20 2020 2020  llo(self):.     
+00015530: 2020 2022 2222 4765 6e65 7261 7465 7320     """Generates 
+00015540: 4361 6272 696c 6c6f 2066 696c 652e 204d  Cabrillo file. M
+00015550: 6179 6265 2e22 2222 0a20 2020 2020 2020  aybe.""".       
+00015560: 2023 2068 7474 7073 3a2f 2f77 7777 2e63   # https://www.c
+00015570: 7177 7078 2e63 6f6d 2f63 6162 7269 6c6c  qwpx.com/cabrill
+00015580: 6f2e 6874 6d0a 2020 2020 2020 2020 6c6f  o.htm.        lo
+00015590: 6767 6572 2e64 6562 7567 2822 2a2a 2a2a  gger.debug("****
+000155a0: 2a2a 4361 6272 696c 6c6f 2a2a 2a2a 2a22  **Cabrillo*****"
+000155b0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+000155c0: 6f6e 7465 7374 2e63 6162 7269 6c6c 6f28  ontest.cabrillo(
+000155d0: 7365 6c66 290a 0a0a 6465 6620 6c6f 6164  self)...def load
+000155e0: 5f66 6f6e 7473 5f66 726f 6d5f 6469 7228  _fonts_from_dir(
+000155f0: 6469 7265 6374 6f72 793a 2073 7472 2920  directory: str) 
+00015600: 2d3e 2073 6574 3a0a 2020 2020 2222 220a  -> set:.    """.
+00015610: 2020 2020 5765 6c6c 2069 7420 6c6f 6164      Well it load
+00015620: 7320 666f 6e74 7320 6672 6f6d 2061 2064  s fonts from a d
+00015630: 6972 6563 746f 7279 2e2e 2e0a 2020 2020  irectory....    
+00015640: 2222 220a 2020 2020 666f 6e74 5f66 616d  """.    font_fam
+00015650: 696c 6965 7320 3d20 7365 7428 290a 2020  ilies = set().  
+00015660: 2020 666f 7220 5f66 6920 696e 2051 4469    for _fi in QDi
+00015670: 7228 6469 7265 6374 6f72 7929 2e65 6e74  r(directory).ent
+00015680: 7279 496e 666f 4c69 7374 285b 222a 2e74  ryInfoList(["*.t
+00015690: 7466 222c 2022 2a2e 776f 6666 222c 2022  tf", "*.woff", "
+000156a0: 2a2e 776f 6666 3222 5d29 3a0a 2020 2020  *.woff2"]):.    
+000156b0: 2020 2020 5f69 6420 3d20 5146 6f6e 7444      _id = QFontD
+000156c0: 6174 6162 6173 652e 6164 6441 7070 6c69  atabase.addAppli
+000156d0: 6361 7469 6f6e 466f 6e74 285f 6669 2e61  cationFont(_fi.a
+000156e0: 6273 6f6c 7574 6546 696c 6550 6174 6828  bsoluteFilePath(
+000156f0: 2929 0a20 2020 2020 2020 2066 6f6e 745f  )).        font_
+00015700: 6661 6d69 6c69 6573 207c 3d20 7365 7428  families |= set(
+00015710: 5146 6f6e 7444 6174 6162 6173 652e 6170  QFontDatabase.ap
+00015720: 706c 6963 6174 696f 6e46 6f6e 7446 616d  plicationFontFam
+00015730: 696c 6965 7328 5f69 6429 290a 2020 2020  ilies(_id)).    
+00015740: 7265 7475 726e 2066 6f6e 745f 6661 6d69  return font_fami
+00015750: 6c69 6573 0a0a 0a64 6566 2069 6e73 7461  lies...def insta
+00015760: 6c6c 5f69 636f 6e73 2829 3a0a 2020 2020  ll_icons():.    
+00015770: 2222 2249 6e73 7461 6c6c 2069 636f 6e73  """Install icons
+00015780: 2222 220a 2020 2020 6f73 2e73 7973 7465  """.    os.syste
+00015790: 6d28 0a20 2020 2020 2020 2022 7864 672d  m(.        "xdg-
+000157a0: 6963 6f6e 2d72 6573 6f75 7263 6520 696e  icon-resource in
+000157b0: 7374 616c 6c20 2d2d 7369 7a65 2033 3220  stall --size 32 
+000157c0: 2d2d 636f 6e74 6578 7420 6170 7073 202d  --context apps -
+000157d0: 2d6d 6f64 6520 7573 6572 2022 0a20 2020  -mode user ".   
+000157e0: 2020 2020 2066 227b 574f 524b 494e 475f       f"{WORKING_
+000157f0: 5041 5448 7d2f 6461 7461 2f6b 3667 7465  PATH}/data/k6gte
+00015800: 2e6e 6f74 316d 6d2d 3332 2e70 6e67 206b  .not1mm-32.png k
+00015810: 3667 7465 2d6e 6f74 316d 6d22 0a20 2020  6gte-not1mm".   
+00015820: 2029 0a20 2020 206f 732e 7379 7374 656d   ).    os.system
+00015830: 280a 2020 2020 2020 2020 2278 6467 2d69  (.        "xdg-i
+00015840: 636f 6e2d 7265 736f 7572 6365 2069 6e73  con-resource ins
+00015850: 7461 6c6c 202d 2d73 697a 6520 3634 202d  tall --size 64 -
+00015860: 2d63 6f6e 7465 7874 2061 7070 7320 2d2d  -context apps --
+00015870: 6d6f 6465 2075 7365 7220 220a 2020 2020  mode user ".    
+00015880: 2020 2020 6622 7b57 4f52 4b49 4e47 5f50      f"{WORKING_P
+00015890: 4154 487d 2f64 6174 612f 6b36 6774 652e  ATH}/data/k6gte.
+000158a0: 6e6f 7431 6d6d 2d36 342e 706e 6720 6b36  not1mm-64.png k6
+000158b0: 6774 652d 6e6f 7431 6d6d 220a 2020 2020  gte-not1mm".    
+000158c0: 290a 2020 2020 6f73 2e73 7973 7465 6d28  ).    os.system(
+000158d0: 0a20 2020 2020 2020 2022 7864 672d 6963  .        "xdg-ic
+000158e0: 6f6e 2d72 6573 6f75 7263 6520 696e 7374  on-resource inst
+000158f0: 616c 6c20 2d2d 7369 7a65 2031 3238 202d  all --size 128 -
+00015900: 2d63 6f6e 7465 7874 2061 7070 7320 2d2d  -context apps --
+00015910: 6d6f 6465 2075 7365 7220 220a 2020 2020  mode user ".    
+00015920: 2020 2020 6622 7b57 4f52 4b49 4e47 5f50      f"{WORKING_P
+00015930: 4154 487d 2f64 6174 612f 6b36 6774 652e  ATH}/data/k6gte.
+00015940: 6e6f 7431 6d6d 2d31 3238 2e70 6e67 206b  not1mm-128.png k
+00015950: 3667 7465 2d6e 6f74 316d 6d22 0a20 2020  6gte-not1mm".   
+00015960: 2029 0a20 2020 206f 732e 7379 7374 656d   ).    os.system
+00015970: 2866 2278 6467 2d64 6573 6b74 6f70 2d6d  (f"xdg-desktop-m
+00015980: 656e 7520 696e 7374 616c 6c20 7b57 4f52  enu install {WOR
+00015990: 4b49 4e47 5f50 4154 487d 2f64 6174 612f  KING_PATH}/data/
+000159a0: 6b36 6774 652d 6e6f 7431 6d6d 2e64 6573  k6gte-not1mm.des
+000159b0: 6b74 6f70 2229 0a0a 0a64 6566 2064 6f69  ktop")...def doi
+000159c0: 6d70 286d 6f64 6e61 6d65 293a 0a20 2020  mp(modname):.   
+000159d0: 2022 2222 7265 7475 726e 206d 6f64 756c   """return modul
+000159e0: 6520 7061 7468 2222 220a 2020 2020 7265  e path""".    re
+000159f0: 7475 726e 2069 6d70 6f72 746c 6962 2e69  turn importlib.i
+00015a00: 6d70 6f72 745f 6d6f 6475 6c65 2866 226e  mport_module(f"n
+00015a10: 6f74 316d 6d2e 706c 7567 696e 732e 7b6d  ot1mm.plugins.{m
+00015a20: 6f64 6e61 6d65 7d22 290a 0a0a 6465 6620  odname}")...def 
+00015a30: 7275 6e28 293a 0a20 2020 2022 2222 0a20  run():.    """. 
+00015a40: 2020 204d 6169 6e20 456e 7472 790a 2020     Main Entry.  
+00015a50: 2020 2222 220a 2020 2020 696e 7374 616c    """.    instal
+00015a60: 6c5f 6963 6f6e 7328 290a 2020 2020 7469  l_icons().    ti
+00015a70: 6d65 722e 7374 6172 7428 3235 3029 0a20  mer.start(250). 
+00015a80: 2020 2073 7973 2e65 7869 7428 6170 702e     sys.exit(app.
+00015a90: 6578 6563 2829 290a 0a0a 6c6f 6767 6572  exec())...logger
+00015aa0: 203d 206c 6f67 6769 6e67 2e67 6574 4c6f   = logging.getLo
+00015ab0: 6767 6572 2822 5f5f 6d61 696e 5f5f 2229  gger("__main__")
+00015ac0: 0a68 616e 646c 6572 203d 206c 6f67 6769  .handler = loggi
+00015ad0: 6e67 2e53 7472 6561 6d48 616e 646c 6572  ng.StreamHandler
+00015ae0: 2829 0a66 6f72 6d61 7474 6572 203d 206c  ().formatter = l
+00015af0: 6f67 6769 6e67 2e46 6f72 6d61 7474 6572  ogging.Formatter
+00015b00: 280a 2020 2020 6461 7465 666d 743d 2225  (.    datefmt="%
+00015b10: 483a 254d 3a25 5322 2c0a 2020 2020 666d  H:%M:%S",.    fm
+00015b20: 743d 225b 2528 6173 6374 696d 6529 735d  t="[%(asctime)s]
+00015b30: 2025 286c 6576 656c 6e61 6d65 2973 2025   %(levelname)s %
+00015b40: 286d 6f64 756c 6529 7320 2d20 2528 6675  (module)s - %(fu
+00015b50: 6e63 4e61 6d65 2973 204c 696e 6520 2528  ncName)s Line %(
+00015b60: 6c69 6e65 6e6f 2964 3a20 2528 6d65 7373  lineno)d: %(mess
+00015b70: 6167 6529 7322 2c0a 290a 6861 6e64 6c65  age)s",.).handle
+00015b80: 722e 7365 7446 6f72 6d61 7474 6572 2866  r.setFormatter(f
+00015b90: 6f72 6d61 7474 6572 290a 6c6f 6767 6572  ormatter).logger
+00015ba0: 2e61 6464 4861 6e64 6c65 7228 6861 6e64  .addHandler(hand
+00015bb0: 6c65 7229 0a0a 4245 5441 5f54 4553 5420  ler)..BETA_TEST 
+00015bc0: 3d20 4661 6c73 650a 6966 2050 6174 6828  = False.if Path(
+00015bd0: 222e 2f62 6574 6174 6573 7422 292e 6578  "./betatest").ex
+00015be0: 6973 7473 2829 3a0a 2020 2020 4245 5441  ists():.    BETA
+00015bf0: 5f54 4553 5420 3d20 5472 7565 0a0a 6966  _TEST = True..if
+00015c00: 2050 6174 6828 222e 2f64 6562 7567 2229   Path("./debug")
+00015c10: 2e65 7869 7374 7328 293a 0a20 2020 206c  .exists():.    l
+00015c20: 6f67 6765 722e 7365 744c 6576 656c 286c  ogger.setLevel(l
+00015c30: 6f67 6769 6e67 2e44 4542 5547 290a 2020  ogging.DEBUG).  
+00015c40: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00015c50: 6465 6275 6767 696e 6720 6f6e 2229 0a65  debugging on").e
+00015c60: 6c73 653a 0a20 2020 206c 6f67 6765 722e  lse:.    logger.
+00015c70: 7365 744c 6576 656c 286c 6f67 6769 6e67  setLevel(logging
+00015c80: 2e57 4152 4e49 4e47 290a 2020 2020 6c6f  .WARNING).    lo
+00015c90: 6767 6572 2e77 6172 6e69 6e67 2822 6465  gger.warning("de
+00015ca0: 6275 6767 696e 6720 6f66 6622 290a 0a61  bugging off")..a
+00015cb0: 7070 203d 2051 7457 6964 6765 7473 2e51  pp = QtWidgets.Q
+00015cc0: 4170 706c 6963 6174 696f 6e28 7379 732e  Application(sys.
+00015cd0: 6172 6776 290a 6170 702e 7365 7453 7479  argv).app.setSty
+00015ce0: 6c65 2822 4164 7761 6974 612d 4461 726b  le("Adwaita-Dark
+00015cf0: 2229 0a66 6f6e 745f 7061 7468 203d 2057  ").font_path = W
+00015d00: 4f52 4b49 4e47 5f50 4154 4820 2b20 222f  ORKING_PATH + "/
+00015d10: 6461 7461 220a 6661 6d69 6c69 6573 203d  data".families =
+00015d20: 206c 6f61 645f 666f 6e74 735f 6672 6f6d   load_fonts_from
+00015d30: 5f64 6972 286f 732e 6673 7061 7468 2866  _dir(os.fspath(f
+00015d40: 6f6e 745f 7061 7468 2929 0a6c 6f67 6765  ont_path)).logge
+00015d50: 722e 696e 666f 2866 616d 696c 6965 7329  r.info(families)
+00015d60: 0a77 696e 646f 7720 3d20 4d61 696e 5769  .window = MainWi
+00015d70: 6e64 6f77 2829 0a68 6569 6768 7420 3d20  ndow().height = 
+00015d80: 7769 6e64 6f77 2e70 7265 662e 6765 7428  window.pref.get(
+00015d90: 2277 696e 646f 775f 6865 6967 6874 222c  "window_height",
+00015da0: 2033 3030 290a 7769 6474 6820 3d20 7769   300).width = wi
+00015db0: 6e64 6f77 2e70 7265 662e 6765 7428 2277  ndow.pref.get("w
+00015dc0: 696e 646f 775f 7769 6474 6822 2c20 3730  indow_width", 70
+00015dd0: 3029 0a78 203d 2077 696e 646f 772e 7072  0).x = window.pr
+00015de0: 6566 2e67 6574 2822 7769 6e64 6f77 5f78  ef.get("window_x
+00015df0: 222c 202d 3129 0a79 203d 2077 696e 646f  ", -1).y = windo
+00015e00: 772e 7072 6566 2e67 6574 2822 7769 6e64  w.pref.get("wind
+00015e10: 6f77 5f79 222c 202d 3129 0a77 696e 646f  ow_y", -1).windo
+00015e20: 772e 7365 7447 656f 6d65 7472 7928 782c  w.setGeometry(x,
+00015e30: 2079 2c20 7769 6474 682c 2068 6569 6768   y, width, heigh
+00015e40: 7429 0a77 696e 646f 772e 6361 6c6c 7369  t).window.callsi
+00015e50: 676e 2e73 6574 466f 6375 7328 290a 7769  gn.setFocus().wi
+00015e60: 6e64 6f77 2e73 686f 7728 290a 7469 6d65  ndow.show().time
+00015e70: 7220 3d20 5174 436f 7265 2e51 5469 6d65  r = QtCore.QTime
+00015e80: 7228 290a 7469 6d65 722e 7469 6d65 6f75  r().timer.timeou
+00015e90: 742e 636f 6e6e 6563 7428 7769 6e64 6f77  t.connect(window
+00015ea0: 2e70 6f6c 6c5f 7261 6469 6f29 0a0a 6966  .poll_radio)..if
+00015eb0: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00015ec0: 6d61 696e 5f5f 223a 0a20 2020 2072 756e  main__":.    run
+00015ed0: 2829 0a                                  ().
```

### Comparing `not1mm-23.6.14/not1mm/bandmap.py` & `not1mm-23.6.2/not1mm/bandmap.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.6.2/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/MASTER.SCP` & `not1mm-23.6.2/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/about.ui` & `not1mm-23.6.2/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/bandmap.ui` & `not1mm-23.6.2/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/configuration.ui` & `not1mm-23.6.2/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/contests.sql` & `not1mm-23.6.2/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/cty.json` & `not1mm-23.6.2/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/cty_old.json` & `not1mm-23.6.2/not1mm/data/cty_old.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/editcontact.ui` & `not1mm-23.6.2/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/editmacro.ui` & `not1mm-23.6.2/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.6.2/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.6.2/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.6.2/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/logwindow.ui` & `not1mm-23.6.2/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/main.ui` & `not1mm-23.6.2/not1mm/data/main.ui`

 * *Files 0% similar despite different names*

#### Comparing `not1mm-23.6.14/not1mm/data/main.ui` & `not1mm-23.6.2/not1mm/data/main.ui`

```diff
@@ -1052,16 +1052,14 @@
         <addaction name="actionGenerate_Cabrillo"/>
         <addaction name="actionGenerate_ADIF"/>
         <addaction name="separator"/>
         <addaction name="actionConfiguration_Settings"/>
         <addaction name="actionStationSettings"/>
         <addaction name="separator"/>
         <addaction name="actionEdit_Macros"/>
-        <addaction name="separator"/>
-        <addaction name="actionQuit"/>
       </widget>
       <widget class="QMenu" name="menuHelp">
         <property name="title">
           <string>Help</string>
         </property>
         <addaction name="actionAbout"/>
       </widget>
@@ -1447,16 +1445,11 @@
       </property>
       <property name="font">
         <font>
           <family>JetBrains Mono</family>
         </font>
       </property>
     </action>
-    <action name="actionQuit">
-      <property name="text">
-        <string>Quit</string>
-      </property>
-    </action>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `not1mm-23.6.14/not1mm/data/new_contest.ui` & `not1mm-23.6.2/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/opon.ui` & `not1mm-23.6.2/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/0.wav` & `not1mm-23.6.2/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/1.wav` & `not1mm-23.6.2/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/2.wav` & `not1mm-23.6.2/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/3.wav` & `not1mm-23.6.2/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/4.wav` & `not1mm-23.6.2/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/5.wav` & `not1mm-23.6.2/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/6.wav` & `not1mm-23.6.2/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/7.wav` & `not1mm-23.6.2/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/73.wav` & `not1mm-23.6.2/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/8.wav` & `not1mm-23.6.2/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/9.wav` & `not1mm-23.6.2/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/a.wav` & `not1mm-23.6.2/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/again.wav` & `not1mm-23.6.2/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/b.wav` & `not1mm-23.6.2/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/c.wav` & `not1mm-23.6.2/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/contest.wav` & `not1mm-23.6.2/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/cq.wav` & `not1mm-23.6.2/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/d.wav` & `not1mm-23.6.2/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/e.wav` & `not1mm-23.6.2/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/f.wav` & `not1mm-23.6.2/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/g.wav` & `not1mm-23.6.2/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/h.wav` & `not1mm-23.6.2/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/i.wav` & `not1mm-23.6.2/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/j.wav` & `not1mm-23.6.2/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/k.wav` & `not1mm-23.6.2/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.6.2/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/l.wav` & `not1mm-23.6.2/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/m.wav` & `not1mm-23.6.2/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.6.2/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/n.wav` & `not1mm-23.6.2/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/nil.wav` & `not1mm-23.6.2/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/o.wav` & `not1mm-23.6.2/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/p.wav` & `not1mm-23.6.2/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/q.wav` & `not1mm-23.6.2/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/r.wav` & `not1mm-23.6.2/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/roger.wav` & `not1mm-23.6.2/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/s.wav` & `not1mm-23.6.2/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/space.wav` & `not1mm-23.6.2/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/t.wav` & `not1mm-23.6.2/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.6.2/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.6.2/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/u.wav` & `not1mm-23.6.2/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/v.wav` & `not1mm-23.6.2/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/w.wav` & `not1mm-23.6.2/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/x.wav` & `not1mm-23.6.2/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/y.wav` & `not1mm-23.6.2/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.6.2/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/phonetics/z.wav` & `not1mm-23.6.2/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/pickcontest.ui` & `not1mm-23.6.2/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/reddot.png` & `not1mm-23.6.2/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/data/settings.ui` & `not1mm-23.6.2/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/lib/cat_interface.py` & `not1mm-23.6.2/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/lib/cwinterface.py` & `not1mm-23.6.2/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/lib/database.py` & `not1mm-23.6.2/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/lib/edit_macro.py` & `not1mm-23.6.2/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/lib/edit_station.py` & `not1mm-23.6.2/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/lib/ham_utility.py` & `not1mm-23.6.2/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/lib/lookup.py` & `not1mm-23.6.2/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/lib/multicast.py` & `not1mm-23.6.2/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/lib/n1mm.py` & `not1mm-23.6.2/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/lib/settings.py` & `not1mm-23.6.2/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/lib/versiontest.py` & `not1mm-23.6.2/not1mm/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/logwindow.py` & `not1mm-23.6.2/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.6.2/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.6.2/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.6.2/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.6.2/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.6.2/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.6.2/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/arrl_field_day.py` & `not1mm-23.6.2/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.6.2/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.6.2/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.6.2/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.6.2/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.6.2/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.6.2/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.6.2/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/cwt.py` & `not1mm-23.6.2/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/general_logging.py` & `not1mm-23.6.2/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/jidx_cw.py` & `not1mm-23.6.2/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/jidx_ph.py` & `not1mm-23.6.2/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/plugins/winter_field_day.py` & `not1mm-23.6.2/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/testing/fakeflrig.py` & `not1mm-23.6.2/not1mm/testing/fakeflrig.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/testing/flrigclient.py` & `not1mm-23.6.2/not1mm/testing/flrigclient.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/testing/n1mm_listener.py` & `not1mm-23.6.2/not1mm/testing/n1mm_listener.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm/testing/test.py` & `not1mm-23.6.2/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.14/not1mm.egg-info/PKG-INFO` & `not1mm-23.6.2/not1mm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.6.14
+Version: 23.6.2
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,15 +15,14 @@
 Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Not1MM
 
-[![PyPI](https://img.shields.io/pypi/v/not1mm)](https://pypi.org/project/not1mm/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Python: 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
 [![Made With:PyQt5](https://img.shields.io/badge/Made%20with-PyQt5-red)](https://pypi.org/project/PyQt5/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/not1mm)](https://pypi.org/project/not1mm/)
 
 ![logo](https://github.com/mbridak/not1mm/raw/master/not1mm/data/k6gte.not1mm.svg)
 
@@ -137,16 +136,14 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-6-14] Added check to see if your Russ and want to operate a contest thats not defined.
-- [23-6-12] Add `File->Quit` because Russ can't click an 'x' to quit program.
 - [23-6-2] Added an automated check and update of the cty.dat file. Added dependency to `notctyparser`
 
 <details>
 
 <summary>May 2023</summary>
 
 - [23-5-31] updated cty.json ( I need to automate this )
```

### Comparing `not1mm-23.6.14/not1mm.egg-info/SOURCES.txt` & `not1mm-23.6.2/not1mm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 not1mm/__init__.py
 not1mm/__main__.py
 not1mm/bandmap.py
 not1mm/logwindow.py
-not1mm/map.py
 not1mm.egg-info/PKG-INFO
 not1mm.egg-info/SOURCES.txt
 not1mm.egg-info/dependency_links.txt
 not1mm.egg-info/entry_points.txt
 not1mm.egg-info/requires.txt
 not1mm.egg-info/top_level.txt
 not1mm/data/JetBrainsMono-Regular.ttf
@@ -29,15 +28,14 @@
 not1mm/data/greendot.png
 not1mm/data/k6gte-not1mm.desktop
 not1mm/data/k6gte.not1mm-128.png
 not1mm/data/k6gte.not1mm-32.png
 not1mm/data/k6gte.not1mm-64.png
 not1mm/data/logwindow.ui
 not1mm/data/main.ui
-not1mm/data/map.ui
 not1mm/data/new_contest.ui
 not1mm/data/opon.ui
 not1mm/data/pickcontest.ui
 not1mm/data/reddot.png
 not1mm/data/settings.ui
 not1mm/data/ssbmacros.txt
 not1mm/data/phonetics/0.wav
```

### Comparing `not1mm-23.6.14/pyproject.toml` & `not1mm-23.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.6.14"
+version = "23.6.2"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

